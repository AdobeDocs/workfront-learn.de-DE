---
title: Verstehen von EXISTS-Filtern
description: Erfahren Sie, was ein EXISTS-Filter ist, welche Möglichkeiten er Ihnen bietet und wie Sie einen Filter von Grund auf neu erstellen können. Außerdem erhalten Sie viele nützliche Beispiele für EXISTS-Filter.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 100%

---

# Verstehen von EXISTS-Filtern

EXISTS-Filter sind erweiterte Textmodusfilter, mit denen wir in einem standardmäßigen Report Builder die Sprungbegrenzung auf zwei Tabellen/Felder umgehen können. Sie können auch verwendet werden, um über NOTEXISTS Objekte im System zu identifizieren, denen eine bestimmte Beziehungsbedingung fehlt.

In diesem Video erfahren Sie, wie Sie einen EXISTS-Filter erstellen, um Korrekturabzug-Genehmigungen für aktuelle Projekte in einem Bericht zu Korrekturabzug-Genehmigungen anzuzeigen.

Eine ausführlichere Anleitung zur Funktionsweise von EXISTS finden Sie in der Dokumentation [Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen](https://experienceleague.adobe.com/de/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements).

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## Beispiele für EXISTS-Filter

### Project Report EXISTS (Projektbericht VORHANDEN)

Hierbei dient die Aufgabe als Verknüpfungsobjekt, indem die auf der Aufgabenebene gefundene Projekt-ID verglichen und mit dem ID-Feld auf der Projektebene abgeglichen wird. Auf diese Weise können wir dann die Zuweisung von Benutzenden zur Aufgabe mit einem $$USER.ID-Platzhalter vergleichen. Dies führt dazu, dass nur Projekte zurückgegeben werden, bei denen die bzw. der anzeigende Benutzende einer
Aufgabe zugewiesen ist, unabhängig davon, ob sie bzw. er die primäre zugewiesene Person ist oder nicht.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Hierbei wird das Problem (optask) als Verknüpfungsobjekt verwendet, indem auch die auf der Problemebene (optask) gefundene Projekt-ID verglichen und mit jener im ID-Feld auf Projektebene abgeglichen wird. So wird geprüft, ob bei einem dieser Probleme (optasks) ein Eingabedatum innerhalb des angegebenen Zeitraums vorhanden ist. In dem Fall würden alle Projekte zurückgegeben, bei denen
in den letzten 30 Tagen (rollierend) aufgrund des NOTEXISTS kein Problem (optask) protokolliert wurde.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Template Report EXISTS (Vorlagenbericht VORHANDEN)

Dieser Filter zeigt alle Vorlagen an, die im letzten Jahr nicht zur Erstellung eines Projekts verwendet oder an ein Projekt angehängt wurden. Voraussetzung: Damit sich ermitteln lässt, ob eine Vorlage als Anhang verwendet wurde oder nicht, muss diese Vorlage über Aufgaben verfügen.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### Task Report EXISTS (Aufgabenbericht VORHANDEN)

Hierbei wird die Benutzertabelle als Verknüpfungsobjekt verwendet, wobei zur Verknüpfung die taskID des Arbeitsauftrags und die Aufgaben-ID dienen. Diese gleicht dann die Team-Sammlung der IDs mit den Team-IDs der Benutzenden ab und gibt die Aufgabe zurück, wenn eine der verantwortlichen Personen im selben Team wie die bzw. der anzeigende Benutzende ist.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### User Report EXISTS (Benutzerbericht VORHANDEN)

Damit werden alle Benutzenden zurückgegeben, die in den letzten 3 Wochen kein Update gepostet haben. Dabei wird das Notizobjekt verwendet, um die Lücke zu schließen, und die Eigentümer-ID wird mit einer Benutzer-ID verglichen. Gibt dann diese Benutzende bzw. diesen Benutzenden zurück, wenn das Eingabedatum aller ihrer bzw. seiner Notizen maximal drei Wochen zurückliegt.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Damit werden alle Benutzenden zurückgegeben, die in der letzten Woche keine Stunden eingetragen haben. Hierbei kommt eine extrem ähnliche Methode wie im obigen Beispiel zum Einsatz. Es werden jedoch die Informationen zur Stundeneigentümerin bzw. zum Stundeneigentümer und das Datum der Stundeneingabe verwendet, um zu ermitteln, welche Benutzenden zurückgegeben werden.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

Zeigen Sie in einem Benutzerbericht eine Liste von Benutzenden an, die mit der Registerkarte „Personen“ eines Projekts übereinstimmt.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Category (Custom Form) Report EXISTS (Kategorienbericht (benutzerdefiniertes Formular) VORHANDEN)

Dieser Text enthält eine Liste aller Projektformulare, die noch nie in einem Projekt verwendet wurden. Dies sollte zusammen mit der Angabe des Objekttyps des Formulars verwendet werden, auf das wir uns konzentrieren. In diesem Fall ist der Fokus also PROJ, sodass wir die Hinweise in die objTypes-Zeilen einbeziehen sollten. Dies könnte für andere
Objekttypen verwendet werden, indem die Teile, die sich auf den Objekt-Code beziehen, verändert werden. Dadurch wird die Sammlung der mit Projekten verbundenen Formulare mit den aufgelisteten Formularen abgeglichen und ausgegeben, wenn keine Übereinstimmung vorliegt.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Parameter (Custom Field) Report EXISTS (Parameterbericht (benutzerdefiniertes Feld) VORHANDEN)

Dadurch werden alle benutzerdefinierten Felder zurückgegeben, die derzeit nicht mit einem benutzerdefinierten Formular im System verbunden sind.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Report EXISTS (Bericht VORHANDEN)

Dadurch werden alle Berichte zurückgegeben, die einen bestimmten Wert in ihren Filtern nutzen.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Dadurch werden alle Berichte zurückgegeben, die an ein Dashboard angehängt sind.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### Proof Approval Report EXISTS (Korrekturabzug-Genehmigungsbericht VORHANDEN)

Dadurch würden Korrekturabzug-Genehmigungen nur für Projekte mit dem Status „Aktuell“ zurückgegeben. Dabei wird das Dokumentobjekt verwendet, um die Lücke von der Korrekturabzug-Genehmigung zum Projekt zu schließen, indem die currentVersionID mit der documentVersionID abgeglichen wird. Von dort aus springen wir zum Projektstatus.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```

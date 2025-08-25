---
title: Vorhandene Filter verstehen
description: Erfahren Sie, was ein EXISTS-Filter ist, was er für Sie tun kann und wie Sie einen Filter von Grund auf neu erstellen können. Außerdem sehen Sie viele nützliche Beispiele für EXISTS-Filter.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
source-git-commit: 7be0b8cce9cba04927d6704d0009b482bbcf4b41
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Vorhandene Filter verstehen

EXISTS-Filter sind erweiterte Textmodusfilter, mit denen wir die Begrenzung auf 2 Tabellen/Felder in einem standardmäßigen Report Builder umgehen können. Sie können auch verwendet werden, um Objekte im System zu identifizieren, denen eine bestimmte Beziehungsbedingung über NOTEXISTS fehlt.

In diesem Video erfahren Sie, wie Sie einen EXISTS-Filter erstellen, um „Korrekturabzugsgenehmigungen für aktuelle Projekte“ in einem Bericht zu Korrekturabzugsgenehmigungen anzuzeigen.

Eine ausführlichere Anleitung zur Funktionsweise von EXISTS finden Sie in der Dokumentation [Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen](https://experienceleague.adobe.com/de/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) .

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops)

## EXISTS Filter Beispiele

### Projektbericht VORHANDEN

Hierbei wird die Aufgabe als Verknüpfungsobjekt verwendet, indem die auf Aufgabenebene gefundene Projekt-ID verglichen und mit dem ID-Feld auf Projektebene abgeglichen wird. Auf diese Weise können wir dann die Zuweisung von Benutzern für die Aufgabe mit einem $$USER.ID-Platzhalter vergleichen. Dies führt dazu, dass nur Projekte zurückgegeben werden, bei denen der anzeigende Benutzer einem
Aufgabe, unabhängig davon, ob sie der primäre Zugewiesene ist oder nicht.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Hierbei wird das Problem (optask) als Verknüpfungsobjekt verwendet, indem auch die auf der Problem-Ebene (optask) gefundene Projekt-ID verglichen wird und mit dieser im Feld für die ID auf Projektebene abgeglichen wird. Dadurch wird überprüft, ob bei einem dieser Probleme (Optasks) ein Eingabedatum innerhalb des angegebenen Zeitraums vorhanden ist. In diesem Fall würde es jedes Projekt zurückgeben, das
In den letzten 30 Tagen wurde aufgrund des NOTEXISTS kein Problem (Optask) rollierend protokolliert.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Vorlagenbericht VORHANDEN

Dieser Filter zeigt alle Vorlagen an, die im letzten Jahr nicht zur Erstellung eines Projekts verwendet oder an ein Projekt angehängt wurden. Ein Nachteil besteht darin, dass eine Vorlage, um herauszufinden, ob sie als Anhang verwendet wurde, von Aufgaben in dieser Vorlage abhängt.

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

### Aufgabenbericht VORHANDEN

Hierbei wird die Benutzertabelle als Verknüpfungsobjekt verwendet, das über die taskID des Arbeitsauftrags und die tasksID verbunden wird. Diese prüft dann die Team-Sammlung mit IDs auf die Benutzer-Team-IDs und gibt die Aufgabe zurück, wenn einer der Verantwortlichen im selben Team wie der anzeigende Benutzer ist.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### Benutzerbericht VORHANDEN

Dadurch werden alle Benutzer zurückgegeben, die in den letzten 3 Wochen kein Update gepostet haben. Hierbei wird das Notizobjekt verwendet, um die Lücke zu schließen, und die Eigentümer-ID wird mit einer Benutzer-ID verglichen. Gibt dann diesen Benutzer zurück, wenn vor mehr als drei Wochen kein Notiz in seinem Besitz war.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Dadurch werden alle Benutzenden zurückgegeben, die in der letzten Woche keine Stunden angemeldet haben. Hierbei wird eine extrem ähnliche Methode wie im obigen Beispiel verwendet, stattdessen werden jedoch die Informationen zum Stundeneigentümer und das Datum der Stundeneingabe verwendet, um zu bestimmen, welche Benutzer zurückgegeben werden.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

Zeigen Sie in einem Benutzerbericht eine Liste von Benutzern an, die mit der Registerkarte Personen eines Projekts übereinstimmt.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Bericht zu Kategorien (benutzerdefiniertes Formular) EXISTIERT

Dieser Text enthält eine Liste aller Projektformulare, die niemals in einem Projekt verwendet wurden. Dies sollte zusammen mit der Angabe des Objekttyps des Formulars verwendet werden, auf das wir uns konzentrieren. In diesem Fall ist der Fokus also PROJ, sodass wir die Hinweise in die objTypes-Zeilen einbeziehen sollten. Dies könnte verwendet werden
für andere Objekttypen durch Ändern der Teile, die sich auf den Objektcode beziehen. Dadurch wird die Auflistung der an die Formulare angehängten Projekte überprüft und ausgegeben, wenn keine Übereinstimmung vorliegt.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Parameterbericht (benutzerdefiniertes Feld) EXISTIERT

Dadurch werden alle benutzerdefinierten Felder zurückgegeben, die derzeit nicht mit einem benutzerdefinierten Formular im System verbunden sind.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Bericht VORHANDEN

Dadurch wird jeder Bericht zurückgegeben, der einen bestimmten Wert in seinen Filtern verwendet.

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

### Korrekturabzugs-Genehmigungsbericht EXISTIERT

Dadurch würden Korrekturabzugs-Genehmigungen nur für Projekte mit dem Status „Aktuell“ zurückgegeben. Dabei wird das Dokumentobjekt verwendet, um die Lücke von der Korrekturabzugsgenehmigung zum Projekt zu schließen, indem die currentVersionID zur documentVersionID überprüft wird. Von dort aus springen wir zum Projektstatus.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```

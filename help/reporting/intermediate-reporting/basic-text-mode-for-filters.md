---
title: Grundlegendes zum Textmodus für Filter
description: Erfahren Sie, was der Textmodus ist, welche Binnenmajuskel-Groß-/Kleinschreibung ist und welchen einfachen "Plug-and-Play"-Textmodus Sie in Ihren Berichtsfiltern in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Grundlegendes zum Textmodus für Filter

>[!IMPORTANT]
>
>Voraussetzungen:
>
>* Berichterstellungselemente
>* Berichtkomponenten verstehen
>* Basisfilter erstellen


In diesem Video erfahren Sie:

* Textmodus
* Was für ein Kamel ist
* Grundlegender Textmodus &quot;Plug-and-Play&quot;, den Sie in Ihren Berichtsfiltern verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

Im folgenden Textmodus werden Aufgaben ausgeschlossen, bei denen ein Benutzer &quot;Fertig mit My Part&quot;markiert hat. Sie müssen lediglich einen Aufgabenfilter erstellen, beliebige Filterregeln hinzufügen, dann in den Textmodus wechseln und den unten stehenden Code nach einem beliebigen Textmodus einfügen, der im Filter angezeigt wird.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Zusätzliche Textmodusfilter für Plug-ins und Wiedergeben

### Aufgabe - Zeigt alle Aufgaben an, die auf meine Genehmigung warten

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Aufgabe - Zeigt alle Aufgaben an, die ich genehmigt habe

Erstellen Sie einen Aufgabenbericht mit den gewünschten Filtern. Gehen Sie dann zur Registerkarte Filter und klicken Sie auf In Textmodus wechseln . Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Aufgabe - Zeigt alle Aufgaben an, die mindestens einen projektübergreifenden Vorgänger haben

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Aufgabe - Zeigt alle Aufgaben an, die ich anderen zugewiesen habe

Erstellen Sie einen Aufgabenbericht mit den gewünschten Filtern. Gehen Sie dann zur Registerkarte Filter und klicken Sie auf In Textmodus wechseln . Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Auf diese Weise werden alle Aufgaben angezeigt, denen der angemeldete Benutzer mindestens einen der aktuellen Verantwortlichen zugewiesen hat. Wenn die Zuweisung von mehreren Benutzern erfolgt ist, wird nur der Name der ersten Person, der die Person zugewiesen hat, auf der Aufgabenlandeseite als &quot;Anfordert von&quot;angezeigt.

## Aktivität: Textmodusfragen

1. Wie würden Sie die Binnenmajuskel-Schreibweise für das Feld &quot;Eingegeben von ID&quot;schreiben?
1. Erstellen Sie in einem Problembericht einen Filter, um Probleme anzuzeigen, die als geschlossen gekennzeichnet wurden, aber noch nicht genehmigt wurden.

### Antworten

1. Die Binnenmajuskeln-Schreibweise für das Feld &quot;Eingegeben von ID&quot; sollte wie folgt geschrieben werden: signedByID
1. Der Textmodus sollte im Filter für Problemberichte wie folgt aussehen:

   ![Ein Bild des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/btm-answer.png)

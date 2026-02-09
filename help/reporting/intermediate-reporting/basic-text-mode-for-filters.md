---
title: Erkunden des einfachen Textmodus für Filter in Workfront
description: Erfahren Sie mehr über den Textmodus, die Binnenmajuskel sowie über einen einfachen Textmodus, den Sie in Berichtsfiltern verwenden können.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 96%

---

# Erkunden des einfachen Textmodus für Filter in Workfront

>[!PREREQUISITES]
>
>* [Grundlegendes zu Reporting-Elementen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=de)
>* [Grundlegendes zu Reporting-Komponenten](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=de)
>* [Einen einfachen Filter erstellen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=de)


>[!TIP]
>
>* Um ein tieferes Verständnis des Textmodus zu erhalten, empfehlen wir Ihnen, sich die einstündige Aufzeichnung des folgenden Webinars anzusehen: [Experten fragen – Einführung in die Berichterstellung zum Textmodus](https://experienceleague.adobe.com/de/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting).
>* Um mehr über den Textmodus zu erfahren, sollten Sie sich die Tutorials [Erweiterte Berichterstellung](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=de) ansehen, die insgesamt fünfeinhalb Stunden lang sind.
>* Klicken Sie hier, um auf den [[!UICONTROL API-Explorer]](https://developer.adobe.com/workfront/api-explorer/) zuzugreifen


In diesem Video lernen Sie Folgendes:

* Textmodus
* Binnenmajuskel
* Einige _Code-Blöcke für den Textmodus_, die Sie in Berichtsfiltern verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/3418630/?captions=ger&quality=12&learn=on&enablevpops=0)

## Aktivitäten: Grundlegendes zum einfachen Textmodus für Filter


### Aufgabe – Aufgaben herausfiltern, die ich als „Fertig mit meinem Teil“ markiert habe

Der folgende Textmodus schließt Aufgaben aus, bei denen Benutzende „Fertig mit meinem Teil“ markiert haben. Sie müssen lediglich einen Aufgabenfilter erstellen, beliebige Filterregeln hinzufügen, dann in den Textmodus wechseln und den unten stehenden Code nach einem beliebigen Textmodus einfügen, der im Filter angezeigt wird.


>[!WARNING]
>
> Dies ist nicht für die Verwendung in Kalenderfiltern vorgesehen.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Aufgabe – Alle Aufgaben anzeigen, die auf meine Genehmigung warten

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Aufgabe – Alle Aufgaben anzeigen, die ich genehmigt habe

Erstellen Sie einen Aufgabenbericht mit den von Ihnen gewünschten Filtern, gehen Sie dann auf die Registerkarte „Filter“ und klicken Sie auf „Zum Textmodus wechseln“. Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Aufgabe – Alle Aufgaben anzeigen, die mindestens einen projektübergreifenden Vorgänger haben

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Aufgabe – Alle Aufgaben anzeigen, die ich anderen zugewiesen habe

Erstellen Sie einen Aufgabenbericht mit den von Ihnen gewünschten Filtern, gehen Sie dann auf die Registerkarte „Filter“ und klicken Sie auf „Zum Textmodus wechseln“. Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

>[!WARNING]
> 
> Dies ist nicht für die Verwendung in Kalenderfiltern vorgesehen.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Hier werden Ihnen alle Aufgaben angezeigt, bei denen die angemeldete Person mindestens einer der aktuell beauftragten Personen etwas zugewiesen hat. Wenn die Zuweisung einer Person durch mehrere Benutzende erfolgt ist, wird nur der Name der ersten Person, die jemanden zugewiesen hat, auf der Aufgaben-Landingpage als „Angefordert durch“ angezeigt.

### Aufgabe – Alle Aufgaben anzeigen, die abgeschlossen sind – ausstehende Genehmigung

```
status=CPL:A
status_Mod=in
```


### Problem – Alle Probleme anzeigen, die abgeschlossen sind mit ausstehender Genehmigung

```
status=CPL:A
status_Mod=in
```


### Projekt – Alle Projekte anzeigen, die abgeschlossen sind mit ausstehender Genehmigung

```
status=CPL:A
status_Mod=in
```


### Hinweis – Alle Kommentare anzeigen, in denen ich getaggt bin

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Bericht zu „Parametern/benutzerdefiniertes Feld“ – Benutzerdefinierte Felder anzeigen, die an kein benutzerdefiniertes Formular angehängt sind (sehr nützlich bei Bereinigungen)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

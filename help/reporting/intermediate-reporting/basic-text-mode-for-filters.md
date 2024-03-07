---
title: Grundlegendes zum einfachen Textmodus für Filter
description: Erfahren Sie, was der Textmodus ist, was die Binnenmajuskel-Schreibweise ist und welchen einfachen „Plug-and-Play“-Textmodus Sie in Ihren Berichtsfiltern in Workfront verwenden können.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: ht
source-wordcount: '409'
ht-degree: 100%

---

# Grundlegendes zum einfachen Textmodus für Filter

>[!IMPORTANT]
>
>Voraussetzungen:
>
>* [Grundlegendes zu Reporting-Elementen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=de)
>* [Grundlegendes zu Reporting-Komponenten](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=de)
>* [Einen einfachen Filter erstellen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=de)

>[!TIP]
>
>* Um ein tieferes Verständnis des Textmodus zu erhalten, empfehlen wir Ihnen, sich die einstündige Aufzeichnung des folgenden Webinars anzusehen: [Experten fragen – Einführung in die Berichterstellung zum Textmodus](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=de).
>* Um mehr über den Textmodus zu erfahren, sollten Sie sich die Tutorials [Erweiterte Berichterstellung](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=de) ansehen, die insgesamt fünfeinhalb Stunden lang sind.
>* Klicken Sie hier, um auf den [[!UICONTROL API-Explorer]](https://developer.adobe.com/workfront/api-explorer/) zuzugreifen


In diesem Video lernen Sie Folgendes:

* Was der Textmodus ist
* Was die Binnenmajuskel-Schreibweise ist
* Etwas einfachen „Plug-and-Play“-Textmodus, den Sie in Ihren Berichtsfiltern verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Aufgabe – Aufgaben herausfiltern, die ich als „Fertig mit meinem Teil“ markiert habe

Der folgende Textmodus schließt Aufgaben aus, bei denen Benutzende „Fertig mit meinem Teil“ markiert haben. Sie müssen lediglich einen Aufgabenfilter erstellen, beliebige Filterregeln hinzufügen, dann in den Textmodus wechseln und den unten stehenden Code nach einem beliebigen Textmodus einfügen, der im Filter angezeigt wird.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Aufgabe – Alle Aufgaben anzeigen, die auf meine Genehmigung warten

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Aufgabe – Alle Aufgaben anzeigen, die ich genehmigt habe

Erstellen Sie einen Aufgabenbericht mit den von Ihnen gewünschten Filtern, gehen Sie dann auf die Registerkarte „Filter“ und klicken Sie auf „Zum Textmodus wechseln“. Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Aufgabe – Alle Aufgaben anzeigen, die mindestens einen projektübergreifenden Vorgänger haben

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Aufgabe – Alle Aufgaben anzeigen, die ich anderen zugewiesen habe

Erstellen Sie einen Aufgabenbericht mit den von Ihnen gewünschten Filtern, gehen Sie dann auf die Registerkarte „Filter“ und klicken Sie auf „Zum Textmodus wechseln“. Fügen Sie diesen Code zu dem bereits vorhandenen hinzu:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Hier werden Ihnen alle Aufgaben angezeigt, bei denen die angemeldete Person mindestens einer der aktuell beauftragten Personen etwas zugewiesen hat. Wenn die Zuweisung einer Person durch mehrere Benutzende erfolgt ist, wird nur der Name der ersten Person, die jemanden zugewiesen hat, auf der Aufgaben-Landingpage als „Angefordert durch“ angezeigt.

## Aufgabe – Alle Aufgaben anzeigen, die abgeschlossen sind – ausstehende Genehmigung

```
status=CPL:A
status_Mod=in
```


## Problem – Alle Probleme anzeigen, die abgeschlossen sind mit ausstehender Genehmigung

```
status=CPL:A
status_Mod=in
```


## Projekt – Alle Projekte anzeigen, die abgeschlossen sind mit ausstehender Genehmigung

```
status=CPL:A
status_Mod=in
```


## Hinweis – Alle Kommentare anzeigen, in denen ich getaggt bin

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Bericht zu „Parametern/benutzerdefiniertes Feld“ – Benutzerdefinierte Felder anzeigen, die an kein benutzerdefiniertes Formular angehängt sind (sehr nützlich bei Bereinigungen)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

---
title: Erstellen von OR-Anweisungen in Filtern
description: Die flexible Filterlogik von Workfront ermöglicht es Benutzenden, Berichtsansichten mithilfe von standardmäßigen „UND“-Regeln, optionalen „ODER“-Bedingungen und organisierten Filtergruppen für komplexe Kriterien zu verfeinern.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 100%

---

# Erstellen von OR-Anweisungen in Filtern

In diesem Video wird erläutert, wie sich in Workfront Filter mit verschiedenen Regeln erstellen und verwenden lassen. Standardmäßig nutzt Workfront zwischen Filterregeln „UND“, was bedeutet, dass alle Bedingungen erfüllt sein müssen, damit ein Element in der Liste angezeigt wird.
Alternativ können Sie die Filterlogik in „ODER“ ändern, sodass Elemente angezeigt werden, die mindestens eine der Bedingungen erfüllen.
Im Video wird auch das Erstellen von Filtern für Aufgaben mithilfe von Filtergruppen vorgestellt. Sie können beispielsweise zwei Gruppen erstellen: eine für unvollständige Aufgaben, die dem Kreativ-Team zugewiesen und verspätet sind, und eine weitere für unvollständige Aufgaben, die dem Kreativ-Team zugewiesen sind, aber noch nicht zugeordnet wurden. Innerhalb jeder Gruppe gilt die Logik „UND“, d. h., alle Bedingungen in der Gruppe müssen erfüllt sein. Die „ODER“-Logik zwischen Gruppen stellt sicher, dass Aufgaben, die die Bedingungen mindestens einer der beiden Gruppen erfüllen, angezeigt werden.

>[!VIDEO](https://video.tv.adobe.com/v/3470702/?captions=ger&quality=12&learn=on&enablevpops=0)

## ODER-Filteraktivität

Sie möchten unvollständige Aufgaben finden, die Ihnen oder niemandem zugewiesen sind. Dazu richten Sie den untenstehenden Filter ein. Wird dieser Filter die gewünschten Ergebnisse liefern? Warum oder warum nicht?

![Bild einer falsch erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antworten

Nein, dieser Filter wird nicht die Ergebnisse liefern, die Sie sich erhoffen (unerledigte Aufgaben, die entweder Ihnen oder niemandem zugewiesen sind), weil die Filterregel für den Aufgabenstatus nur auf einer Seite von ODER steht.

Stattdessen generiert dieser Filter eine Liste, die Folgendes anzeigt:

* Ihnen zugewiesene Aufgaben, die unvollständig sind.
* **PLUS (ODER)**
* Alle nicht zugewiesenen Aufgaben, unabhängig vom Status.

Der Filter sollte stattdessen wie folgt aussehen. Beachten Sie, dass bei diesem Filter die Filterregel für den Aufgabenstatus auf beiden Seiten von ODER steht.

![Bild einer ordnungsgemäß erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-2.png)

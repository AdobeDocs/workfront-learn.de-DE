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
last-substantial-update: '2025-08-11T00:00:00.000Z'
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:11:54.379Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 65%

---

# Erstellen von OR-Anweisungen in Filtern

In diesem Video wird erläutert, wie Filter mit mehreren Regeln in Workfront erstellt und verwendet werden. &#x200B; Workfront verwendet standardmäßig „AND“ zwischen Filterregeln, was bedeutet, dass alle Bedingungen erfüllt sein müssen, damit ein Element in der Liste angezeigt wird.
Alternativ können Sie die Filterlogik in „ODER“ ändern, sodass Elemente angezeigt werden, die mindestens eine der Bedingungen erfüllen.
Das Video zeigt auch das Erstellen von Filtern für Aufgaben mithilfe von Filtergruppen. &#x200B; können Sie beispielsweise zwei Gruppen erstellen: eine für nicht abgeschlossene Aufgaben, die dem Kreativ-Team zugewiesen wurden und zu spät kommen, und eine weitere für nicht abgeschlossene Aufgaben, die dem Kreativ-Team zugewiesen wurden und nicht zugewiesen wurden. &#x200B; Innerhalb jeder Gruppe gilt die Logik „AND“, d. h., alle Bedingungen in der Gruppe müssen erfüllt sein. &#x200B; Die „OR“-Logik zwischen Gruppen stellt sicher, dass Aufgaben, die die Bedingungen einer der Gruppen erfüllen, angezeigt werden.

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

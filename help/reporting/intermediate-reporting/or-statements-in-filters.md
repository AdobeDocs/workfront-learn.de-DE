---
title: Erstellen von OR-Anweisungen in Filtern
description: Die flexible Filterlogik von Workfront ermöglicht es Benutzenden, Berichtsansichten mithilfe von Standardregeln für „AND“, optionalen Bedingungen für „OR“ und organisierten Filtergruppen für komplexe Kriterien zu verfeinern.
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
source-git-commit: b3cff8f86ceeb6e79e2b88ab335b2671aa25600a
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 31%

---

# Erstellen von OR-Anweisungen in Filtern

In diesem Video wird erläutert, wie Filter mit mehreren Regeln in Workfront erstellt und verwendet werden. &#x200B; Standardmäßig verwendet Workfront „AND“ zwischen Filterregeln, was bedeutet, dass alle Bedingungen erfüllt sein müssen, damit ein Element in der Liste angezeigt wird.
Alternativ können Sie die Filterlogik in „ODER“ ändern, wodurch Elemente angezeigt werden, die eine der Bedingungen erfüllen.
Das Video zeigt auch das Erstellen von Filtern für Aufgaben mithilfe von Filtergruppen. &#x200B; Sie können beispielsweise zwei Gruppen erstellen: eine für noch nicht abgeschlossene Aufgaben, die dem Kreativ-Team zugewiesen wurden und die dem Kreativ-Team zugewiesen wurden und die andere für noch nicht abgeschlossene Aufgaben, die nicht zugewiesen wurden. &#x200B; Innerhalb jeder Gruppe gilt die Logik „AND“, d. h., alle Bedingungen in der Gruppe müssen erfüllt sein. &#x200B; Die „OR“-Logik zwischen Gruppen stellt sicher, dass Aufgaben, die die Bedingungen einer der Gruppen erfüllen, angezeigt werden.

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on)

## ODER-Filteraktivität

Sie möchten unvollständige Aufgaben finden, die Ihnen oder niemandem zugewiesen sind. Dazu richten Sie den untenstehenden Filter ein. Wird dieser Filter die gewünschten Ergebnisse liefern? Warum oder warum nicht?

![Bild einer falsch erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antworten

Nein, dieser Filter liefert nicht die gewünschten Ergebnisse - Aufgaben, die noch nicht abgeschlossen sind und die Ihnen oder niemandem zugewiesen sind -, da die Filterregel für die Aufgabenvollständigkeit nur auf einer Seite des ODER liegt.

Stattdessen generiert dieser Filter eine Liste, die Folgendes anzeigt:

* Ihnen zugewiesene Aufgaben, die noch nicht abgeschlossen sind.
* **PLUS (ODER)**
* Alle nicht zugewiesenen Aufgaben, unabhängig vom Status.

Der Filter sollte stattdessen wie folgt aussehen. Beachten Sie, dass dieser Filter auf beiden Seiten des ODER die Filterregel für die Vollständigkeit der Aufgaben enthält.

![Bild einer ordnungsgemäß erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-2.png)

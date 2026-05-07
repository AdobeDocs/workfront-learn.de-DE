---
title: Übung zur Aggregation
description: Erfahren Sie, wie Sie mehrere Informationsbündel in einem einzigen Wert zusammenfassen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
recommendations: noDisplay,catalog
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:46:06.511Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 100%

---

# Übung zur Aggregation

Erfahren Sie, wie Sie mehrere Informationsbündel in einem einzigen Wert zusammenfassen.

## Übungsübersicht

Fassen Sie anhand des Szenarios „Einführung in die Iteration“, das Sie in der letzten Übung erstellt haben, die geplanten Stunden für jede Arbeitsaufgabe im Projekt zusammen und senden Sie sich selbst eine E-Mail mit diesen Informationen.

![Aggregation Bild 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Zu befolgende Schritte

**Fügen Sie einen Filter hinzu und summieren Sie die geplanten Stunden.**

1. Klonen Sie das Szenario „Einführung in die Iteration“, das Sie in der vorherigen Übung erstellt haben, und nennen Sie es „Einführung in die Aggregation“.
1. Fügen Sie einen Filter zwischen den Modulen „Projektaufgaben lesen“ und „Anzahl der Aufgaben zählen“ ein. Nennen Sie den Filter „Nur Arbeitsaufgaben“.
1. Setzen Sie die Bedingung auf Anzahl der untergeordneten Elemente [Numerischer Operator: Gleich] 0.

   ![Aggregation Bild 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Fügen Sie nach dem Modul „Zufallsmathematik“ ein Tool-Modul „Numerischer Aggregator“ ein.
1. Setzen Sie das Quellmodul auf „Projektaufgaben lesen“.
1. Setzen Sie die Aggregatfunktion auf „SUMME“.
1. Setzen Sie den Wert auf das Feld „Arbeit“ im Modul „Projektaufgaben lesen“.
1. Benennen Sie dieses Modul in „SUMME aller geplanten Aufgabenstunden“ um.

   ![Aggregation Bild 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Beachten Sie den Schatten, der anzeigt, dass die Aggregation die Iteration beendet.**

   ![Aggregation Bild 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Senden Sie eine E-Mail mit aggregierten Stunden.**

1. Fügen Sie in der E-Mail-App nach dem numerischen Aggregator ein Modul „E-Mail senden“ hinzu.
1. Schicken Sie die E-Mail an sich selbst.
1. Die Betreffzeile lautet „Projektdetails“.
1. Geben Sie in das Inhaltsfeld ein: „Ein Projekt mit dem Namen [Projektname] enthält eine Gesamtzahl von [Ergebnis] geplanten Stunden.“ Der „[Projektname]“ stammt aus dem Modul „Einen Eintrag lesen“ und das „[Ergebnis]“ aus dem Aggregatormodul.

   ![Aggregation Bild 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Speichern Sie und führen Sie einmal aus. Suchen Sie die E-Mail in Ihrem Posteingang.

Innerhalb der Iteration kann auf die einzelnen Bündel zugegriffen werden. Außerhalb der Iteration kann im Modul „E-Mail senden“ jedoch nur auf aggregierte Felder zugegriffen werden.

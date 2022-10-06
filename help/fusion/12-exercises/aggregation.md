---
title: Aggregation
description: Erfahren Sie, wie Sie mehrere Informationsbündel in einem einzigen Wert zusammenfassen.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Aggregation

Erfahren Sie, wie Sie mehrere Informationsbündel in einem einzigen Wert zusammenfassen.

## Übungsübersicht

Mit dem Szenario &quot;Einführung in die Iteration&quot;, das Sie in der letzten Übung erstellt haben, aggregieren Sie die geplanten Stunden für jede Arbeitsaufgabe im Projekt und senden Sie sich eine E-Mail mit diesen Informationen.

![Aggregationsbild 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

**Fügen Sie einen Filter hinzu und fügen Sie die geplanten Stunden hinzu.**

1. Klonen Sie das Szenario &quot;Einführung in die Iteration&quot;, das Sie in der vorherigen Übung erstellt haben, und nennen Sie es &quot;Einführung in die Aggregation&quot;.
1. Fügen Sie einen Filter zwischen dem Modul Aufgaben des Projekts lesen und dem Modul Anzahl der Aufgaben hinzu. Benennen Sie den Filter &quot;Nur funktionierende Aufgaben&quot;.
1. Stellen Sie die Bedingung auf Anzahl der untergeordneten Elemente ein. [Numerischer Operator: Gleich] 0.

   ![Aggregationsbild 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Fügen Sie nach dem Modul &quot;Random Math&quot;ein Tool-Modul &quot;Numerischer Aggregator&quot;hinzu.
1. Legen Sie das Quellmodul auf die Aufgaben des Projekts lesen fest.
1. Setzen Sie die Aggregate-Funktion auf SUM.
1. Legen Sie den Wert im Feld &quot;Arbeit&quot;im Modul &quot;Aufgaben des Projekts lesen&quot;fest.
1. Benennen Sie dieses Modul &quot;SUM aller geplanten Aufgaben&quot;um.

   ![Aggregationsbild 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Beachten Sie den Schatten, der anzeigt, dass die Aggregation die Iteration beendet.**

   ![Aggregationsbild 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Senden Sie eine E-Mail mit aggregierten Stunden.**

1. Fügen Sie nach dem numerischen Aggregator ein E-Mail-Modul Senden aus der E-Mail-App hinzu.
1. Schicken Sie die E-Mail an sich.
1. Die Betreffzeile lautet &quot;Projektdetails&quot;.
1. Legen Sie im Feld &quot;Inhalt&quot;die Option &quot;Es gibt ein Projekt mit dem Namen [Projektname] , die die Gesamtzahl der [result] geplante Stunden.&quot; Die &quot;[Projektname]&quot; wird aus dem Modul &quot;Datensatz lesen&quot;entnommen und &quot;[result]&quot; wird aus dem Aggregatormodul entnommen.

   ![Aggregationsbild 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Speichern und einmal ausführen. Suchen Sie die E-Mail in Ihrem Posteingang.

Innerhalb der Iteration können die einzelnen Bundles aufgerufen werden. Außerhalb der Iteration können im Modul E-Mail senden jedoch nur aggregierte Felder aufgerufen werden.

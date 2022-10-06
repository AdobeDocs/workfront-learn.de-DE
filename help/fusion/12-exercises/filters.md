---
title: Filter
description: Erfahren Sie, wie Sie den Filter zwischen Modulen verwenden, um nur bestimmte Typen von Bundles zuzulassen.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Filter

Erfahren Sie, wie Sie den Filter zwischen Modulen verwenden, um nur bestimmte Typen von Bundles zuzulassen.

## Übungsübersicht

Fügen Sie einen Filter zwischen den beiden Modulen im Szenario Über grundlegende Zuordnung hinzu, um nur Projekte mit einer roten Projektfarbe in der CSV-Datei zu erstellen.

![Filter Bild 1](../12-exercises/assets/filters-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Erstellen Sie einen Klon des Szenarios &quot;Über die grundlegende Zuordnung&quot;und nennen Sie ihn &quot;Verwenden des mächtigen Filters&quot;.

   **Fügen Sie vor dem Modul Workfront-Projekte erstellen einen Filter hinzu, damit nur rote Projekte erstellt werden können.**

   ![Filter Image 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Fügen Sie einen Filter hinzu, indem Sie auf die gepunktete Linie klicken, die die Module verbindet, oder auf den Schraubenschlüssel klicken und Filter einrichten auswählen.
1. Verwenden Sie das Feld Titel , um den Filter &quot;Nur rote Projekte&quot;zu benennen.
1. Mappen Sie im Feld Bedingung das Feld Projektfarbe (Spalte 3 in der CSV-Datei). Wählen Sie den Operator Gleich (nicht von Schreibweise abhängig) und geben Sie dann &quot;Rot&quot;ein.
1. Klicken Sie auf OK.

   ![Filter Image 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Testen Sie den Filter und überprüfen Sie die Ergebnisse.**

1. Klicken Sie auf Speichern , um das Szenario zu speichern, und dann auf einmal ausführen.
1. Klicken Sie auf den Ausführungsinspektor für den Filter, um zu sehen, wie jedes Bundle vom Filter geprüft wurde und entweder an das Modul Workfront-Projekte erstellen weitergeleitet wurde oder nicht weitergeleitet wurde.

   ![Filter Bild 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Suchen Sie die in Ihrer Workfront-Instanz erstellten Projekte.

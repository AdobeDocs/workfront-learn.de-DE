---
title: Übung zu Filtern
description: Erfahren Sie, wie Sie den Filter zwischen Modulen verwenden können, um nur bestimmte Typen von Bündeln durchzulassen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# Übung zu Filtern

Erfahren Sie, wie Sie den Filter zwischen Modulen verwenden können, um nur bestimmte Typen von Bündeln durchzulassen.

## Übungsübersicht

Fügen Sie einen Filter zwischen den beiden Modulen im Szenario „Über die grundlegende Zuordnung hinaus“ hinzu, um nur Projekte mit der Projektfarbe „Rot“ in der CSV-Datei zu erstellen.

![Filter – Bild 1](../12-exercises/assets/filters-walkthrough-1.png)

## Zu befolgende Schritte

1. Erstellen Sie einen Klon des Szenarios „Über die grundlegende Zuordnung hinaus“ und nennen Sie ihn „Den mächtigen Filter verwenden“.

   **Fügen Sie vor dem Modul „Workfront-Projekte erstellen“ einen Filter hinzu, damit nur rote Projekte erstellt werden können.**

   ![Filter – Bild 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Fügen Sie einen Filter hinzu, indem Sie auf die gepunktete Linie klicken, die die Module verbindet, oder klicken Sie auf den Schraubenschlüssel und wählen Sie „Filter einrichten“ aus.
1. Verwenden Sie das Feld „Bezeichnung“, um den Filter „Nur rote Projekte“ zu nennen.
1. Ordnen Sie im Feld „Bedingung“ das Feld „Projektfarbe“ (Spalte 3 in der CSV-Datei) zu. Wählen Sie den Operator „Gleich“ aus (nicht von Schreibweise abhängig) und geben Sie dann „Rot“ ein.
1. Klicken Sie auf „OK“.

   ![Filter – Bild 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Testen Sie den Filter und überprüfen Sie die Ergebnisse.**

1. Klicken Sie auf „Speichern“, um das Szenario zu speichern, und dann auf „Einmal ausführen“.
1. Klicken Sie auf den Ausführungsinspektor für den Filter, um zu sehen, wie jedes Bündel vom Filter geprüft wurde und entweder an das Modul „Workfront-Projekte erstellen“ weitergeleitet oder nicht weitergeleitet wurde.

   ![Filter – Bild 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Suchen Sie die Projekte, die in Ihrer Workfront-Instanz erstellt wurden.

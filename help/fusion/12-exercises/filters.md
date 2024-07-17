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
recommendations: noDisplay,noCatalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '229'
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

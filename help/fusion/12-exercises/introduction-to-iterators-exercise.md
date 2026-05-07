---
title: Einführung in die Iteratoren-Übung
description: Erfahren Sie, wie Sie Iterations-Apps verwenden und Aktionen für jedes Informationsbündel durchführen können.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,catalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:42:51.955Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 390
ht-degree: 100%

---

# Einführung in die Iteratoren-Übung

Erfahren Sie, wie Sie Iterations-Apps verwenden und Aktionen für jedes Informationsbündel durchführen können.

## Übungsübersicht

Sehen Sie sich ein bestimmtes Projekt in Workfront an und dann alle Aufgaben innerhalb dieses Projekts. Mit dem Inkrement-Tool-Modul zählen Sie die Anzahl der Aufgaben im Projekt. Schließlich verwenden Sie das Modul „Variable festlegen“, um die Anzahl der untergeordneten Elemente von der Anzahl der offenen Probleme zu subtrahieren und für jedes der Aufgabenbündel einen numerischen Wert zu generieren.

![Einführung in Iteratoren Bild 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Zu befolgende Schritte

**Ein Projekt und zugehörige Aufgaben lesen.**

1. Starten Sie ein neues Szenario. Nennen Sie es „Einführung in die Iteration“.
1. Wählen Sie Workfront als Trigger-Modul und lesen Sie einen Eintrag.
1. Wählen Sie für „Eintragstyp“ die Option „Projekt“.
1. Wählen Sie für Ausgaben „ID“, „Name“ und „Beschreibung“ aus.
1. Geben Sie im Feld „ID“ die Projekt-ID des Messestandprojekts für Northstar Fashion aus Ihrer Workfront-Testlaufwerkinstanz ein.
1. Benennen Sie dieses Modul in „WF-Projekte suchen“ um.
1. Fügen Sie ein weiteres Workfront-Modul hinzu, um die mit diesem Projekt verbundenen Aufgaben zu lesen. Wählen Sie das Modul „Zugehörige Einträge lesen“ aus.
1. Wählen Sie für „Eintragstyp“ die Option „Projekt“.
1. Wählen Sie für die übergeordnete Eintrags-ID die ID aus dem Modul „Eintrag lesen“ aus.
1. Wählen Sie für „Sammlungen“ die Option „Aufgaben“.
1. Wählen Sie für „Ausgaben“ „ID“, „Name“, „Beschreibung“, „Anzahl der untergeordneten Elemente“, „Anzahl offener Probleme“ und „Arbeit“ aus.
1. Benennen Sie dieses Modul in „Projektaufgaben lesen“ um.
1. Speichern Sie das Szenario und klicken Sie dann auf „Einmal ausführen“, um die Ausgaben anzuzeigen.

   + Wenn Sie auf den Ausführungsinspektor klicken, sehen Sie ein Bündel als Eingabe (das Projekt) und 28 Bündel als Ausgabe (die Aufgaben).

   **Iterierte Bündel zählen und verarbeiten.**

1. Fügen Sie nach „Zugehörige Einträge lesen“ ein weiteres Modul hinzu. Wählen Sie ein Inkrementierungsfunktions-Tool-Modul aus.

   + Belassen Sie das Feld „Wert zurücksetzen“ auf „Nie“ und klicken Sie auf „OK“.

1. Benennen Sie dieses Modul um in „Aufgaben zählen“.
1. Fügen Sie ein Modul „Variable festlegen“ hinzu. Setzen Sie den Variablennamen auf „Zufallsmathematik“.
1. Ziehen Sie im Feld „Variablenwert“ die Anzahl der offenen untergeordneten Elemente von der Anzahl der offenen Aufgaben ab.

   **Das sollte wie folgt aussehen:**

   ![Einführung in Iteratoren Bild 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Benennen Sie dieses Modul in „Zufallsmathematik“ um.
1. Speichern Sie das Szenario und klicken Sie auf „Einmal ausführen“.

Für jede der vom Iterator-Modul „Zugehörige Einträge lesen“ erzeugten Aufgaben führte Workfront Fusion 28 Ausführungen durch. Diese 28 Bündel werden während des gesamten Szenarios weiterhin verarbeitet, es sei denn, es wird ein Aggregator hinzugefügt, der den Kreislauf schließt.

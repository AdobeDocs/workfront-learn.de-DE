---
title: Erkunden von Läufen, Zyklen und Bundles
description: Erfahren Sie, wie sich Ausführungen, Zyklen und Bundles verhalten und den Ausführungsverlauf eines Szenarios nutzen.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11050
thumbnail: KT1101.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Erkunden von Läufen, Zyklen und Bundles

Erfahren Sie, wie sich Ausführungen, Zyklen und Bundles verhalten und den Ausführungsverlauf eines Szenarios nutzen.

## Übungsübersicht

Üben Sie mit verschiedenen Szenario-Konfigurationen, um mithilfe von Läufen und Zyklen zu untersuchen.

![Analyse von Ausführungszyklen und -paketen Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Klonen Sie das Szenario mit dem Namen &quot;Freigeben von Variablen zwischen Routing-Pfaden&quot;. Nennen Sie das neue Szenario &quot;Freigeben von Variablen zwischen Routing-Pfaden - Zyklustest&quot;.
1. Entfernen Sie das Modul E-Mail senden , da es für diesen Test nicht benötigt wird.

   **Richten Sie Ihr Szenario so ein, dass drei Zyklen pro Ausführung verarbeitet werden. Verarbeiten Sie 5 Projekte in jedem Zyklus.**

1. Klicken Sie auf das Trigger-Modul und ändern Sie das Feld Maximal in 5, sodass in jedem Zyklus nur fünf Projekte verarbeitet werden.
1. Entfernen Sie in den Suchkriterien den zweiten Filter, der die Suche auf ein einzelnes Projekt beschränkt.
1. Klicken Sie auf OK.

1. Öffnen Sie in der Fusion-Symbolleiste die Szenario-Einstellungen und ändern Sie das Feld Maximale Anzahl der Zyklen von 1 in 3.
1. Klicken Sie auf OK.

   ![Analyse von Ausführungszyklen und -paketen Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Planen Sie das Szenario so, dass es jede Minute ausgeführt wird.**

1. Klicken Sie auf das Uhrensymbol neben dem Trigger-Modul und ändern Sie das Feld &quot;Minutes&quot;in 1 Minute.

   ![Analyse von Ausführungszyklen und -paketen Bild 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Wechseln Sie dann unter der Schaltfläche Einmal ausführen den Umschalter Planung auf Ein . Speichern Sie Ihr Szenario.

   ![Analyse von Ausführungszyklen und -paketen Bild 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Wechseln Sie zum Ausführungsverlauf für das Szenario und sehen Sie sich an, wie in der nächsten Minute ein neuer Verlaufsdatensatz erscheint. Möglicherweise müssen Sie die Seite aktualisieren.

   ![Analyse von Ausführungszyklen und -paketen Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Klicken Sie auf die Schaltfläche Details eines Vorgangs. Klicken Sie im rechten Bereich durch das einfache Protokoll, ähnlich wie im Abschnitt zum Ausführungsverlauf der Workfront Fusion-Schulung.
1. Die Aufzeichnungen der verarbeiteten Vorgänge werden in Zyklen unterteilt.

   ![Analyse von Ausführungszyklen und Bundles Bild 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. In einem Dropdown-Menü oben rechts im Fenster können Sie einen der drei Zyklen auswählen, die Sie jedes Mal einrichten, um sie auszuführen.

   ![Analyse von Ausführungszyklen und Bundles Bild 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)

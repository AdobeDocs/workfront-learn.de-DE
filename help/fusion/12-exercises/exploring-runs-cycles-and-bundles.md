---
title: Übung zum Kennenlernen von Durchläufen, Zyklen und Bündeln
description: Erfahren Sie, wie sich Durchläufe, Zyklen und Bündel verhalten und den Ausführungsverlauf eines Szenarios nutzen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,noCatalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 100%

---

# Übung zum Kennenlernen von Durchläufen, Zyklen und Bündeln

Erfahren Sie, wie sich Durchläufe, Zyklen und Bündel verhalten und den Ausführungsverlauf eines Szenarios nutzen.

## Übungsübersicht

Üben Sie mit verschiedenen Szenariokonfigurationen, um die Verwendung von Durchläufen und Zyklen zu erkunden.

![Erkundung von Durchläufen, Zyklen und Bündeln Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Zu befolgende Schritte

1. Klonen Sie das Szenario mit dem Namen „Freigeben von Variablen zwischen Routing-Pfaden“. Nennen Sie das neue Szenario „Variablenfreigabe zwischen Routing-Pfaden – Zyklentest“.
1. Entfernen Sie das Modul „E-Mail senden“, da es für diesen Test nicht benötigt wird.

   **Richten Sie Ihr Szenario so ein, dass 3 Zyklen pro Durchlauf verarbeitet werden. Verarbeiten Sie 5 Projekte in jedem Zyklus.**

1. Klicken Sie auf das Trigger-Modul und ändern Sie das Feld „Maximal“ in 5, sodass in jedem Zyklus nur fünf Projekte verarbeitet werden.
1. Entfernen Sie in den Suchkriterien den zweiten Filter, der die Suche auf ein einzelnes Projekt beschränkt.
1. Klicken Sie auf „OK“.

1. Öffnen Sie in der Fusion-Symbolleiste die Szenario-Einstellungen und ändern Sie das Feld „Max. Anzahl von Zyklen“ von 1 in 3.
1. Klicken Sie auf „OK“.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Planen Sie das Szenario so, dass es jede Minute ausgeführt wird.**

1. Klicken Sie auf das Uhrensymbol neben dem Trigger-Modul und ändern Sie das Feld „Minuten“ in 1 Minute.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Stellen Sie dann den Schalter „Planung“ unter der Schaltfläche „Einmal ausführen“ auf „Ein“. Speichern Sie Ihr Szenario.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Rufen Sie den Ausführungsverlauf des Szenarios auf und schauen Sie, ob innerhalb der nächsten Minute ein neuer Verlaufseintrag erscheint. Möglicherweise müssen Sie die Seite aktualisieren.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Klicken Sie auf die Schaltfläche „Details“ eines Durchlaufs. Klicken Sie im rechten Bereich durch das einfache Protokoll, ähnlich wie im Abschnitt zum Ausführungsverlauf der Workfront Fusion-Schulung.
1. Die Einträge der verarbeiteten Vorgänge werden in Zyklen unterteilt.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. In einem Dropdown-Menü oben rechts im Fenster können Sie einen der drei eingerichteten Zyklen auswählen, um ihn jedes Mal auszuführen.

   ![Erkunden von Durchläufen, Zyklen und Bündeln Bild 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)

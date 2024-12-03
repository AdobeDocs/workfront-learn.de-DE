---
title: Arbeiten mit JSON-Übung
description: Erfahren Sie, wie Sie JSON-Dateien in einem Szenario erstellen und analysieren können, um Ihre Design-Anforderungen zu unterstützen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
recommendations: noDisplay,catalog
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 100%

---

# Arbeiten mit JSON-Übung

Erfahren Sie, wie Sie JSON-Dateien in einem Szenario erstellen und analysieren können, um Ihre Design-Anforderungen zu unterstützen.

## Übungsübersicht

Diese Übung soll konzeptionell aufzeigen, wie Informationen, die im JSON-Format an ein Szenario gesendet werden, genutzt werden können, indem sie in Felder und Elemente zerlegt werden, die Sie in Ihrem Szenario abbilden können. Anschließend können Sie Informationen aus diesen zugeordneten Arrays abrufen oder die Informationen in JSON aggregieren, um sie dann an ein anderes System zu senden, das JSON als Empfangseingabe erwartet.

![Arbeiten mit JSON Bild 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Zu befolgende Schritte

**Erstellen einer Datenstruktur und JSON-Analyse.**

1. Erstellen Sie ein neues Szenario und nennen Sie es „Arbeiten mit JSON-Donut-Daten“.
1. Verwenden Sie für das Trigger-Modul das Modul „Variable festlegen“.
1. Geben Sie für den Variablennamen „Donut-Daten“ ein.
1. Kopieren Sie für den Variablenwert den Inhalt des Dokuments „_Donut Data - Sample JSON.rtf“, das Sie im Ordner „Fusion Exercise Files“ auf Ihrem Testlaufwerk finden.

   ![Arbeiten mit JSON Bild 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Benennen Sie dieses Modul in „JSON von einem anderen Connector“ um.
1. Fügen Sie ein Modul „JSON-Analyse“ hinzu.
1. Klicken Sie im Feld „Datenstruktur“ auf „Hinzufügen“.
1. Wählen Sie den Generator aus und fügen Sie die Daten aus „Donut Data - Sample JSON“ ein, die Sie in das Feld „Beispieldaten“ kopiert haben.

   ![Arbeiten mit JSON Bild 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Klicken Sie auf „Speichern“ und nennen Sie die Datenstruktur „Donut-Daten“. Klicken Sie dann auf „Speichern“.
1. Ordnen Sie die Donut-Daten aus dem Modul „Variablen festlegen“ dem Feld „JSON-Zeichenfolge“ zu.

   ![Arbeiten mit JSON Bild 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Speichern Sie das Szenario und klicken Sie dann auf „Einmal ausführen“, um die Ausgabe anzuzeigen.

   **Die Ausgabe des Moduls „JSON-Analyse“ sollte wie folgt aussehen:**

   ![Arbeiten mit JSON Bild 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Zuordnung zu bestimmten Array-Variablen.**

1. Fügen Sie hinter dem Modul „JSON-Analyse“ einen Router hinzu.
1. Fügen Sie im obersten Pfad ein Modul „Variable festlegen“ hinzu.
1. Geben Sie als Variablennamen &quot;Batter-Typen nach Donut-Daten“ ein.
1. Verwenden Sie für den Variablenwert die Zuordnungsfunktion, um die Batter-Typen aus dem Batter-Array abzurufen.

   ![Arbeiten mit JSON Bild 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Klicken Sie auf „OK“ und dann auf „Einmal ausführen“.
1. Öffnen Sie den Ausführungsinspektor, um das Ausgabebündel und die Batter-Typen für jeden der drei Vorgänge anzuzeigen.

   ![Arbeiten mit JSON Bild 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Aggregieren der Szenario-Daten in JSON.**

1. Fügen Sie im unteren Routing-Pfad ein Modul „Zu JSON aggregieren“ hinzu.
1. Wählen Sie als Quellmodul den Iterator – das Modul „JSON-Analyse“.
1. Als Datenstruktur können Sie eine beliebige Datenstruktur anlegen oder auswählen. Verwenden Sie für dieses Beispiel Donut-Daten.
1. Ordnen Sie die Felder für dieses Beispiel direkt zu, wie unten dargestellt.
1. Beachten Sie bei Batter und Topping, dass es sich um Arrays handelt. Klicken Sie daher auf „Element hinzufügen“, um sie zuzuordnen.

   ![Arbeiten mit JSON Bild 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Speichern Sie das Szenario und klicken Sie auf „Einmal ausführen“.

Suchen Sie im Ausführungsinspektor nach dem Modul „Zu JSON aggregieren“ und prüfen Sie, ob Sie drei Bündel in einer einzigen JSON-Zeichenfolge zusammenfassen konnten. Sie können diese Zeichenfolge dann an andere Systeme senden, die JSON erwarten.

![Arbeiten mit JSON Bild 9](../12-exercises/assets/working-with-json-walkthrough-9.png)

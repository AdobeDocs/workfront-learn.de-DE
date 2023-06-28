---
title: Arbeiten mit JSON
description: Erfahren Sie, wie Sie JSON in einem Szenario erstellen und analysieren, um Ihre Designanforderungen zu unterstützen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Arbeiten mit JSON

Erfahren Sie, wie Sie JSON in einem Szenario erstellen und analysieren, um Ihre Designanforderungen zu unterstützen.

## Übungsübersicht

Ziel dieser Übung ist es, konzeptionell zu zeigen, wie die in ein Szenario gesendeten Informationen in einem JSON-Format verwendet und in Felder und Elemente analysiert werden, die Sie in Ihrem Szenario zuordnen können. Anschließend können Sie Informationen aus diesen zugeordneten Arrays abrufen oder die Informationen in JSON aggregieren, um sie dann an ein anderes System zu senden, das JSON als empfangende Eingabe erwartet.

![Arbeiten mit JSON Image 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

**Erstellen Sie eine Datenstruktur und analysieren Sie JSON.**

1. Erstellen Sie ein neues Szenario und nennen Sie es &quot;Arbeiten mit JSON-Ringdaten&quot;.
1. Verwenden Sie für das Trigger-Modul das Modul Variable festlegen .
1. Geben Sie für den Variablennamen &quot;Daten ablegen&quot;ein.
1. Kopieren Sie für den Variablenwert den Inhalt des Dokuments &quot;_Donut Data - Sample JSON.rtf&quot;, das Sie im Ordner Fusion Übungsdateien in Ihrem Testlaufwerk finden.

   ![Arbeiten mit JSON Image 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Benennen Sie dieses Modul &quot;JSON von einem anderen Connector&quot;um.
1. Fügen Sie ein JSON-Parse-Modul hinzu.
1. Klicken Sie im Feld Datenstruktur auf Hinzufügen .
1. Wählen Sie den Generator aus und fügen Sie die JSON-Beispieldaten Donut Data - Sample ein, die Sie in das Feld Beispieldaten kopiert haben.

   ![Arbeiten mit JSON Image 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Klicken Sie auf Speichern und benennen Sie die Datenstruktur &quot;Daten ablegen&quot;. Klicken Sie dann auf Speichern.
1. Ordnen Sie die Donut-Daten aus dem Set-Variablenmodul dem JSON-Zeichenfolgenfeld zu.

   ![Arbeiten mit JSON Image 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Speichern Sie das Szenario und klicken Sie dann auf Einmal ausführen , um die Ausgabe anzuzeigen.

   **Die Ausgabe des Parse-JSON-Moduls sollte wie folgt aussehen:**

   ![Arbeiten mit JSON Image 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Ordnen Sie bestimmten Array-Variablen zu.**

1. Fügen Sie nach dem JSON-Modul Parse einen Router hinzu.
1. Fügen Sie im obersten Pfad ein Set-Variablenmodul hinzu.
1. Geben Sie für den Variablennamen &quot;Batter types by donut&quot;ein.
1. Verwenden Sie für den Wert Variable die Funktion map , um die Stapeltypen aus dem Batter-Array abzurufen.

   ![Arbeiten mit JSON Image 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Klicken Sie auf OK und dann einmal ausführen.
1. Öffnen Sie den Ausführungsinspektor, um das Ausgabebundle für jeden der drei Vorgänge anzuzeigen und die Stapeltypen für jeden der drei Vorgänge anzuzeigen.

   ![Arbeiten mit JSON Image 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Aggregieren Sie die Szenario-Daten in JSON.**

1. Fügen Sie im unteren Routing-Pfad ein Aggregat zum JSON-Modul hinzu.
1. Wählen Sie für das Quellmodul den Iterator - das JSON-Modul &quot;Parse&quot;.
1. Erstellen oder wählen Sie für die Datenstruktur eine beliebige Datenstruktur. Verwenden Sie für dieses Beispiel Ringdaten.
1. Ordnen Sie die Felder für dieses Beispiel direkt zu, wie unten dargestellt.
1. Beachten Sie beim Aufstocken und Aufstocken, dass es sich um Arrays handelt. Klicken Sie daher auf Element hinzufügen , um sie zuzuordnen.

   ![Arbeiten mit JSON Image 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Speichern Sie das Szenario und klicken Sie einmal auf Ausführen .

Sehen Sie sich den Ausführungsinspektor für das Modul Aggregat zu JSON an und stellen Sie fest, wie Sie drei Bundles zu einer JSON-Zeichenfolge aggregieren konnten. Sie können diese Zeichenfolge dann an andere Systeme senden, die JSON erwarten.

![Arbeiten mit JSON Image 9](../12-exercises/assets/working-with-json-walkthrough-9.png)

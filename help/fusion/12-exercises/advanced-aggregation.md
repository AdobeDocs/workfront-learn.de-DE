---
title: Erweiterte Aggregation
description: Rufen Sie einen Web-Dienst zur Rückgabe von Details über mehrere Länder und zur Identifizierung der Bevölkerung, gruppiert nach Unterregionen, auf.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '481'
ht-degree: 100%

---

# Erweiterte Aggregation

Erfahren Sie, wie Sie beim Aggregieren Gruppierungen verwenden.

## Übungsübersicht

Rufen Sie einen Web-Dienst zur Rückgabe von Details über mehrere Länder und zur Ermittlung der Gesamtbevölkerung aller Länder, gruppiert nach Unterregionen, auf.

![Erweiterte Aggregation Bild 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Zu befolgende Schritte

**Rufen Sie die Länderdetails ab.**

![Erweiterte Aggregation Bild 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Erstellen Sie ein neues Szenario und nennen Sie es „Erweiterte Aggregation“.
1. Setzen Sie das Trigger-Modul auf ein „Anfrage stellen“-HTTP-Modul.
1. Unter dieser URL, `https://restcountries.com/v2/lang/es`, finden Sie eine Liste aller Länder, in denen Spanisch gesprochen wird.
1. Belassen Sie die Methode auf Get.
1. Klicken Sie auf das Kontrollkästchen „Antwort auswerten“.
1. Benennen Sie dieses Modul in „Länder abrufen“ um.
1. Klicken Sie auf „Speichern und einmal ausführen“.

   **Die Ausgabe ist ein einzelnes Paket, aber es wird in einem Array mit 24 Sammlungen geliefert, einer für jedes spanischsprachige Land.**

   ![Erweiterte Aggregation Bild 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **Sie müssen für jedes Land Informationen über die Unterregionen sammeln, also müssen Sie eine zusätzliche HTTP-Anfrage stellen.**

1. Fügen Sie eine weitere Anfrage hinzu, um Informationen über Teilregionen zu erhalten. Es wird nur das erste Land zurückgegeben, aber das ist vorerst in Ordnung. Fügen Sie ein weiteres „Anfrage stellen“-HTTP-Modul hinzu und verwenden Sie die URL `https://restcountries.com/v2/name/{country name}`.
1. Um den Namen des ersten Landes abzurufen, klicken Sie im Zuordnungsbedienfeld auf „Daten“ und dann im Array auf „Name“. Die [1] im Datenfeld bedeutet, dass das erste Element im Array zurückgegeben wird.

   + Klicken Sie auf die Nummer und ändern Sie bei Bedarf den Index, aber in diesem Fall wollen Sie nur das erste Element.

![Erweiterte Aggregation Bild 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Markieren Sie „Antwort auswerten“ im Zuordnungsbedienfeld und klicken Sie dann auf „OK“.
1. Benennen Sie es in „Länderdetails abrufen“ um.
1. Klicken Sie auf „Speichern“ und dann auf „Einmal ausführen“.

   + Die Ausgabe besteht aus Informationen für ein einzelnes Land.

1. Um die anderen Länder zu erhalten, müssen Sie durch das Array iterieren. Fügen Sie einen Iterator hinzu, der eine Liste von Dingen nimmt und für jedes Element auf der Liste ein Bündel ausgibt.

   **Fügen Sie den Iterator und den Aggregator hinzu.**

1. Klicken Sie mit der rechten Maustaste zwischen die HTTP-Module und fügen Sie das Modul „Iterator-Flow-Kontrolle“ hinzu.
1. Wählen Sie im Array-Feld Daten aus dem Modul „Länder abrufen“.

   ![Erweiterte Aggregation Bild 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. Aktualisieren Sie im Modul „Länderdetails abrufen“ das URL-Feld, um das Namensfeld aus dem Iterator anstatt aus dem Modul „Länder abrufen“ zu übernehmen.

   ![Erweiterte Aggregation Bild 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Fügen Sie nun nach „Länderdetails abrufen“ einen numerischen Aggregator hinzu, um die Populationen zu gruppieren und zu summieren.
1. Das Quellmodul ist das Iteratormodul.
1. Die Aggregatfunktion ist SUM.
1. Der Wert ist [data:population] aus dem Modul „Länderdetails abrufen“.
1. Klicken Sie unten auf die Option „Erweiterte Einstellungen anzeigen“ und gruppieren Sie nach [data:subregion] aus dem Modul „Länderdetails abrufen“.

   ![Erweiterte Aggregation Bild 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Schließen Sie mit einem Text-Aggregator ab, um die im numerischen Aggregator gruppierten Elemente zu aggregieren.**

1. Fügen Sie am Ende einen Text-Aggregator hinzu.
1. Das Quellmodul ist der numerische Aggregator.
1. Fügen Sie im Textbereich ein: „Die Gesamtbevölkerung von [KEY] ist [result].“

   ![Erweiterte Aggregation Bild 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Speichern Sie und führen Sie einmal aus.

   + Überprüfen Sie die Ergebnisse des letzten Moduls.

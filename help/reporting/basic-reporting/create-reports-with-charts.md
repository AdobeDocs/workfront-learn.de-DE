---
title: Erstellen von Berichten mit Diagrammen
description: Lernen Sie, wie Diagramme die Visualisierung von Daten verbessern können und wie Diagramm-Tools in Workfront verwendet werden.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: ht
source-wordcount: '334'
ht-degree: 100%

---

# Erstellen von Berichten mit Diagrammen

In diesem Video lernen Sie Folgendes:

* Wie Diagramme die Visualisierung von Daten verbessern können
* Wie die Diagramm-Tools von Workfront verwendet werden

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Aktivitäten zum Erstellen von Berichten mit Diagrammen

### Aktivität 1: Hinzufügen eines Diagramms zu einem Bericht

Das Quartalsende naht, und Sie möchten sehen, inwieweit die kürzlich abgeschlossenen Projekte ihr Budget eingehalten haben. Erstellen Sie einen Bericht, der die geplanten Kosten im Vergleich zu den tatsächlichen Kosten für Projekte zeigt. Sie möchten nur die Projekte sehen, die im letzten Quartal abgeschlossen wurden. Fügen Sie ein Diagramm mit einer Kombination von Spalten hinzu, das benutzerdefinierte Farben verwendet.

### Antwort 1

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf das Menü **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Projekt]** aus.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Spalten (Ansicht)]** und dann auf **[!UICONTROL Spalte hinzufügen]**.
1. Wählen Sie [!UICONTROL Projekt] > [!UICONTROL Geplante Kosten] aus und fassen Sie diese Spalte mit **[!UICONTROL Summieren]** zusammen.
1. Klicken Sie erneut auf **[!UICONTROL Spalte hinzufügen]**.
1. Wählen Sie [!UICONTROL Projekt] > [!UICONTROL Tatsächliche Kosten] aus und fassen Sie diese Spalte mit **[!UICONTROL Summieren]** zusammen.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Spalten zu einem Bericht](assets/chart-report-columns.png)

1. Legen Sie auf der Registerkarte **[!UICONTROL Gruppierungen]** fest, dass der Bericht nach [!UICONTROL Projekt] > [!UICONTROL Name] gruppiert werden soll.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Gruppierungen zu einem Bericht](assets/chart-report-groupings.png)

1. Fügen Sie auf der Registerkarte **[!UICONTROL Filter]** zwei Filterregeln hinzu:

   * [!UICONTROL Projekt] > [!UICONTROL Status entspricht] > [!UICONTROL Abgeschlossen]
   * [!UICONTROL Projekt] > [!UICONTROL Tatsächliches Abschlussdatum] > [!UICONTROL Letztes Quartal]

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Filtern zu einem Bericht](assets/chart-report-filters.png)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Diagramm]** die Option **[!UICONTROL Spalte]** für den Diagrammtyp aus.
1. Wählen Sie für die [!UICONTROL linke Achse (Y)] [!UICONTROL Projekt] > [!UICONTROL Geplante Kosten].
1. Wählen Sie für die [!UICONTROL untere Achse (X)] [!UICONTROL Projekt] > [!UICONTROL Name].
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Kombinationsdiagramm]** und wählen Sie [!UICONTROL Projekt] > [!UICONTROL Tatsächliche Kosten] im Feld **[!UICONTROL Wert]** aus.
1. Klicken Sie auf den Pfeil neben dem Farbfeld, um die Farbe der [!UICONTROL tatsächlichen Kosten] zu ändern. Wählen Sie eine der angezeigten Farben aus oder klicken Sie auf das Feld unten rechts, um die Farbpalette aufzurufen.
1. Klicken Sie auf **[!UICONTROL Speichern + schließen]**. Wenn Sie zur Eingabe eines Berichtnamens aufgefordert werden, nennen Sie ihn „Geplante vs. tatsächliche Kosten nach abgeschlossenem Projekt im letzten Quartal“.

   ![Ein Screenshot des Bildschirms zum Hinzufügen eines Diagramms zu einem Bericht](assets/chart-report-chart.png)

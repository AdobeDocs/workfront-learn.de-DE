---
title: Erstellen von Berichten mit Diagrammaktivitäten
description: Üben Sie das Erstellen von Berichten mit Diagrammen mit schrittweisen Anweisungen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# Erstellen von Berichten mit Diagrammaktivitäten

Üben Sie das Erstellen von Berichten mit Diagrammen mit schrittweisen Anweisungen.

## Aktivität 1: Hinzufügen eines Diagramms zu einem Bericht

Das Quartalsende naht, und Sie möchten sehen, inwieweit die kürzlich abgeschlossenen Projekte ihr Budget eingehalten haben. Erstellen Sie einen Bericht, der die geplanten Kosten im Vergleich zu den tatsächlichen Kosten für Projekte zeigt. Sie möchten nur die Projekte sehen, die im letzten Quartal abgeschlossen wurden. Fügen Sie ein Diagramm mit einer Kombination von Spalten hinzu, das benutzerdefinierte Farben verwendet.

## Antwort 1

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
1. Klicken Sie auf **[!UICONTROL Speichern + schließen]**. Wenn Sie nach einem Berichtsnamen gefragt werden, nennen Sie ihn „Geplante Kosten im Vgl. zu Istkosten nach Projekt abgeschlossen im letzten Quartal“.

   ![Ein Screenshot des Bildschirms zum Hinzufügen eines Diagramms zu einem Bericht](assets/chart-report-chart.png)

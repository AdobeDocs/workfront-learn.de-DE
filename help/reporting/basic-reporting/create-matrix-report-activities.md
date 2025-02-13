---
title: Erstellen von Matrixberichtsaktivitäten
description: Üben Sie die Erstellung von Matrixberichten mit schrittweisen Anweisungen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 66%

---

# Erstellen von Matrixberichtsaktivitäten

Üben Sie die Erstellung von Matrixberichten mit schrittweisen Anweisungen.

## Aktivität 1: Erstellen eines Matrixberichts

Erstellen Sie einen Matrix-Bericht, aus dem hervorgeht, wie viele Anfragen in jedem Status vorhanden sind, sortiert nach Anfrage-Warteschlange. Dies gibt Ihnen einen schnellen Überblick über den Arbeitsaufwand, der eingeht, und wie gut Sie damit Schritt halten.

Sie möchten, dass die Anfrage-Warteschlangen in den Zeilengruppierungen erscheinen. Der Status erscheint als die Spaltengruppierungen. Geben Sie dem Bericht den Namen „Anfragen nach Status und Anfrage-Warteschlange“.

## Antwort 1

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf die Option **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Problem]** aus.
1. Navigieren Sie zur Registerkarte **[!UICONTROL Gruppierungen]** und klicken Sie auf **[!UICONTROL Zu Matrix-Gruppierung wechseln]**.
1. Wählen Sie für [!UICONTROL Zeilengruppierungen] die Option **[!UICONTROL Projekt]** > **[!UICONTROL Name]** aus.
1. Wählen Sie für [!UICONTROL Spaltengruppierung] die Option **[!UICONTROL Problem]** > **[!UICONTROL Status]** aus.

   ![Ein Screenshot des Bildschirms zur Erstellung einer neuen Problembericht-Gruppierung](assets/matrix-report-groupings.png)

1. Wechseln Sie zur Registerkarte **[!UICONTROL Filter]**.
1. Um sicherzustellen, dass nur Anfragen in aktiven Anfrage-Warteschlangen angezeigt werden, fügen Sie die folgenden Filterregeln hinzu:

   * [!UICONTROL Projekt] > [!UICONTROL Status entspricht] > [!UICONTROL Gleich] > [!UICONTROL Aktuell]
   * [!UICONTROL Warteschlangendefinition] > [!UICONTROL Ist öffentlich] > [!UICONTROL Ungleich] > [!UICONTROL Keines] (So wissen wir, dass ein Projekt tatsächlich eine Anfrage-Warteschlange ist, indem die Warteschlangendefinition einer der öffentlichen Optionen zugewiesen wird.)

1. Klicken Sie auf **[!UICONTROL Speichern + schließen]**. Geben Sie bei Aufforderung zur Eingabe eines Berichtsnamens „Anfragen nach Status und Anfrage-Warteschlange“ ein.

   ![Ein Screenshot des Bildschirms zur Erstellung eines neuen Problembericht-Filters](assets/matrix-report-filters.png)

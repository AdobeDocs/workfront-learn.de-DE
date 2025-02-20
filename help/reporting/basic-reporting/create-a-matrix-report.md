---
title: Erstellen eines Matrix-Berichts
description: Erfahren Sie, wann ein Matrix-Bericht nützlich sein kann und wie Sie einen Matrix-Bericht in Workfront erstellen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: ht
source-wordcount: '268'
ht-degree: 100%

---

# Erstellen eines Matrix-Berichts

In diesem Video lernen Sie Folgendes:

* Wann ein Matrix-Bericht nützlich sein kann
* Und wie man einen Matrix-Bericht erstellt

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## Aktivitäten zum Erstellen eines Matrix-Berichts

Klicken Sie [hier](/help/assets/create-matrix-report-activities.pdf), um eine PDF-Datei dieser Seite herunterzuladen.

### Aktivität 1: Erstellen eines Matrix-Berichts

Erstellen Sie einen Matrix-Bericht, aus dem hervorgeht, wie viele Anfragen in jedem Status vorhanden sind, sortiert nach Anfrage-Warteschlange. Dies gibt Ihnen einen schnellen Überblick über die eingehende Arbeit und darüber, wie gut Sie mit ihr Schritt halten.

Sie möchten, dass die Anfrage-Warteschlangen in den Zeilengruppierungen erscheinen. Der Status erscheint als die Spaltengruppierungen. Nennen Sie den Bericht „Anfragen nach Status und Anfrage-Warteschlange“.

### Antwort 1

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

1. Klicken Sie auf **[!UICONTROL Speichern + schließen]**. Wenn Sie zur Eingabe eines Berichtnamens aufgefordert werden, geben Sie „Anfragen nach Status und Anfrage-Warteschlange“ ein.

   ![Ein Screenshot des Bildschirms zur Erstellung eines neuen Problembericht-Filters](assets/matrix-report-filters.png)

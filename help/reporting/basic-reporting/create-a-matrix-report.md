---
title: Erstellen eines Matrix-Berichts
description: In diesem Video erfahren Sie, wann ein Matrix-Bericht nützlich sein kann und wie Sie einen Matrix-Bericht in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
source-git-commit: f4000878d453c58fabf34308a8e3ab31d9667a1f
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Erstellen eines Matrix-Berichts

In diesem Video erfahren Sie:

* Wann ein Matrix-Bericht nützlich sein kann
* Und wie man einen Matrix-Bericht erstellt

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Aktivität: Erstellen eines Matrix-Berichts

Erstellen Sie einen Matrix-Bericht, der anzeigt, wie viele Anforderungen es in jedem Status gibt, sortiert nach Anforderungswarteschlange. Dies gibt Ihnen einen schnellen Überblick über die Arbeit, die eingeht und wie gut Sie damit Schritt halten.

Sie möchten, dass die Anforderungswarteschlangen in den Zeilengruppierungen angezeigt werden. Status wird als Spaltengruppierungen angezeigt. Benennen Sie Ihren Bericht &quot;Anforderungen nach Status und Anforderungswarteschlange&quot;.

## Antwort

1. Auswählen **[!UICONTROL Berichte]** von **[!UICONTROL Hauptmenü]**.
1. Klicken Sie auf **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Problem]**.
1. Navigieren Sie zu **[!UICONTROL Gruppierungen]** Registerkarte und klicken Sie auf **[!UICONTROL Zur Matrix-Gruppierung wechseln]**.
1. Für [!UICONTROL Zeilengruppierungen]auswählen **[!UICONTROL Projekt]** > **[!UICONTROL Name]**.
1. Für [!UICONTROL Spaltengruppierung]auswählen **[!UICONTROL Problem]** > **[!UICONTROL Status]**.

   ![Ein Bild des Bildschirms, um einen neuen Bericht zu Problemen zu erstellen](assets/matrix-report-groupings.png)

1. Navigieren Sie zu **[!UICONTROL Filter]** Registerkarte.
1. Um sicherzustellen, dass nur Anforderungen in aktiven Anforderungswarteschlangen angezeigt werden, fügen Sie die folgenden Filterregeln hinzu:

   * [!UICONTROL Projekt] > [!UICONTROL Status entspricht] > [!UICONTROL Gleich] > [!UICONTROL Aktuell]
   * [!UICONTROL Warteschlangendefinition] > [!UICONTROL Ist öffentlich] > [!UICONTROL Ungleich] > [!UICONTROL Keines] (So wissen wir, dass ein Projekt tatsächlich eine Anforderungswarteschlange ist, indem die Warteschlangendefinition einer der öffentlichen Optionen zugewiesen wird.)

1. Klicken Sie auf **[!UICONTROL Speichern und schließen]**. Wenn Sie zur Eingabe eines Berichtsnamens aufgefordert werden, geben Sie &quot;Anforderungen nach Status und Anforderungswarteschlange&quot;ein.

   ![Ein Bild des Bildschirms, um einen neuen Filter für Problemberichte zu erstellen](assets/matrix-report-filters.png)

---
title: Basisfilteraktivitäten erstellen
description: In dieser Aktivität erstellen Sie einen Projektfilter mit dem Namen "Projekte, die in diesem Monat abgeschlossen werden".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0c822b5be5272c5b638039d83294b00d25c32141
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Basisfilteraktivitäten erstellen

## Aktivität 1 - Alle Projekte im Marketingportfolio

In dieser Aktivität erstellen Sie einen Projektfilter mit dem Namen &quot;Alle Projekte im Marketing-Portfolio&quot;im [!UICONTROL Veralteter Filter] Erlebnis. Dadurch werden alle Projekte im Portfolio mit dem Namen &quot;Marketing Portfolio&quot;unabhängig von ihrem Status angezeigt.

Nachfolgend finden Sie eine schrittweise Anleitung.

### Antwort auf Aktivität 1

![Ein Bild des Bildschirms zum Erstellen eines neuen Filters](assets/basic-filter-activity-1.png)

1. Navigieren Sie zum [!UICONTROL Projekte] Bereich von [!UICONTROL Hauptmenü]. Hier sehen Sie eine Liste der Projekte.
1. Klicken Sie auf **[!UICONTROL Filter]** Menü und wählen Sie [!UICONTROL Alte Filter]
1. Auswählen **[!UICONTROL Neuer Filter]**.
1. Benennen Sie Ihren Filter &quot;Alle Projekte im Marketing-Portfolio&quot;.
1. Klicks **[!UICONTROL Filterregel hinzufügen]**.
1. Im [!UICONTROL Eingabe des Feldnamens beginnen] Feld, Typ[!UICONTROL Portfolioname]&quot;. Wählen Sie anschließend [!UICONTROL Name] unter [!UICONTROL Portfolio] -Feldquelle.
1. Lassen Sie die [!UICONTROL Gleich] verwendet.
1. Typ &quot;[!UICONTROL Marketing]&quot; in der [!UICONTROL Eingabe des Namens beginnen] -Feld.
1. Auswählen [!UICONTROL Marketing-Portfolio] vorausgesetzt, Sie verfügen über ein Portfolio mit diesem Namen, nach dem Sie filtern möchten. Wenn Sie nicht einfach die type ahead-Funktion verwenden, um das gewünschte Portfolio zu finden.
1. Klicks **[!UICONTROL Filter speichern]**

## Aktivität 2 - Projekte, deren Inhaber ich bin, schließen diesen Monat

In diesem Video erstellen Sie einen Projektfilter mit dem Namen &quot;Projekte, deren Inhaber ich bin, schließen diesen Monat&quot;im [!UICONTROL Veralteter Filter] Erlebnis. Wenn Sie viele Projekte im Auge behalten, kann dieser Filter Ihnen helfen, die zu schließenden Projekte heranzuzoomen.

Nachfolgend finden Sie eine schrittweise Anleitung.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### Antwort auf Aktivität 2

![Ein Bild des Bildschirms zum Erstellen eines neuen Filters](assets/basic-filter-activity-updated-6-15-21.png)

1. Navigieren Sie zum [!UICONTROL Projekte] Bereich von [!UICONTROL Hauptmenü]. Hier sehen Sie eine Liste der Projekte.
1. Klicken Sie auf **[!UICONTROL Filter]** Menü und wählen Sie [!UICONTROL Alte Filter]
1. Auswählen **[!UICONTROL Neuer Filter]**.
1. Nennen Sie Ihren Filter &quot;Projekte, deren Inhaber ich bin, schließen diesen Monat&quot;.
1. Klicks **[!UICONTROL Filterregel hinzufügen]**.
1. Im [!UICONTROL Eingabe des Feldnamens beginnen] -Feld, geben Sie &quot;owner&quot;ein. Wählen Sie anschließend [!UICONTROL Eigentümer-ID] unter [!UICONTROL Projekt] -Feldquelle.
1. Lassen Sie die [!UICONTROL Gleich] verwendet.
1. Geben Sie &quot;$$&quot;in das Feld [!UICONTROL Eingabe des Namens beginnen] -Feld.
1. Auswählen [!UICONTROL $$USER.ID]. Dies ist der Platzhalter für den angemeldeten Benutzer.
1. Klicks [!UICONTROL Filterregel hinzufügen] erneut.
1. Im [!UICONTROL Eingabe des Feldnamens beginnen] eingeben, beginnen Sie mit der Eingabe &quot;Ist abgeschlossen&quot;. Wählen Sie anschließend [!UICONTROL Ist abgeschlossen] unter der Quelle des Projektfelds.
1. Lassen Sie die [!UICONTROL Gleich] verwendet.
1. Wählen Sie &quot;False&quot;.
1. Klicks [!UICONTROL Filterregel hinzufügen] erneut.
1. Im [!UICONTROL Eingabe des Feldnamens beginnen] Feldtyp &quot;Geplant&quot;, dann auswählen [!UICONTROL Geplantes Abschlussdatum] unter [!UICONTROL Projekt] -Feldquelle.
1. Ändern Sie die [!UICONTROL Gleich] Operator zu [!UICONTROL Diesen Monat].
1. Klicks **[!UICONTROL Filter speichern]**

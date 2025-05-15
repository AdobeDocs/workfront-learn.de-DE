---
title: Erstellen einer einfachen Filteraktivität
description: In dieser Aktivität erstellen Sie einen Projektfilter mit dem Namen „Alle Projekte im Marketing-Portfolio“ und einen weiteren Projektfilter mit dem Namen „In diesem Monat abgeschlossene Projekte in meinem Besitz“.
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
last-substantial-update: 2025-05-15T00:00:00Z
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0755d62240ab307d3759c47c4561264cb4baadab
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 64%

---

# Erstellen einer einfachen Filteraktivität


## Aktivität 1 – Alle Projekte im Marketing-Portfolio

In dieser Aktivität erstellen Sie einen Projektfilter mit dem Namen „Alle Projekte im Marketing-Portfolio“ im [!UICONTROL alten Filtererlebnis]. Dadurch werden alle Projekte im Portfolio mit dem Namen „Marketing Portfolio“ unabhängig von ihrem Status angezeigt.

Eine schrittweise Anleitung finden Sie weiter unten.

## Antwort auf Aktivität 1

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters](assets/basic-filter-activity-1.png)

1. Navigieren Sie vom [!UICONTROL Hauptmenü] zum Bereich [!UICONTROL Projekte]. Dort sehen Sie eine Liste der Projekte.
1. Klicken Sie auf **[!UICONTROL Filter]** Menü und wählen Sie [!UICONTROL Legacy-Filter] aus, falls diese nicht bereits ausgewählt ist.
1. Wählen Sie **[!UICONTROL Neuer Filter]** aus.
1. Nennen Sie Ihren Filter „Alle Projekte im Marketing-Portfolio“.
1. Klicken Sie auf **[!UICONTROL Filterregel hinzufügen]**.
1. Klicken Sie auf **Feld „Feld auswählen** und geben Sie die Wörter &quot;[!UICONTROL Portfolioname] ein. Wählen Sie dann[!UICONTROL Name] unter der Feldquelle [!UICONTROL Portfolio] aus.
1. Belassen Sie den Operator [!UICONTROL Gleich] so, wie er ist.
1. Geben Sie [!UICONTROL &#x200B; Suchfeld &quot;]&quot; ein.
1. Wählen Sie [!UICONTROL Marketing-Portfolio] aus, vorausgesetzt, Sie verfügen über ein Portfolio mit dem Namen, nach dem Sie filtern möchten. Wenn nicht, nutzen Sie einfach die Funktion zum automatischen Vervollständigen, um das gewünschte Portfolio zu finden.
1. Klicken Sie auf **[!UICONTROL Filter speichern]**.

## Aktivität 2 – Projekte, für die ich verantwortlich bin, die in diesem Monat abgeschlossen werden

In diesem Video erstellen Sie einen Projektfilter mit dem Namen „Projekte, für die ich verantwortlich bin, die in diesem Monat abgeschlossen werden“ im [!UICONTROL alten Filtererlebnis]. Wenn Sie viele Projekte im Auge behalten, können Sie mit diesem Filter die Projekte herausfiltern, die in Kürze abgeschlossen werden sollen.

Eine schrittweise Anleitung finden Sie weiter unten.

>[!VIDEO](https://video.tv.adobe.com/v/3443388/?quality=12&learn=on&enablevpops&captions=ger)

## Antwort auf Aktivität 2

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters](assets/basic-filter-activity-2.png)

1. Navigieren Sie vom [!UICONTROL Hauptmenü] zum Bereich [!UICONTROL Projekte]. Dort sehen Sie eine Liste der Projekte.
1. Klicken Sie auf **[!UICONTROL Filter]** Menü und wählen Sie [!UICONTROL Legacy-Filter] aus, falls diese nicht bereits ausgewählt ist.
1. Wählen Sie **[!UICONTROL Neuer Filter]** aus.
1. Nennen Sie Ihren Filter „Projekte, für die ich verantwortlich bin, die in diesem Monat abgeschlossen werden“.
1. Klicken Sie auf **[!UICONTROL Filterregel hinzufügen]**.
1. Klicken Sie auf das **Feld „Feld auswählen** und beginnen Sie, das Wort „Inhaber“ einzugeben. Klicken Sie nun unter der Feldquelle [!UICONTROL Projekt] auf Inhaber-ID .
1. Belassen Sie den Operator [!UICONTROL Gleich] so, wie er ist.
1. Geben Sie &quot;$$&quot; in das Suchfeld ein.
1. Wählen Sie [!UICONTROL $$USER.ID]. Dies ist der Platzhalter für die angemeldeten Benutzenden.
1. Klicken Sie auf Weitere Filterregel hinzufügen .
1. Klicken Sie auf **Feld „Feld auswählen** und geben Sie das Wort „Ist abgeschlossen“ ein. Klicken Sie nun unter der Feldquelle [!UICONTROL Projekt] auf „Ist abgeschlossen“.
1. Belassen Sie den Operator [!UICONTROL Gleich] so, wie er ist.
1. Wählen Sie „False“ aus.
1. Klicken Sie erneut auf Weitere Filterregel hinzufügen .
1. Klicken Sie auf **Feld „Feld auswählen** und geben Sie das Wort „Geplant“ ein. Klicken Sie nun auf „Geplantes Abschlussdatum“ unter der [!UICONTROL Projekt] Feldquelle.
1. Ändern Sie den Operator [!UICONTROL Gleich] zu [!UICONTROL Dieser Monat].
1. Klicken Sie auf **[!UICONTROL Filter speichern]**.

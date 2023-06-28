---
title: Leistungsmetriken verstehen
description: Erfahren Sie, wie Sie die Leistungsmetriken verwenden - die [!UICONTROL Leistungsindex-Methode] ([!UICONTROL PIM]) und der [!UICONTROL Schätzen bei Abschluss] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Leistungsmetriken verstehen

Zu den zwei Leistungsmetriken, die von Projektmanagern verwendet werden, gehören die [!UICONTROL Leistungsindex-Methode] ([!UICONTROL PIM]) und der [!UICONTROL Schätzen bei Abschluss] ([!UICONTROL EAC]). Systemweite Standardwerte können in [!DNL Workfront] und gelten für neu erstellte Projekte. [!UICONTROL PIM] kann dann für einzelne Projekte geändert werden.

**[!UICONTROL PIM]**

Die Einstellungen für [!UICONTROL PIM] steuern, wie [!DNL Workfront] berechnet andere Projektleistungsmetriken wie die [!UICONTROL Kostenleistungs-Index] ([!UICONTROL CPI]), [!UICONTROL Performance-Index des Kostenplans] ([!UICONTROL CSI]), [!UICONTROL Performance-Index planen] ([!UICONTROL SPI]) und [!UICONTROL Schätzen bei Abschluss] ([!UICONTROL EAC]).

Optionen für [!UICONTROL PIM] sind stundenbasiert und kostenbasiert.

* **Stundenbasiert** — Workfront verwendet die geplanten Arbeitsstunden zur Berechnung des CPI und des EAC des Projekts. Die EAC des Projekts wird als Zahl in Stunden angezeigt.
* **Kostenbasiert** — Workfront verwendet die geplanten Arbeitskosten zur Berechnung des CPI und des EAC des Projekts. EAC wird als Währungswert angezeigt. Stellen Sie bei Verwendung dieser Option sicher, dass Aufgabenverantwortliche (Benutzer und/oder Aufgabenrollen) Kostensätzen zugeordnet sind.

**[!UICONTROL EAC]**

[!UICONTROL EAC] stellt die voraussichtlichen Gesamtkosten Ihrer Aufgabe oder des Projekts nach Abschluss dar. Optionen werden auf Projektebene berechnet und von Aufgaben/Unteraufgaben aggregiert.

* **Auf Projektebene berechnen** — [!UICONTROL EAC] für die übergeordnete Aufgabe und das Projekt anhand der tatsächlichen Stunden/tatsächlichen Arbeitskosten in [!UICONTROL EAC] Formeln bezeichnet. Die Berechnung umfasst die tatsächlichen Stunden/Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.
* R **Aus Aufgaben/Unteraufgaben holen** — [!UICONTROL EAC] für die übergeordnete Aufgabe und das übergeordnete Projekt durch Addieren der [!UICONTROL EAC] für jede untergeordnete Aufgabe. Diese Berechnung schließt tatsächliche Stunden/Kosten aus, die direkt zu einer übergeordneten Aufgabe oder einem übergeordneten Projekt hinzugefügt werden.

Die [!UICONTROL EAC] Berechnungen werden in [Schätzung nach Abschluss berechnen (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Leistungsmetriken: Einstellungen**

Zum Festlegen [!UICONTROL PIM] und [!UICONTROL EAC] Systemstandardwerte:

1. Auswählen **[!UICONTROL Einrichtung]** aus dem Hauptmenü.
1. Klicken **[!UICONTROL Projektvoreinstellungen]** Klicken Sie im Menü des linken Bedienfelds auf **[!UICONTROL Projekte]**
1. Im [!UICONTROL Projektstatus] finden Sie [!UICONTROL Leistungsindex-Methode]. Wählen Sie Stunden- oder Kostenbasiert aus.
1. Für [!UICONTROL Schätzen bei Abschluss], wählen Sie auf Projektebene berechnen oder Aus Aufgaben/Unteraufgaben aggregieren aus.
1. Klicken **[!UICONTROL Speichern]** unten im Fenster.

![Ein Bild der [!UICONTROL Projektvoreinstellungen] Bildschirm](assets/setting-up-finances-1.png)

**Satz [!UICONTROL PIM] zu einzelnen Projekten**

1. Rufen Sie die Landingpage eines Projekts auf.
1. Klicken **[!UICONTROL Projektdetails]** aus dem linken Bereich.
1. Öffnen Sie die **[!UICONTROL Finanzen]** Abschnitt.
1. Doppelklicken Sie auf den Text unten **[!UICONTROL Leistungsindex-Methode]** , um sie zu bearbeiten.
1. Wählen Sie Stunden- oder Kostenbasiert aus.
1. Klicken **[!UICONTROL Speichern]** Änderungen an der Fertigstellung.

![Ein Bild der [!UICONTROL Projektdetails] Bildschirm](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kann für eine Projektvorlage im [!UICONTROL Finanzen] -Abschnitt der Vorlagendetails.

---
title: Verstehen von Leistungsmetriken
description: Erfahren Sie, wie Sie die Leistungsmetriken verwenden – die [!UICONTROL Performance-Index-Methode] ([!UICONTROL PIM]) und [!UICONTROL Schätzung bei Abschluss] ([!UICONTROL EAC]).
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
source-wordcount: '423'
ht-degree: 100%

---

# Verstehen von Leistungsmetriken

Zu den zwei Leistungsmetriken, die von Projekt-Managerinnen und -Managern verwendet werden, gehören die [!UICONTROL Performance-Index-Methode] ([!UICONTROL PIM]) und die [!UICONTROL Schätzung bei Abschluss] ([!UICONTROL EAC]). Systemweite Standardwerte können in [!DNL Workfront] festgelegt werden und gelten für neu erstellte Projekte. Die [!UICONTROL PIM] kann dann für einzelne Projekte geändert werden.

**[!UICONTROL PIM]**

Die Einstellungen für die [!UICONTROL PIM] steuern, wie [!DNL Workfront] andere Projektleistungsmetriken berechnet werden wie [!UICONTROL Kosten-Performance-Index] ([!UICONTROL CPI]), [!UICONTROL Kostenplan-Performance-Index] ([!UICONTROL CSI]), [!UICONTROL -Zeitplan-Performance-Index] ([!UICONTROL SPI]) und [!UICONTROL Schätzung bei Abschluss] ([!UICONTROL EAC]).

Optionen für die [!UICONTROL PIM] sind stundenbasiert und kostenbasiert.

* **Stundenbasiert** – Workfront verwendet die geplanten Arbeitsstunden zur Berechnung des CPI und der EAC des Projekts. Die EAC des Projekts wird als Zahl in Stunden angezeigt.
* **Kostenbasiert** – Workfront verwendet die geplanten Arbeitskosten zur Berechnung des CPI und der EAC des Projekts. EAC wird als Währungswert angezeigt. Stellen Sie bei Verwendung dieser Option sicher, dass Personen, die Aufgaben zugewiesen wurden (Benutzende und/oder Aufgabengebiete), Kostensätzen zugeordnet sind.

**[!UICONTROL EAC]**

[!UICONTROL EAC] stellt die voraussichtlichen Gesamtkosten Ihrer Aufgabe oder des Projekts nach Abschluss dar. Optionen werden auf Projektebene berechnet und von Aufgaben/Unteraufgaben hochgerechnet.

* **Auf Projektebene berechnen** – [!UICONTROL EAC] für die übergeordnete Aufgabe und das Projekt werden anhand der tatsächlichen Stunden bzw. tatsächlichen Arbeitskosten in [!UICONTROL EAC]-Formeln bestimmt. Die Berechnung umfasst die tatsächlichen Stunden/Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.
* **Aggregation von Aufgaben/Unteraufgaben** – Die [!UICONTROL EAC] für die übergeordnete Aufgabe und das übergeordnete Projekt wird durch Addieren der [!UICONTROL EAC] für jede untergeordnete Aufgabe ermittelt. Diese Berechnung schließt tatsächliche Stunden/Kosten aus, die direkt zu einer übergeordneten Aufgabe oder einem übergeordneten Projekt hinzugefügt werden.

Die [!UICONTROL EAC]-Berechnungen werden in der Liste [Berechnen der Schätzung bei Abschluss (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=de) aufgeführt.

**Leistungsmetriken: Einstellungen**

So werden Systemstandardwerte für [!UICONTROL PIM] und [!UICONTROL EAC] festgelegt:

1. Wählen Sie **[!UICONTROL Setup]** aus dem Hauptmenü aus.
1. Klicken Sie im Menü des linken Bedienfelds auf **[!UICONTROL Projektvoreinstellungen]** und dann auf **[!UICONTROL Projekte]**
1. Suchen Sie im Abschnitt [!UICONTROL Projektstatus] die [!UICONTROL Leistungsindex-Methode]. Wählen Sie „Stundenbasiert“ oder „Kostenbasiert“ aus.
1. Wählen Sie für [!UICONTROL Schätzung bei Abschluss] die Option „Auf Projektebene berechnen“ oder „Rollup aus Aufgaben/Unteraufgaben durchführen“ aus.
1. Klicken Sie unten im Fenster auf **[!UICONTROL Speichern]**.

![Ein Bild des Bildschirms [!UICONTROL Projektvoreinstellungen]](assets/setting-up-finances-1.png)

**Festlegen von [!UICONTROL PIM] für einzelne Projekte**

1. Rufen Sie die Landingpage eines Projekts auf.
1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Projektdetails]**.
1. Öffnen Sie den Abschnitt **[!UICONTROL Finanzen]**.
1. Doppelklicken Sie auf den Text **[!UICONTROL Performance-Index-Methode]** unten, um ihn zu bearbeiten.
1. Wählen Sie „Stundenbasiert“ oder „Kostenbasiert“ aus.
1. Klicken Sie zum Beenden auf **[!UICONTROL Speichern]**.

![Ein Bild des Bildschirms [!UICONTROL Projektdetails]](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kann für eine Projektvorlage im Abschnitt [!UICONTROL Finanzen] der Vorlagendetails festgelegt werden.

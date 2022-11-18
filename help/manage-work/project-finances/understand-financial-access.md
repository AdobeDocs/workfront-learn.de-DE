---
title: Finanziellen Zugang verstehen
description: Erfahren Sie, wie Administratoren mit finanziellen Zugriffsrechten steuern können, wer die in Workfront verfolgten Finanzinformationen anzeigen und bearbeiten kann.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# Finanziellen Zugang verstehen

Wenn Ihr Unternehmen Finanzdaten mit [!DNL Workfront]Als Systemadministrator sind Sie dafür verantwortlich, die Benutzer zu schützen und zu verwalten, die Zugriff auf diese Informationen haben.

Zwei Dinge sind erforderlich, damit ein Benutzer Finanzinformationen anzeigen oder bearbeiten kann:

1. Zugriffsberechtigungen müssen in der [!UICONTROL Zugriffsstufe].
2. Die Berechtigung zur Nutzung dieser Zugriffsrechte muss objektabhängig erteilt werden.

Beispielsweise kann einem Benutzer die Berechtigung zum Anzeigen von Finanzdaten in seiner Zugriffsebene gewährt werden, er kann jedoch nur Finanzdaten zu einer Aufgabe anzeigen, die für ihn freigegeben ist und die finanzielle Anzeige bei der Freigabe dieser Aufgabe aktiviert ist.

So ist es möglich, dass ein Benutzer mit [!UICONTROL Zugriffsstufe] Rechte zur Anzeige von Finanzmitteln, um Finanzierungen auf einigen Objekten und nicht auf anderen anzeigen zu können, abhängig von den individuellen Teilungsoptionen dieser Objekte. Kein Benutzer kann jedoch finanzielle Mittel zu einem Objekt einsehen, es sei denn, er hat in seinem [!UICONTROL Zugriffsstufe].

## [!UICONTROL Zugriffsstufe] settings

Der allgemeine Zugang zu Finanzdaten wird zunächst durch [!DNL Workfront] Lizenztyp.

**[!UICONTROL Plan] -Lizenzen können:**

* Rechnungsdatensätze verwalten
* Verwalten und Anzeigen der Rollenabrechnung und der Kostensätze
* Benutzerabrechnung und -kosten verwalten und anzeigen
* Verwalten von Ausgaben
* Anzeigen und Bearbeiten von Finanzen

**[!UICONTROL Arbeit] -Lizenzen können:**

* Verwalten von Ausgaben
* Anzeigen von Finanzen

**[!UICONTROL Überprüfen] -Lizenzen können:**

* Anzeigen von Finanzen

**Berechtigungen können durch die [!UICONTROL Zugriffsstufe]. Die drei Optionen für den finanziellen Datenzugriff sind:**

* [!UICONTROL Kein Zugriff] — Der Benutzer kann keine Finanzinformationen anzeigen.
* [!UICONTROL Ansicht] — Benutzer können die Informationen überprüfen und teilen.
* [!UICONTROL Bearbeiten] — Benutzer können die Informationen erstellen, bearbeiten, löschen und freigeben. (Nur für eine Planungslizenz verfügbar.)

![Ein Bild mit allgemeinen Finanzdatenoptionen auf Zugriffsebene](assets/setting-up-finances-8.png)

Beachten Sie, dass die Variable [!UICONTROL Ansicht] und [!UICONTROL Bearbeiten] -Optionen zusätzliche Einstellungen für eine [!UICONTROL Plan] Lizenz. Klicken Sie auf das Zahnrad auf der [!UICONTROL Ansicht] Schaltfläche für diese Optionen:

**[!UICONTROL Anzeigen]**

* Funktionsbezogene Fakturierung und Kostensätze anzeigen
* Benutzerfakturierung und Kostensätze anzeigen

![Ein Bild mit den Optionen zur Ansicht der Finanzdaten auf der Zugriffsebene](assets/setting-up-finances-9.png)

**[!UICONTROL Bearbeiten]**

Diese beiden Optionen sind im [!UICONTROL Bearbeiten] -Option sowie:

* Funktionsbezogene Fakturierung und Kostensätze bearbeiten
* Benutzerfakturierung und Kostensätze bearbeiten

![Ein Bild mit den Bearbeitungsoptionen für Finanzdaten auf Zugriffsebene](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Ein Benutzer mit Zugriff auf zusätzliche Ausgaben kann auch die von ihm hinzugefügten Ausgaben sowie die durch seine direkten Berichte hinzugefügten Ausgaben einsehen.

---
title: Globale Standardprojekteinstellungen konfigurieren
description: Erfahren Sie, wie Sie einen benutzerdefinierten Status ändern, globale Projektvoreinstellungen festlegen und Zeitpläne erstellen, die globale Standardeinstellungen sind.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Globale Standardprojekteinstellungen konfigurieren

<!---
21.4 updates have been made
--->

In diesem Video erfahren Sie, wie Sie:

* Benutzerdefinierten Status ändern
* Globale Projektvoreinstellungen festlegen
* Erstellen und Verwenden von Zeitplänen

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12)

## Globale und Gruppenprojekt-, Aufgaben- und Problemeinstellungen

Wenn Sie die [!UICONTROL Projekte] Einstellungen in [!DNL Workfront], werden Sie feststellen, dass &quot;[!UICONTROL Systemprojektvoreinstellungen]&quot; in der Suchleiste am oberen Rand des Fensters. Auf diese Weise erfahren Sie, welche Auswirkungen diese Einstellungen auf jeden in Ihrer [!DNL Workfront] System - es ist eine globale Konfiguration.

![[!UICONTROL Projektvoreinstellungen] Seite in [!UICONTROL Einrichtung]](assets/admin-fund-system-project-preferences-1.png)

Sie sehen etwas Ähnliches, wenn Sie die [!UICONTROL Aufgaben und Probleme] -Einstellungen.

![[!UICONTROL Voreinstellungen für Aufgaben und Probleme] in [!UICONTROL Einrichtung]](assets/admin-fund-task-issue-preferences-2.png)

Es ist jedoch möglich, dass nicht jede Gruppe in [!DNL Workfront] dieselben Voreinstellungen für Projekt, Aufgabe und Ausgabe benötigt. Beispielsweise möchte die Marketing-Gruppe, dass der Status eines neuen Projekts &quot;Planung&quot;lautet, während die Projekt-Manager-Gruppe den Anforderungsstatus bevorzugt.

[!DNL Workfront] ermöglicht es Gruppenadministratoren, bestimmte Projekt-, Aufgaben- und Problemvoreinstellungen für ihre Gruppen anzupassen. Welche Voreinstellungen angepasst werden können, hängt von der [!DNL Workfront] Systemadministrator, der die Umschalter zum Sperren/Entsperren verwendet.

Navigieren Sie zunächst zur [!UICONTROL Einrichtung] Bereich:

1. Auswählen **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern **[!UICONTROL Projektvoreinstellungen]** im linken Menü.
1. Auswählen **[!UICONTROL Projekte]** oder **[!UICONTROL Aufgaben und Probleme]**, je nachdem, welche Einstellungen Sie ändern möchten.

Sperren Sie eine Voreinstellung, um zu verhindern, dass Gruppenadministratoren diese Einstellung für ihre Gruppe anpassen.

![Gesperrte Präferenznachricht](assets/admin-fund-preferences-locked-3.png)

Entsperren Sie die Voreinstellung, um sie für Gruppenadministratoren zur Verfügung zu stellen.

![Entsperrte Präferenznachricht](assets/admin-fund-preferences-unlocked-4.png)

Einige Einstellungen können nicht entsperrt werden und bleiben globale Systemeinstellungen.

![Gesperrte Präferenznachricht](assets/admin-fund-preferences-always-locked-5.png)

### Festlegen von Gruppen- und Untergruppenvoreinstellungen

Für alle vom Systemadministrator entsperrten Einstellungen können die Gruppenadministratoren Anpassungen für die von ihnen verwalteten Gruppen und alle Untergruppen vornehmen, die unter diesen Gruppen verschachtelt sind. Darüber hinaus können Gruppenadministratoren steuern, welche Einstellungen ihre Untergruppen-Administratoren ändern können.

1. Auswählen **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Klicken **[!DNL Groups]** im linken Menü.
1. Klicken Sie auf den Namen der Gruppe oder Untergruppe, um sie zu öffnen.
1. Auswählen **[!UICONTROL Projektvoreinstellungen]** oder **[!UICONTROL Voreinstellungen für Aufgaben und Probleme]** im linken Menü.
1. Nehmen Sie die für die einzelnen Voreinstellungen erforderlichen Änderungen vor, die entsperrt wurden.
1. Auswählen **[!UICONTROL Speichern]**.

![[!UICONTROL Projektstatus] Abschnitt [!UICONTROL Gruppe] page](assets/admin-fund-group-preferences.png)

Wenn Ihr Unternehmen keine Gruppenadministratoren verwendet, kann der Systemadministrator die Voreinstellungen für die verschiedenen Gruppen verwalten.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->

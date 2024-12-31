---
title: Einrichten von Gruppen und Benutzern
description: Erfahren Sie, wie Sie Ordner, Gruppen und Benutzende in [!UICONTROL Workfront DAM] erstellen. Machen Sie sich mit den Typen von Benutzerrollen und dem Gewähren von Berechtigungen für Ordner vertraut.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 95%

---

# Einrichten von Gruppen und Benutzern

In diesem Video lernen Sie Folgendes:

* Erfahren Sie, wie sich Gruppen-Setups auf den Zugriff auf Assets auswirken
* Erstellen von Ordnern, Gruppen und Benutzenden in einer bestimmten Reihenfolge
* Verstehen von Typen von Benutzerrollen
* Gewähren von Berechtigungen für Ordner
* Erstellen und Bearbeiten von Gruppen
* Hinzufügen und Bearbeiten von Benutzenden

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Überprüfen von Gruppen und Benutzenden

Beim Konfigurieren des [!UICONTROL Workfront DAM]-Systems ist es wichtig, die Rollen zu berücksichtigen, die Benutzende und Gruppen im Gesamtbild spielen.

Gruppen steuern den Zugriff auf Asset-Ordner in [!UICONTROL Workfront DAM]. Gruppeneinstellungen steuern auch, was Benutzer mit den Assets tun können (Anzeigen, Herunterladen, Bearbeiten usw.), für die sie Zugriffsberechtigungen haben.

Beim Erstellen von Gruppen ist es wichtig zu beachten, auf welche Asset-Ordner in [!UICONTROL Workfront DAM] die Mitglieder der jeweiligen Gruppe Zugriff benötigen.

Benutzende sind Personen, die sich bei [!UICONTROL Workfront DAM] anmelden können. Benutzende können auf nichts in [!UICONTROL Workfront DAM] zugreifen, es sei denn, sie sind einer Gruppe zugewiesen. Je nach Bedarf können Benutzende mehreren Gruppen angehören.

## Standardgruppen

Es gibt zwei Standardgruppen in [!UICONTROL Workfront DAM]. Alle Benutzenden gehören automatisch zu einer dieser beiden Gruppen, je nachdem, ob sie sich bei [!UICONTROL Workfront DAM] anmelden können oder nicht. Sie können keine Benutzenden zu diesen Gruppen hinzufügen oder daraus entfernen:

* **Gastgruppe** – Wird verwendet, um den Zugriff für anonyme Benutzende zu steuern. Dies kann eine Person ohne Anmeldeinformationen oder eine Person sein, die derzeit nicht angemeldet ist.
* Gruppe **Angemeldet** – Alle angemeldeten Benutzenden gehören dieser Gruppe an.

Die Admingruppe und ihre Einstellungen sind ebenfalls standardmäßig vorhanden. Sie können dieser Gruppe Benutzende hinzufügen, die Einstellungen können jedoch nicht angepasst werden.

## Rollentypen

Bei der Erstellung von Gruppen wird diesen ein Rollentyp zugewiesen. Der Rollentyp bestimmt, welchen Teil von [!UICONTROL Workfront DAM] die Systembenutzenden bei der Anmeldung erhalten – [!UICONTROL Workfront DAM] selbst oder [!UICONTROL Brand Connect].

Mit einer Lizenz für [!UICONTROL Workfront DAM] stehen drei Rollentypen zur Verfügung:

* **[!UICONTROL Brand Portal]** – Diese Benutzenden haben nur Zugriff auf [!UICONTROL Brand Connect], wo sie genehmigte Assets anzeigen und herunterladen können.
* **[!UICONTROL Mitwirkende]** – Diese Benutzenden können auf [!UICONTROL Workfront DAM] und [!UICONTROL Brand Connect] zugreifen. Sie verfügen über vollständige Zugriffsrechte auf Assets und Ordner – Ansicht, Download, Upload, Bearbeiten, Verschieben und Löschen.
* **[!UICONTROL Administrator]** – Systemadmins haben Zugriff auf alles in [!UICONTROL Brand Connect] und [!UICONTROL Workfront DAM] und die Möglichkeit, die globalen Systemeinstellungen für jedes System festzulegen. Sie können auch auf Assets zugreifen, die abgelaufen sind oder als inaktiv festgelegt wurden.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->

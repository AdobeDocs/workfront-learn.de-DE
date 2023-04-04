---
title: Grundlegendes zu Gruppen und Benutzern in [!UICONTROL Workfront DAM]
description: Erfahren Sie, wie Sie Ordner, Gruppen und Benutzer in [!UICONTROL Workfront DAM]. Machen Sie sich mit den Benutzerrollentypen und gewähren Sie Berechtigungen für Ordner.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# System-Setup: Gruppen und Benutzer

In diesem Video erfahren Sie, wie Sie:

* Erfahren Sie, wie sich Gruppenkonfigurationen auf den Zugriff auf Assets auswirken
* Erstellen von Ordnern, Gruppen und Benutzern in einer bestimmten Reihenfolge
* Grundlegendes zu den Benutzerrollentypen
* Berechtigungen für Ordner gewähren
* Gruppen erstellen und bearbeiten
* Benutzer hinzufügen und bearbeiten

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Gruppen und Benutzer - Überblick

Während der Konfiguration [!UICONTROL Workfront DAM] -System, ist es wichtig, die Rollen zu berücksichtigen, die Benutzer und Gruppen im Großen und Ganzen spielen.

Gruppen steuern den Zugriff auf Asset-Ordner in [!UICONTROL Workfront DAM]. Gruppeneinstellungen steuern auch, was Benutzer mit den Assets tun können (Anzeigen, Herunterladen, Bearbeiten usw.) sie haben Zugriff.

Beim Erstellen von Gruppen ist es wichtig zu beachten, auf welche Asset-Ordner die Mitglieder dieser Gruppe Zugriff in benötigen [!UICONTROL Workfront DAM].

Benutzer sind Personen, die sich bei anmelden [!UICONTROL Workfront DAM]. Ein Benutzer kann auf nichts in [!UICONTROL Workfront DAM] , es sei denn, sie sind einer Gruppe zugewiesen. Je nach Bedarf können Benutzer mehreren Gruppen angehören.

## Standardgruppen

Es gibt zwei Standardgruppen, die [!UICONTROL Workfront DAM]. Alle Benutzer gehören automatisch zu diesen Gruppen, je nachdem, ob sie [!UICONTROL Workfront DAM] Anmeldedaten. Sie können keine Benutzer zu diesen Gruppen hinzufügen oder daraus entfernen:

* **Gastgruppe**—Dient zur Zugriffskontrolle für einen anonymen Benutzer. Dies kann eine Person ohne Anmeldeinformationen oder ein Benutzer sein, der derzeit nicht angemeldet ist.
* **Protokolliert**-In-Gruppe - Alle angemeldeten Benutzer gehören dieser Gruppe an.

Die Administratorgruppe und ihre Einstellungen sind ebenfalls standardmäßig vorhanden. Sie können dieser Gruppe Benutzer hinzufügen, die Einstellungen können jedoch nicht angepasst werden.

## Rollenarten

Bei der Erstellung von Gruppen wird ihnen ein Rollentyp zugewiesen. Der Rollentyp bestimmt, welcher Teil der [!UICONTROL Workfront DAM] Systembenutzer erhalten bei der Anmeldung eine [!UICONTROL Workfront DAM] selbst oder [!UICONTROL Brand Connect].

Es stehen drei Rollentypen zur Verfügung mit [!UICONTROL Workfront DAM] Lizenzen:

* **[!UICONTROL Brand Portal]**—Diese Benutzer haben nur Zugriff auf [!UICONTROL Brand Connect], wo sie genehmigte Assets anzeigen und herunterladen können.
* **[!UICONTROL Mitarbeiter]**—Diese Benutzer können auf [!UICONTROL Workfront DAM] und [!UICONTROL Brand Connect]. Sie haben volle Zugriffsrechte auf Assets und Ordner - Ansicht, Download, Upload, Bearbeiten, Verschieben und Löschen.
* **[!UICONTROL Administrator]**—Systemadministratoren haben Zugriff auf alles in [!UICONTROL Brand Connect] und [!UICONTROL Workfront DAM]und die Möglichkeit, die globalen Systemeinstellungen für jedes System festzulegen. Sie können auch auf Assets zugreifen, die abgelaufen sind oder als inaktiv festgelegt wurden.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->

---
title: Erfahren Sie, wie Sie Assets in verwalten [!UICONTROL Workfront DAM]
description: Erfahren Sie, wie Sie Assets in verwalten [!UICONTROL Workfront DAM] , um Ihren Workflow zu verbessern.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Mitarbeiter: Asset-Management

In diesem Video erfahren Sie, wie Sie:

* Verwenden des Menüs &quot;Bearbeiten&quot;für ein Asset
* Ablaufdatum festlegen
* Benachrichtigungen anzeigen
* Festlegen einzelner Benachrichtigungseinstellungen
* Hochladen einer Asset-Version
* Neuen Ordner erstellen
* Anwenden einer Metadatenvorlage auf einen Ordner
* Festlegen von Ordnerberechtigungen

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## Funktionsweise von Asset-Versionen

Ein Teil Ihres Workflows kann die Verwaltung mehrerer Versionen eines Assets (Runden, Testsendungen, Iterationen, so wie Sie sie nennen) umfassen. Sie können alle Versionen über [!UICONTROL Workfront DAM].

Das System ermöglicht eine automatische Versionskontrolle für Assets, wenn eine Datei mit demselben Namen wie eine vorhandene Datei in denselben Ordner hochgeladen wird. Wenden Sie sich an Ihren Systemadministrator, um zu sehen, ob diese Funktion aktiviert wurde.

Wenn die automatische Versionskontrolle aktiviert ist, wird ein Asset nur dann in die Version geladen, wenn es in den Ordner geladen wird, der das Original-Asset enthält. Beide Assets müssen denselben Dateinamen haben. Wenn das Asset in einen anderen Ordner geladen wird, wird das Asset als neue Datei eingefügt.
Wenn die Versionskontrolle nicht aktiviert ist, wird eine Datei mit demselben Namen wie eine vorhandene Datei als neue Datei hochgeladen, unabhängig davon, in welchem Ordner sie gespeichert ist. Dies könnte dazu führen, dass sich zwei Assets mit demselben Namen im selben Ordner befinden.

Sie können auch manuell Versionen eines bestimmten Assets hochladen. Klicken Sie auf das Bearbeitungssymbol für das Asset und wählen Sie **[!UICONTROL Neue Version hochladen]**.

Wenn Sie ein Asset mit Versionen in Brand Connect veröffentlichen, sieht der Brand Connect-Benutzer nur die neueste Version des Assets.

## Ordner- und Asset-Status und -Ablauf

Status sind eine weitere Möglichkeit, den Zugriff auf Ordner und Assets in [!UICONTROL Workfront DAM]. Status können verwendet werden, um bestimmte Assets oder Ordner vor [!UICONTROL Brand Connect] Benutzer oder ein Asset oder einen Ordner ablaufen lassen, damit nur der Systemadministrator darauf zugreifen kann.

* **[!UICONTROL Aktiv]**- Wird für Assets und Ordner verwendet. Assets und Ordner mit dem [!UICONTROL Aktiv] Status sind für alle Benutzer mit Berechtigungen sichtbar und können in veröffentlicht werden. [!UICONTROL Brand Connect]. [!UICONTROL Aktiv] wird mit einem grünen Punkt auf einem Asset oder Ordner angezeigt.
* **[!UICONTROL Inaktiv]**- Wird für Assets und Ordner verwendet. Assets und Ordner mit dem [!UICONTROL Inaktiv] -Status sichtbar für [!UICONTROL Workfront DAM] -Benutzer, jedoch nicht in der [!UICONTROL Brand Connect]. [!UICONTROL Inaktiv] wird mit einem roten Punkt auf einem Asset oder Ordner angezeigt.
* **[!UICONTROL Unerwartet]**- Wird nur für Assets verwendet. Dies ist der Standardstatus aller Assets. Unerwartete Assets, die ebenfalls [!UICONTROL Aktiv] sind im [!UICONTROL Brand Connect].
* **[!UICONTROL Abgelaufen]**- Wird nur für Assets verwendet. Assets mit der [!UICONTROL Abgelaufen] -Status kann von keinem Benutzer außer dem Systemadministrator heruntergeladen werden. Abgelaufene Assets sind im [!UICONTROL Brand Connect], abhängig von den Systemkonfigurationen.

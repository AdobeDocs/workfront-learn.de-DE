---
title: Grundlegendes zur Asset-Verwaltung als Mitwirkende
description: Erfahren Sie, wie Sie Assets in [!UICONTROL Workfront DAM] verwalten können, um Ihren Workflow zu verbessern.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:28:05.016Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 100%

---

# Grundlegendes zur Asset-Verwaltung als Mitwirkende

In diesem Video lernen Sie Folgendes:

* Wie Sie das Menü „Bearbeiten“ für ein Asset verwenden
* Ablaufdatum festlegen
* Benachrichtigungen anzeigen
* Einzelne Benachrichtigungseinstellungen festlegen
* Eine Asset-Version hochladen
* Einen neuen Ordner erstellen
* Eine Metadatenvorlage auf einen Ordner anwenden
* Ordnerberechtigungen festlegen

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on&enablevpops=1)

## Funktionsweise von Asset-Versionen

Ein Teil Ihres Workflows kann die Verwaltung mehrerer Versionen – oder Runden, Überprüfungen, Iterationen, wie auch immer Sie sie nennen – eines Assets beinhalten. Sie können alle Versionen über [!UICONTROL Workfront DAM] verwalten.

Das System ermöglicht eine automatische Asset-Versionskontrolle, wenn eine Datei mit dem Namen einer bereits bestehenden Datei in denselben Ordner hochgeladen wird. Wenden Sie sich an Ihre Systemadmins, um zu prüfen, ob diese Funktion aktiviert wurde.

Wenn die automatische Versionskontrolle aktiviert ist, wird ein Asset nur dann versioniert, wenn es in den Ordner mit dem Original-Asset geladen wird. Beide Assets müssen denselben Dateinamen haben. Wenn das Asset in einen anderen Ordner geladen wird, wird das Asset als neue Datei eingefügt.
Wenn die Versionskontrolle nicht aktiviert ist, wird eine Datei mit dem Namen einer bereits vorhandenen Datei als neue Datei hochgeladen, unabhängig davon, in welchem Ordner sie abgelegt ist. Dies kann dazu führen, dass sich zwei Assets mit demselben Namen im selben Ordner befinden.

Sie können auch manuell Versionen eines bestimmten Assets hochladen. Klicken Sie auf das Bearbeitungssymbol für das Asset und wählen Sie **[!UICONTROL Neue Version hochladen]**.

Wenn Sie ein Asset mit Versionen in Brand Connect veröffentlichen, sieht die Person, die Brand Connect verwendet, nur die neueste Version des Assets.

## Status und Ablauf von Ordnern und Assets

Status sind eine weitere Möglichkeit, den Zugang zu Ordnern und Assets in [!UICONTROL Workfront DAM] zu verwalten. Anhand des Status können Sie bestimmte Assets oder Ordner vor [!UICONTROL Brand Connect]-Benutzenden verbergen oder ein Asset oder einen Ordner ablaufen lassen, sodass nur Systemadmins darauf zugreifen können.

* **[!UICONTROL Aktiv]** – Wird für Assets und Ordner verwendet. Assets und Ordner mit dem Status [!UICONTROL Aktiv] sind für alle Benutzenden mit Berechtigungen sichtbar und können auf [!UICONTROL Brand Connect] veröffentlicht werden. [!UICONTROL Aktiv] wird mit einem grünen Punkt auf einem Asset oder Ordner angezeigt.
* **[!UICONTROL Inaktiv]** – Wird für Assets und Ordner verwendet. Assets und Ordner mit dem Status [!UICONTROL Inaktiv] sind für [!UICONTROL Workfront DAM]-Benutzende sichtbar, aber nicht in [!UICONTROL Brand Connect]. [!UICONTROL Inaktiv] wird durch einen roten Punkt auf einem Asset oder Ordner angezeigt.
* **[!UICONTROL Nicht abgelaufen]** – Wird nur für Assets verwendet. Dies ist der Standardstatus aller Assets. Nicht abgelaufene Assets, die auch [!UICONTROL Aktiv] sind, werden in [!UICONTROL Brand Connect] angezeigt.
* **[!UICONTROL Abgelaufen]** – Wird nur für Assets verwendet. Assets mit dem Status [!UICONTROL Abgelaufen] können nur von Systemadmins heruntergeladen werden. Abgelaufene Assets sind je nach Systemkonfiguration in [!UICONTROL Brand Connect] sichtbar/nicht sichtbar.

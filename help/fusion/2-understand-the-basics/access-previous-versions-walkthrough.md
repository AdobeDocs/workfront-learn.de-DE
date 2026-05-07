---
title: Anleitung zum Zugriff auf frühere Versionen
description: Erfahren Sie, wie Sie frühere Versionen wiederherstellen können, nachdem Sie Änderungen an Ihrem Szenario vorgenommen und in  [!DNL Adobe Workfront Fusion] gespeichert haben.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9009
exl-id: dd2cc2a2-e5af-41cc-bc0d-6be1efd996d9
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:39:17.503Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# Anleitung zum Zugriff auf frühere Versionen

In diesem Video werden Sie:

* Erfahren Sie, wie Sie frühere Versionen wiederherstellen können, nachdem Sie Änderungen an Ihrem Szenario vorgenommen und mehrmals gespeichert haben.

## Anleitung zum Zugriff auf frühere Versionen

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335268/?quality=12&learn=on&enablevpops=1)

>[!NOTE]
>
>Nach dem Speichern des Szenarios ist eine neue Version unter dem Menü mit drei Punkten verfügbar, falls Sie in Zukunft darauf zugreifen müssen. Zuvor gespeicherte Szenario-Versionen sind nur für 60 Tage verfügbar. Wenn Sie zu Prüfzwecken über die 60 Tage hinaus auf frühere Versionen zugreifen müssen, empfiehlt Workfront, einen Entwurf Ihres Szenarios zu speichern und an einem vereinbarten Speicherort zu archivieren.


## Zu Ihrer Terminologie hinzufügen

![Ein Bild eines überwachten Eintrags und eines benutzerdefinierten Webhook-Moduls](assets/understand-the-basics-3.png)

### Trigger-Module

Trigger-Module können nur als erstes Modul verwendet werden und können null, eins oder mehrere Bündel zurückgeben. Diese werden einzeln in nachfolgenden Modulen verarbeitet, sofern sie nicht aggregiert werden.

**Abruf-Trigger (mit Uhrensymbol)** – Spezielle Funktionen, um den zuletzt verarbeiteten Eintrag zu verfolgen.

**Sofortiger Trigger (mit Blitzsymbol)** – Wird sofort ausgelöst, je nach Webhook.

![Ein Bild einer Eintragserstellung und eines Suchmoduls](assets/understand-the-basics-4.png)

### Aktionen und Suchmodule

**Aktion** – Wird verwendet, um CRUD-Vorgänge (Erstellen, Lesen, Aktualisieren und Löschen) durchzuführen

**Suchvorgänge** – Wird verwendet, um nach null, einem oder mehreren Einträgen zu suchen, und gibt diese als Bündel zurück, die einzeln in nachfolgenden Modulen verarbeitet werden, sofern sie nicht aggregiert werden.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Workfront Fusion-Dokumentation](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

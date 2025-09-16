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
source-git-commit: dfcca5f02a6d9f7ee44a1e894106ae48259eea91
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 99%

---

# Anleitung zum Zugriff auf frühere Versionen

In diesem Video werden Sie:

* Erfahren Sie, wie Sie frühere Versionen wiederherstellen können, nachdem Sie Änderungen an Ihrem Szenario vorgenommen und mehrmals gespeichert haben.

## Anleitung zum Zugriff auf frühere Versionen

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335268/?quality=12&learn=on&enablevpops)

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

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

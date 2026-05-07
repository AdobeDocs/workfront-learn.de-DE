---
title: Datenspeicher – Anleitung
description: Erfahren Sie, wie Sie in [!DNL Adobe Workfront Fusion]mit einem Datenspeicher Firmennamen zwischen einer Firmenliste und Workfront synchronisieren können.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:18:10.872Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 411
ht-degree: 100%

---

# Datenspeicher – Anleitung

In dieser Übung verwenden wir einen Datenspeicher, um Firmennamen zwischen einer Firmenliste und Workfront zu synchronisieren.

Dies ist Teil einer unidirektionalen Synchronisierung von Firmen in Workfront und anderen Systemen. Derzeit wird nur zwischen einer CSV-Datei und Workfront synchronisiert. Es wird jedoch auch eine Tabelle in einem Datenspeicher verwaltet, in der die Workfront-ID (WFID) und die Firmen-ID in der CSV-Datei (CID) für jedes Unternehmen verfolgt werden. Dies ermöglicht es uns, die Synchronisierung zu einem späteren Zeitpunkt bidirektional zu machen.

![Ein Bild eines Fusion-Szenarios](assets/data-structures-and-data-stores-2.png)

## Datenspeicher – Anleitung

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on&enablevpops=1)



## Schlussbemerkung

Nachdem Sie nun mit dem Lernen über Datenstrukturen und Datenspeicher fertig sind, fragen Sie sich vielleicht, wann Sie diese verwenden sollten.

Datenstrukturen werden meist zum Serialisieren oder Analysieren von JSON, XML, CSV und anderen Datenformaten verwendet. Mit Datenstrukturen können Sie die Struktur Ihrer Daten steuern und sogar Daten validieren. Am häufigsten werden Datenstrukturen dafür verwendet, gültige Daten zu erstellen, um sie an eine API zu senden, die JSON oder XML erwartet. In diesen Fällen sollten Sie die JSON- oder XML-App zusammen mit Ihrer Datenstruktur verwenden, um sicherzustellen, dass die Daten im richtigen Format vorliegen.

Datenspeicher sollten nur zum Speichern persistenter Daten verwendet werden, auf die von mehr als einer Szenarioausführung zugegriffen werden muss. Sie können beispielsweise bei fortgeschrittenen Anwendungsfällen, die eine präzise Steuerung der Verarbeitung erfordern, Metadaten über den letzten verarbeiteten Eintrag speichern.

Datenspeicher sind nicht für die Verwendung als Data Warehouse oder zur Protokollierung vorgesehen. Datenspeicher sind außerhalb von Workfront Fusion nicht zugänglich, und die meisten Interaktionen mit Datenspeichern erfolgen über ein Workfront Fusion-Szenario. Folglich ist es nicht möglich, einen Datenspeicher mit einem Analyse- oder Reporting-Tool zu verbinden, das für Anwendungsfälle von Data Warehouses oder Protokollierung zu erwarten wäre. Die Rolle von Workfront Fusion in Anwendungsfällen wie diesen bestünde darin, ein System aufzufüllen, das sich für das Organisieren und Speichern von Daten eignet (z. B. SQL oder MariaDB).

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Workfront Fusion-Dokumentation](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

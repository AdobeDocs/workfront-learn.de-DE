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
source-git-commit: dfcca5f02a6d9f7ee44a1e894106ae48259eea91
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 99%

---

# Datenspeicher – Anleitung

In dieser Übung verwenden wir einen Datenspeicher, um Firmennamen zwischen einer Firmenliste und Workfront zu synchronisieren.

Dies ist Teil einer unidirektionalen Synchronisierung von Firmen in Workfront und anderen Systemen. Derzeit wird nur zwischen einer CSV-Datei und Workfront synchronisiert. Es wird jedoch auch eine Tabelle in einem Datenspeicher verwaltet, in der die Workfront-ID (WFID) und die Firmen-ID in der CSV-Datei (CID) für jedes Unternehmen verfolgt werden. Dies ermöglicht es uns, die Synchronisierung zu einem späteren Zeitpunkt bidirektional zu machen.

![Ein Bild eines Fusion-Szenarios](assets/data-structures-and-data-stores-2.png)

## Datenspeicher – Anleitung

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on&enablevpops)



## Schlussbemerkung

Nachdem Sie nun mit dem Lernen über Datenstrukturen und Datenspeicher fertig sind, fragen Sie sich vielleicht, wann Sie diese verwenden sollten.

Datenstrukturen werden meist zum Serialisieren oder Analysieren von JSON, XML, CSV und anderen Datenformaten verwendet. Mit Datenstrukturen können Sie die Struktur Ihrer Daten steuern und sogar Daten validieren. Am häufigsten werden Datenstrukturen dafür verwendet, gültige Daten zu erstellen, um sie an eine API zu senden, die JSON oder XML erwartet. In diesen Fällen sollten Sie die JSON- oder XML-App zusammen mit Ihrer Datenstruktur verwenden, um sicherzustellen, dass die Daten im richtigen Format vorliegen.

Datenspeicher sollten nur zum Speichern persistenter Daten verwendet werden, auf die von mehr als einer Szenarioausführung zugegriffen werden muss. Sie können beispielsweise bei fortgeschrittenen Anwendungsfällen, die eine präzise Steuerung der Verarbeitung erfordern, Metadaten über den letzten verarbeiteten Eintrag speichern.

Datenspeicher sind nicht für die Verwendung als Data Warehouse oder zur Protokollierung vorgesehen. Datenspeicher sind außerhalb von Workfront Fusion nicht zugänglich, und die meisten Interaktionen mit Datenspeichern erfolgen über ein Workfront Fusion-Szenario. Folglich ist es nicht möglich, einen Datenspeicher mit einem Analyse- oder Reporting-Tool zu verbinden, das für Anwendungsfälle von Data Warehouses oder Protokollierung zu erwarten wäre. Die Rolle von Workfront Fusion in Anwendungsfällen wie diesen bestünde darin, ein System aufzufüllen, das sich für das Organisieren und Speichern von Daten eignet (z. B. SQL oder MariaDB).

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

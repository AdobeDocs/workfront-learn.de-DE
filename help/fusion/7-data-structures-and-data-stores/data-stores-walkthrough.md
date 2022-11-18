---
title: Anleitung zu Datenspeichern
description: Erfahren Sie, wie Sie mit einem Datenspeicher Firmennamen zwischen einer Unternehmensliste und Workfront synchronisieren können, indem Sie [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Anleitung zu Datenspeichern

## Übersicht

In dieser Übung verwenden wir einen Datenspeicher, um Unternehmensnamen zwischen einer Unternehmensliste und Workfront zu synchronisieren.

Dies ist Teil einer unidirektionalen Synchronisation von Unternehmen in Workfront und anderen Systemen. Derzeit wird sie nur zwischen einer CSV-Datei und Workfront synchronisiert. Es wird jedoch auch eine Tabelle in einem Datenspeicher verwaltet, in dem die Workfront ID (WFID) und die Unternehmens-ID in der CSV-Datei (CID) für jedes Unternehmen verfolgt werden. Dies wird es uns ermöglichen, dies zu einem späteren Zeitpunkt zu einer bidirektionalen Synchronisation zu machen.

![Bild eines Fusionsszenarios](assets/data-structures-and-data-stores-2.png)

## Anleitung zu Datenspeichern

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Eine schrittweise Anleitung zum Abschließen der exemplarischen Vorgehensweise finden Sie im Abschnitt [Anleitung zu Datenspeichern](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) Übung.


## Schlussbemerkung

Nachdem Sie sich mit den Datenstrukturen und Datenspeichern vertraut gemacht haben, fragen Sie sich vielleicht: &quot;Wann sollten Sie sie verwenden?&quot;

Datenstrukturen werden meist zum Serialisieren oder Parsen von Datenformaten wie JSON, XML, CSV und anderen verwendet. Mit Datenstrukturen können Sie die Struktur Ihrer Daten steuern und sogar Daten validieren. Der häufigste Grund für die Verwendung einer Datenstruktur besteht darin, gültige Daten zu erstellen, die an eine API gesendet werden, die JSON oder XML erwartet. In diesen Fällen sollten Sie die JSON- oder XML-App zusammen mit Ihrer Datenstruktur verwenden, um sicherzustellen, dass die Daten im richtigen Format vorliegen.

Datenspeicher sollten nur zum Speichern persistenter Daten verwendet werden, auf die für mehrere Szenarien zugegriffen werden muss. Sie können beispielsweise Metadaten zum letzten Datensatz speichern, der für erweiterte Anwendungsfälle verarbeitet wurde, die eine genaue Kontrolle über die Verarbeitung erfordern.

Datenspeicher sind nicht für die Verwendung als Data Warehouse oder Protokollierung vorgesehen. Datenspeicher sind außerhalb von Workfront Fusion nicht zugänglich und die meisten Interaktionen mit Datenspeichern erfolgen über ein Workfront Fusion-Szenario. Folglich ist es nicht möglich, einen Datenspeicher mit einem Analyse- oder Reporting-Tool zu verbinden, das für Data Warehouse- und Protokollierungsanwendungsfälle erwartet wird. Die Rolle von Workfront Fusion bei Anwendungsfällen wie diesen bestünde darin, ein für die Organisation und Speicherung von Daten geeignetes System (z. B. SQL, MariaDB) aufzufüllen.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)

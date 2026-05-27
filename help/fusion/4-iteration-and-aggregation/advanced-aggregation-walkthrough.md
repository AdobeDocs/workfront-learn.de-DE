---
title: Erweiterte Aggregation – Anleitung
description: Lernen Sie, wie Sie in [!DNL Adobe Workfront Fusion]einen Web-Dienst aufrufen, um Details zu mehreren Ländern abzurufen und die Population zu identifizieren, gruppiert nach Unterregionen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 100%

---

# Erweiterte Aggregation – Anleitung

Aufruf eines Web-Dienstes zur Abfrage von Details zu mehreren Ländern und zur Ermittlung der Gesamtpopulation aller Länder, gruppiert nach Unterregionen.

![Ein Bild des Fusion-Szenarios](assets/iteration-and-aggregation-3.png)

## Erweiterte Aggregation – Anleitung

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## Übungs-URLs

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Stärkung des Aggregationsprinzips

Immer wenn ein Modul mehrere Bündel ausgibt, wird jedes nachfolgende Modul jedes Bündel ausführen.

Um dies zu verhindern, fügen Sie hinter einem Modul, das möglicherweise mehrere Bündel erzeugt, einen Aggregator ein.

Sie werden einen Schatten sehen, der jedes Segment in Ihrem Szenario von einem **Anfangsiterator** bis zum **Endaggregator** umgibt. So lassen sich diese Segmente in Ihrem Workfront Fusion-Szenario leicht erkennen.

## Sie sind dran

>[!NOTE]
>
>Die Übungen und Herausforderungen sind optional und nicht notwendig, um die Fusion-Schulung abzuschließen.

Diese Übung baut auf dem auf, was Sie in der exemplarischen Vorgehensweise gelernt haben, aber die Lösung wird nicht bereitgestellt.

Erstellen Sie ein neues Szenario, um alle Stunden zu summieren, die für Aufgaben in Projekten aus dem Marketing-Portfolio aufgezeichnet wurden. Senden Sie dann eine E-Mail mit dem Inhalt „Ihr Projekt-Team {Project Name} hat {summed hours} der insgesamt {planned hours} geplanten Stunden verbucht, sodass {percentage} des Plans erfüllt sind.“

**Herausforderung:** Versuchen Sie, nun dasselbe zu tun, aber nur für die in diesem Jahr erfassten Stunden.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Workfront Fusion-Dokumentation](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

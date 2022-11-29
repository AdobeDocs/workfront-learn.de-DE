---
title: Anleitung zur erweiterten Aggregation
description: Erfahren Sie, wie Sie einen Webdienst aufrufen, um Details zu mehreren Ländern zurückzugeben und die Population, gruppiert nach Unterregion, zu identifizieren, die alle in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: 96f963bf5a44eac234cbf9215f19f6dddbe23143
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Anleitung zur erweiterten Aggregation

## Übersicht

Rufen Sie einen Webdienst auf, um Details zu mehreren Ländern zurückzugeben und die Gesamtbevölkerung aller Länder, gruppiert nach Unterregion, zu identifizieren.

![Ein Bild des Fusion-Szenarios](assets/iteration-and-aggregation-3.png)

## Anleitung zur erweiterten Aggregation

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## Übungs-URLs

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Eine schrittweise Anleitung zum Abschließen der exemplarischen Vorgehensweise finden Sie im Abschnitt [Anleitung zur erweiterten Aggregation](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) Übung.

## Stärkung des Aggregationsprinzips

Jedes Mal, wenn ein Modul mehrere Bundles ausgibt, wird jedes nachfolgende Modul jedes Bundle ausführen.

Um dies zu verhindern, fügen Sie einen Aggregator nach einem Modul hinzu, das möglicherweise mehrere Bundles erzeugt.

Sie sehen einen Schatten, der jedes Segment in Ihrem Szenario von einem **Startiterator** der **endaggregator**. Dies erleichtert die Erkennung dieser Segmente in Ihrem Workfront Fusion-Szenario.

## Ihre Wendung

>[!NOTE]
>
>Übungen sind optional und nicht erforderlich, um die Fusion-Schulung abzuschließen.

Diese Übung baut auf dem auf, was Sie in der exemplarischen Vorgehensweise gelernt haben, aber die Lösung wird nicht bereitgestellt.

Erstellen Sie ein neues Szenario, um alle Stunden zu summieren, die für Aufgaben in Projekten im Marketing-Portfolio angemeldet sind. Senden Sie dann eine E-Mail, in der steht: &quot;Ihr {Projektname} Projektteam hat {Gesamtstunden} der geplanten Gesamtstunden protokolliert, sodass Sie {Prozentsatz} des Plans erreichen.&quot;

**Herausforderung:** Überprüfen Sie, ob Sie dasselbe tun können, aber nur für Stunden, die in diesem Jahr protokolliert werden.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)

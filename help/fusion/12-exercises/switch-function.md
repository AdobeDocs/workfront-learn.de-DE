---
title: Übung zur Switch-Funktion
description: Erfahren Sie, wie Sie die Umschaltfunktionalität nutzen können, indem Sie die Umschaltfunktion verwenden.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
autotag-review: '2026-05-06T16:41:24.173Z'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
    internal-label: Workfront Fusion
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 100%
---
# Übung zur Switch-Funktion

Erfahren Sie, wie Sie die Umschaltfunktionalität nutzen können, indem Sie die Umschaltfunktion verwenden.

## Übungsübersicht

Verwenden Sie für einfache Datenänderungen die Switch-Funktion, um einen Wert innerhalb eines Modulfelds in einen anderen umzuwandeln. Ändern Sie in dieser Übung den Zwei-Buchstaben-Schlüssel zum tatsächlichen Namen für den Projektfortschrittsstatus, den Sie in einer E-Mail versenden möchten.

![Umschaltfunktion Bild 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Zu befolgende Schritte

1. Klonen Sie das Szenario mit dem Namen „Freigeben von Variablen zwischen Routing-Pfaden“.
1. Nennen Sie das neue Szenario „Freigeben von Variablen zwischen Routing-Pfaden – Umschalten“.
1. Klicken Sie auf das Trigger-Modul und fügen Sie den Fortschrittsstatus in den Ausgabeabschnitt ein.
1. Fügen Sie im Modul „E-Mail senden“ dem Inhaltsfeld „Fortschrittsstatus“ hinzu.

   + Wenn Sie einfach den Wert aus dem Suchmodul anwenden, gibt es einen zweibuchstabigen Code für den Fortschrittsstatus.
   + Um den Code für den vollständigen Namen jedes möglichen Fortschrittsstatus „umzuschalten“, verwenden Sie die Funktion „Umschalten“ auf der Registerkarte „Allgemeine Funktionen“.

1. Die Umschaltfunktion verwendet den Wert oder Ausdruck des Fortschrittsstatus als Schlüssel und gibt dann den auf diesem Schlüssel basierenden Ausgabewert zurück.

   + An der ersten Stelle nach dem Fortschrittsstatus („VS“) wird ein Schlüsselwert definiert, an der zweiten Stelle die entsprechende Ausgabe („Verspätet“).
   + An dritter Stelle wird der nächste Schlüsselwert definiert, an vierter Stelle die entsprechende Ausgabe usw., und zwar für so viele Schlüssel wie gewünscht.

     ![Umschaltfunktion Bild 2](../12-exercises/assets/switch-function-walkthrough-2.png)

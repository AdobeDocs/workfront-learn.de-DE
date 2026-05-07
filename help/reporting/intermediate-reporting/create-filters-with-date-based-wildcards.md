---
title: Erstellen von Filtern mit datumsbasierten Platzhaltern
description: Erfahren Sie, wie und wann datumsbasierte Platzhalter verwendet werden und wie Sie einen Filter basierend auf dem aktuellen Datum erstellen.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-06-27T00:00:00.000Z'
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:57:08.996Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 100%

---

# Erstellen von Filtern mit datumsbasierten Platzhaltern

In diesem Video lernen Sie Folgendes:

* Verwenden datumsbasierter Platzhalter
* Lernen Sie den Unterschied zwischen den beiden datumsbasierten Platzhaltern in Workfront kennen
* Hinzufügen eines datumsbasierten Platzhalters zu einem Filter
* Erstellen eines benutzerdefinierten Datums mithilfe von Platzhaltern, Attributen, Operatoren und Modifikatoren
* Erstellen eines benutzerdefinierten Datumsbereichs mithilfe von Platzhaltern

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on&enablevpops=0)


## Aktivitäten zum Erstellen von Filtern mit datumsbasierten Platzhaltern


### Aktivitätsfragen

1. Wie würden Sie die Filterregel erstellen, wenn Sie nach Ausgaben suchen, deren Fälligkeitsdatum gestern oder heute ist?
1. Wie würden Sie die Filterregel erstellen, um nach Projekten zu suchen, die letzte Woche fällig waren?
1. Folgende Filterregeln sind Teil eines Aufgabenberichts, den Sie regelmäßig verwenden. Welche Art von Ergebnissen würden Sie mit diesem Bericht erzielen?

![Ein Screenshot des Bildschirms zum Erstellen eines Aufgabenfilters mit einem datumsbasierten Platzhalter](assets/date-wildcard-answer-1.png)

### Antworten

1. Filtern nach dem geplanten Fertigstellungsdatum der Ausgabe zwischen [!UICONTROL $$TODAY-1d] und [!UICONTROL $$TODAY].
1. Filtern nach dem geplanten Fertigstellungsdatum des Projekts zwischen [!UICONTROL $$TODAYb-1w] und [!UICONTROL $$TODAYe-1w].
1. In diesem Bericht werden die Ihnen zugewiesenen Aufgaben angezeigt, die noch nicht abgeschlossen sind (d. h. deren Fertigstellungsgrad unter 100 % liegt) und die überfällig oder heute fällig sind. Die Filterregel für das geplante Fertigstellungsdatum der Aufgaben besagt, dass nach Aufgaben mit einem Fälligkeitsdatum vor oder gleich dem heutigen Datum gesucht werden soll.

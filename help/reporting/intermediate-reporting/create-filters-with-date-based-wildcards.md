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
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 70%

---

# Erstellen von Filtern mit datumsbasierten Platzhaltern

In diesem Video lernen Sie Folgendes:

* Verwenden datumsbasierter Platzhalter
* Verstehen Sie den Unterschied zwischen den beiden datumsbasierten Platzhaltern von Workfront
* Hinzufügen eines datumsbasierten Platzhalters zu einem Filter
* Erstellen eines benutzerdefinierten Datums mithilfe von Platzhaltern, Attributen, Operatoren und Modifikatoren
* Erstellen eines benutzerdefinierten Datumsbereichs mithilfe von Platzhaltern

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)


## Aktivitäten vom Typ „Filter mit datumsbasierten Platzhaltern erstellen“


### Aktivitätsfragen

1. Wie würden Sie die Filterregel erstellen, wenn Sie nach Ausgaben suchen, deren Fälligkeitsdatum gestern oder heute ist?
1. Wie würden Sie die Filterregel erstellen, um nach Projekten zu suchen, die letzte Woche fällig waren?
1. Folgende Filterregeln sind Teil eines Aufgabenberichts, den Sie regelmäßig verwenden. Welche Art von Ergebnissen würden Sie mit diesem Bericht erzielen?

![Ein Screenshot des Bildschirms zum Erstellen eines Aufgabenfilters mit einem datumsbasierten Platzhalter](assets/date-wildcard-answer-1.png)

### Antworten

1. Filtern nach dem geplanten Fertigstellungsdatum der Ausgabe zwischen [!UICONTROL $$TODAY-1d] und [!UICONTROL $$TODAY].
1. Filtern nach dem geplanten Fertigstellungsdatum des Projekts zwischen [!UICONTROL $$TODAYb-1w] und [!UICONTROL $$TODAYe-1w].
1. Dieser Bericht findet Aufgaben, die Ihnen zugewiesen wurden und noch nicht abgeschlossen sind (d. h. einen Prozentsatz von weniger als 100 abgeschlossen haben) und die heute überfällig oder fällig sind. Die Filterregel für das geplante Abschlussdatum der Aufgaben besagt, dass Aufgaben mit einem Fälligkeitsdatum, das dem heutigen Datum entspricht oder vor diesem liegt, betrachtet werden sollen.

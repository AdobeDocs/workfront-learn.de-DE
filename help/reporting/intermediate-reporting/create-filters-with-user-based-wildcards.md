---
title: Erstellen von Filtern mit benutzerbasierten Platzhaltern
description: Erfahren Sie, wie Sie benutzerbasierte Platzhalter verwenden und wie Sie einen Filter auf der Grundlage der angemeldeten Person erstellen können.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 48%

---

# Erstellen von Filtern mit benutzerbasierten Platzhaltern

In diesem Video lernen Sie Folgendes:

* Grundlegendes dazu, warum Platzhalter verwendet werden
* Erstellen eines Filters mit einem benutzerbasierten Platzhalter

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Verwenden Sie beim Erstellen von Filtern, die sich mit Aufgaben- oder Problemzuweisungsinformationen beschäftigen, die Option „Arbeitsauftrag – Benutzer“ >> „ID-Feldquelle und -Name“. Diese Option berücksichtigt alle   Benutzende, die der Aufgabe oder dem Problem zugewiesen sind, nicht nur der „Inhaber“ oder der primäre Zugewiesene.

>[!TIP]
>
>Verwenden Sie die $$USER.ID (statt Ihres Namens), selbst dann, wenn Sie Filter für sich selbst erstellen. Auf diese Weise ist der Filter bereits eingerichtet, sodass jede Person, die den Filter verwendet, ihre eigenen Informationen sieht, wenn jemand einen Filter sieht, den Sie gerade verwenden, und sagt „Teilen Sie ihn mit mir“.

>[!TIP]
>
>Bei der Verwendung von benutzerbasierten Platzhaltern müssen Sie immer den Filterqualifizierer „Gleich“ verwenden.


## Erstellen von Filtern mit benutzerbasierten Platzhalteraktivitäten

Klicken Sie [hier](/help/assets/create-filters-with-user-based-wildcards-activities.pdf), um eine PDF-Datei dieser Seite herunterzuladen.

### Aktivität 1

Diese Woche haben Sie etwas mehr Zeit. Sie möchten also herausfinden, ob es jemanden in Ihrem Team gibt, der Unterstützung bei seinen Aufgaben benötigen könnte. Erstellen Sie einen Aufgabenfilter , um Aufgaben zu finden, die für diese Woche fällig sind und noch nicht abgeschlossen wurden.

### Antwort 1

Du bist großartig, wenn du deinen Teamkollegen hilfst! Wenn der Filter wie im folgenden Bild eingerichtet ist, finden Sie Aufgaben:

* die nicht abgeschlossen wurden (was bedeutet, dass sie keinen Status [!UICONTROL Abgeschlossen] oder Status haben, der &quot;[!UICONTROL &quot; ];
* die in Projekten mit dem [!UICONTROL Aktuell]-Status enthalten sind (schließlich möchten Sie keine Aufgaben für Projekte finden, die noch nicht gestartet wurden);
* Aufgaben, die einer Person in Ihrem Stamm-Team zugewiesen wurden, wie in den Team-Einstellungen von Workfront definiert;
* und ein Abschlussdatum irgendwann in dieser Woche haben (diese Regel verwendete den vordefinierten Datumsfilter, um „diese Woche“ zu definieren).

![Ein Screenshot des Bildschirms zum Erstellen eines Aufgabenfilters mit einem benutzerbasierten Platzhalter](assets/user-wildcard-exercise-answer.png)

Möglicherweise müssen Sie zusätzliche Filter hinzufügen, wenn Sie die Liste noch weiter einschränken möchten. Sie können zum Beispiel eine Filterregel hinzufügen, die ein bestimmtes Programm oder Portfolio berücksichtigt, in dem Ihr Team arbeitet.

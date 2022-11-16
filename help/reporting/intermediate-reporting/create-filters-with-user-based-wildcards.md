---
title: Erstellen von Filtern mit benutzerdefinierten Platzhaltern
description: Erfahren Sie, wie Sie benutzerbasierte Platzhalter verwenden und wie Sie einen Filter basierend auf dem angemeldeten Benutzer erstellen.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Erstellen von Filtern mit benutzerdefinierten Platzhaltern

In diesem Video erfahren Sie, wie Sie:

* Gründe für die Verwendung von Platzhaltern
* Erstellen eines Filters mit einem benutzerbasierten Platzhalter

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Verwenden Sie beim Erstellen von Filtern, die sich mit Aufgaben- oder Problemzuweisungsinformationen beschäftigen, die Quelle und den Namen des Felds Zuweisen > ID .  Bei dieser Option werden alle der Aufgabe oder dem Problem zugewiesenen Benutzer berücksichtigt, nicht nur der &quot;Eigentümer&quot;oder der primäre Verantwortliche.

>[!TIP]
>
>Verwenden Sie die $$USER.ID (anstelle Ihres Namens) auch beim Erstellen von Filtern für sich selbst. Auf diese Weise wird der Filter bereits eingerichtet, wenn jemand einen Filter sieht, den Sie verwenden, und &quot;Für mich freigeben&quot;sagt, sodass jede Person, die ihn verwendet, ihre eigenen Informationen sieht.

>[!TIP]
>
>Sie müssen bei der Verwendung benutzerdefinierter Platzhalter immer den Filter Gleich verwenden.

## Aktivität

Sie haben diese Woche etwas mehr Zeit, also möchten Sie sehen, ob jemand in Ihrem Team etwas Hilfe bei der Aufgabenstellung verwenden kann. Erstellen Sie einen Aufgabenfilter, um Aufgaben zu finden, die in dieser Woche fällig und noch nicht abgeschlossen sind.

## Antwort

Du bist fantastisch für deine Teamkollegen! Wenn der Filter wie das folgende Bild eingerichtet ist, finden Sie Aufgaben:

* Das ist noch nicht abgeschlossen (d. h. sie haben keine [!UICONTROL Fertig] Status oder Status, der [!UICONTROL Fertig]);
* In Projekten mit einer [!UICONTROL Aktuell] -Status (schließlich möchten Sie keine Aufgaben für Projekte finden, die noch nicht gestartet wurden);
* die einer Person in Ihrem Startseiten-Team zugewiesen werden, wie in den Workfront-Teameinstellungen definiert;
* Und die ein Abschlussdatum haben, an dem diese Woche etwas Zeit hat (diese Regel verwendet den vordefinierten Datumsfilter, um &quot;diese Woche&quot;zu definieren).

![Ein Bild des Bildschirms zum Erstellen eines Aufgabenfilters mit einem benutzerbasierten Platzhalter](assets/user-wildcard-exercise-answer.png)

Möglicherweise müssen Sie weitere Filter hinzufügen, um die Liste noch etwas zu beschränken. Sie können beispielsweise eine Filterregel hinzufügen, die sich auf ein bestimmtes Programm oder Portfolio bezieht, aus dem Ihr Team ausgeht.

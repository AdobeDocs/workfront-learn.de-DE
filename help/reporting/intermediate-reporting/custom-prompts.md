---
title: Erstellen von benutzerdefinierten Eingabeaufforderungen im Textmodus
description: Erfahren Sie, was ein benutzerdefinierter Prompt ist, wie Sie ihn im Textmodus erstellen, und einige Beispiele, die Sie im Berichtswesen in Workfront verwenden können.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-05T00:00:00Z
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 94%

---

# Erstellen von benutzerdefinierten Eingabeaufforderungen im Textmodus

In diesem Video lernen Sie Folgendes:

* Was ist ein benutzerdefinierter Prompt?
* Erstellen eines benutzerdefinierten Prompts im Textmodus
* Einige Beispiele, die Sie in Ihren Berichten verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0)

## Aktivitäten zum Erstellen benutzerdefinierter Prompts


### Aktivität: Benutzerdefinierte Prompts erstellen

1. Erstellen Sie einen benutzerdefinierten Prompt, der folgende Projektstatus im Dropdown-Menü der Eingabeaufforderung anzeigt:
   * In Planung
   * Aktuell
   * Abgeschlossen
   * Eingestellt
1. Ändern Sie den Prompt so, dass aktuelle Projekte angezeigt werden, die in diesem Monat fällig sind.

### Antworten

1. Ihre benutzerdefinierten Prompts sollten in etwa wie folgt aussehen und folgenden Textmodus aufweisen:

   ![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-01.png)

   Nachdem Sie den benutzerdefinierten Prompt gespeichert haben, sollte das Dropdown-Menü für den Prompt wie folgt aussehen:

1. Der Textmodus in Ihrem benutzerdefinierten Prompt sollte wie folgt aussehen:

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Außerdem sollte die Dropdown-Beschriftung für aktive Prompts aktualisiert werden, um die Code-Änderung wie folgt widerzuspiegeln:

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02a.png)

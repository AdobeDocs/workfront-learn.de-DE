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
last-substantial-update: '2025-08-05T00:00:00.000Z'
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:55.263Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 207
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

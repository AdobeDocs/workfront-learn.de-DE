---
title: Erstellen benutzerdefinierter Eingabeaufforderungen
description: Erfahren Sie, was eine benutzerdefinierte Eingabeaufforderung ist, wie Sie sie im Textmodus erstellen, und einige Beispiele, die Sie im Berichtswesen in Workfront verwenden können.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: f03518b568cc24ad39b32f6dbfd763400529cf0f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 100%

---

# Erstellen benutzerdefinierter Eingabeaufforderungen

In diesem Video lernen Sie Folgendes:

* Was ist eine benutzerdefinierte Eingabeaufforderung?
* Erstellen einer benutzerdefinierten Eingabeaufforderung im Textmodus
* Einige Beispiele, die Sie in Ihren Berichten verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Aktivitäten zum Erstellen benutzerdefinierter Eingabeaufforderungen


### Aktivität: Benutzerdefinierte Eingabeaufforderungen erstellen

1. Erstellen Sie eine benutzerdefinierte Eingabeaufforderung, die folgende Projektstatus im Dropdown-Menü der Eingabeaufforderung anzeigt:
   * In Planung
   * Aktuell
   * Abgeschlossen
   * Eingestellt
1. Ändern Sie die Eingabeaufforderung so, dass aktuelle Projekte angezeigt werden, die in diesem Monat fällig sind.

### Antworten

1. Ihre benutzerdefinierten Eingabeaufforderungen sollten in etwa wie folgt aussehen und folgenden Textmodus aufweisen:

   ![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-01.png)

   Nachdem Sie die benutzerdefinierte Eingabeaufforderung gespeichert haben, sollte das Dropdown-Menü für die Eingabeaufforderung wie folgt aussehen:

1. Der Textmodus in Ihrer benutzerdefinierten Eingabeaufforderung sollte wie folgt aussehen:

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Außerdem sollte die Dropdown-Beschriftung für aktive Eingabeaufforderungen aktualisiert werden, um die Code-Änderung wie folgt widerzuspiegeln:

![Ein Screenshot des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02a.png)

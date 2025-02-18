---
title: Erstellen benutzerdefinierter Eingabeaufforderungen
description: Erfahren Sie, was eine benutzerdefinierte Eingabeaufforderung ist, wie Sie sie im Textmodus erstellen, und einige Beispiele, die Sie im Berichtswesen in Workfront verwenden können.
activity: use
feature: Text Mode Reporting
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 98%

---

# Erstellen benutzerdefinierter Eingabeaufforderungen

In diesem Video lernen Sie Folgendes:

* Was ist eine benutzerdefinierte Eingabeaufforderung?
* Erstellen einer benutzerdefinierten Eingabeaufforderung im Textmodus
* Einige Beispiele, die Sie in Ihren Berichten verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Erstellen benutzerdefinierter Eingabeaufforderungsaktivitäten

Klicken Sie [hier](/help/assets/create-custom-prompts-activities.pdf), um eine PDF-Datei dieser Seite herunterzuladen.

## Aktivität: Benutzerdefinierte Eingabeaufforderungen erstellen

1. Erstellen Sie eine benutzerdefinierte Eingabeaufforderung, die folgende Projektstatus im Dropdown-Menü der Eingabeaufforderung anzeigt:
   * In Planung
   * Aktuell
   * Abgeschlossen
   * Eingestellt
1. Ändern Sie die Eingabeaufforderung so, dass aktuelle Projekte angezeigt werden, die in diesem Monat fällig sind.

## Antworten

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

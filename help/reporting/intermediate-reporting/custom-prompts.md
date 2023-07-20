---
title: Benutzerdefinierte Eingabeaufforderungen erstellen
description: Erfahren Sie, was eine benutzerdefinierte Eingabeaufforderung ist, wie Sie eine benutzerdefinierte Eingabeaufforderung im Textmodus erstellen, und einige Beispiele, die Sie für die Berichterstellung in Workfront verwenden können.
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
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# Benutzerdefinierte Eingabeaufforderungen erstellen

In diesem Video erfahren Sie:

* Was ist eine benutzerdefinierte Eingabeaufforderung?
* Erstellen einer benutzerdefinierten Eingabeaufforderung im Textmodus
* Einige Beispiele, die Sie in Ihren Berichten verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Aktivität: Benutzerdefinierte Eingabeaufforderungen erstellen

1. Erstellen Sie eine benutzerdefinierte Eingabeaufforderung, die die folgenden Projektstatus im Eingabeaufforderungs-Dropdown-Menü anzeigt:
   * In Planung
   * Aktuell
   * Abgeschlossen
   * Eingestellt
1. Ändern Sie die Aufforderung, aktuelle Projekte anzuzeigen, die in diesem Monat anstehen.

## Antworten

1. Ihre benutzerdefinierten Eingabeaufforderungen sollten in etwa wie folgt aussehen und den folgenden Textmodus aufweisen:

   ![Ein Bild des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-01.png)

   Nachdem Sie die benutzerdefinierte Eingabeaufforderung gespeichert haben, sollte das Dropdown-Menü für die Eingabeaufforderung wie folgt aussehen:

1. Der Textmodus in Ihrer benutzerdefinierten Eingabeaufforderung sollte wie folgt aussehen:

![Ein Bild des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Außerdem sollte die Dropdown-Bezeichnung für aktive Eingabeaufforderungen aktualisiert werden, um die Änderung im Code wie folgt widerzuspiegeln:

![Ein Bild des Bildschirms zum Erstellen eines neuen Filters im Textmodus](assets/cp-02a.png)

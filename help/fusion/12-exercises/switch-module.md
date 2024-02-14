---
title: Schaltmodul-Übung
description: Erfahren Sie, wie Sie das Switch-Modul verwenden können, um komplexere oder dynamische Datentransformationen durchzuführen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,noCatalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 98%

---

# Schaltmodul-Übung

Erfahren Sie, wie Sie das Switch-Modul verwenden können, um komplexere oder dynamische Datentransformationen durchzuführen.

## Übungsübersicht

Suchen Sie nach Briefpost-Projekten auf Ihrem Testlaufwerk und ändern Sie den Namen jedes Projekts anhand eines Werts, der in einem benutzerdefinierten, dem Projekt zugeordneten Feld ausgewählt wurde.

![Switch-Modul Bild 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Zu befolgende Schritte

1. Erstellen Sie ein neues Szenario und nennen Sie es „Verwendung des Switch-Moduls“.
1. Verwenden Sie für das Trigger-Modul das Workfront-Suchmodul.
1. Richten Sie Ihre Workfront-Verbindung ein und setzen Sie den Eintragstyp auf „Projekt“.
1. Geben Sie in den Suchkriterien an, dass nur Projekte mit einem Wert im benutzerdefinierten Feld „Kanal“ angezeigt werden sollen.
1. Wählen Sie als Ausgaben ID, Name, Referenznummer und das benutzerdefinierte Feld „Kanal“.

   ![Switch-Modul Bild 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Fügen Sie das Switch-Modul aus der Option „Tools“ hinzu.
1. Weisen Sie für das Eingabefeld das benutzerdefinierte Feld „Kanal“ aus dem Suchmodul zu.

   ![Switch-Modul Bild 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Fügen Sie als Nächstes Fälle für jeden möglichen Wert aus dem benutzerdefinierten Feld „Kanal“ hinzu. Der mögliche Wert wird in das Feld „Muster“ eingetragen. Sie können festlegen, dass das Ausgabefeld einen spezifischen 3 Zeichen langen Code enthält, gefolgt von der Projektreferenznummer und dem Projektnamen.

   **Ihr Zuordnungsfenster sollte wie folgt aussehen:**

   ![Switch-Modul Bild 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Sie können beliebig viele zusätzliche Fälle hinzufügen. Beachten Sie das Feld „Sonst“ am unteren Rand. Dies wird verwendet, wenn der Eingabewert mit keinem der Fälle übereinstimmt.

   **Aktualisieren Sie den Projektnamen in Workfront.**

   ![Switch-Modul Bild 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Fügen Sie ein Workfront-Modul zum Aktualisieren von Datensätzen hinzu.
1. Weisen Sie im ID-Feld die ID des Trigger-Moduls zu.
1. Setzen Sie den Eintragstyp auf „Projekt“.
1. Wählen Sie das Feld „Name“ aus dem Abschnitt „Zuzuordnende Felder auswählen“ und weisen Sie es der Ausgabe des Switch-Moduls zu.
1. Speichern Sie Ihr Szenario und führen Sie es einmal aus. Sehen Sie sich die aktualisierten Projektnamen auf Ihrem Testlaufwerk an.

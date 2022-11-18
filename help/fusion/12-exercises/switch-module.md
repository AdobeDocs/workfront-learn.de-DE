---
title: Switch-Modul
description: Erfahren Sie, wie Sie das Switch-Modul verwenden, wenn Sie komplexere oder dynamischere Datenumwandlungen durchführen müssen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Switch-Modul

Erfahren Sie, wie Sie das Switch-Modul verwenden, wenn Sie komplexere oder dynamischere Datenumwandlungen durchführen müssen.

## Übungsübersicht

Suchen Sie in Ihrem Testlaufwerk nach Briefpost-Projekten und ändern Sie dann den Namen jedes Projekts basierend auf einem Wert, der in einem benutzerdefinierten Feld ausgewählt ist, das an das Projekt angehängt ist.

![Switch-Modul Bild 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Erstellen Sie ein neues Szenario und nennen Sie es &quot;Verwendung des Switch-Moduls&quot;.
1. Verwenden Sie für das Trigger-Modul das Workfront-Suchmodul.
1. Richten Sie Ihre Workfront-Verbindung ein und legen Sie den Datensatztyp auf Projekt fest.
1. Geben Sie in den Suchkriterien an, dass nur Projekte mit einem Wert im benutzerdefinierten Feld Kanal angezeigt werden sollen.
1. Wählen Sie für Ausgaben ID, Name, Referenznummer und das benutzerdefinierte Feld Kanal aus.

   ![Switch-Modul Bild 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Fügen Sie das Switch-Modul aus Tools hinzu.
1. Mappen Sie für das Eingabefeld das benutzerdefinierte Feld Kanal aus dem Suchmodul.

   ![Switch-Modul Bild 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Als Nächstes fügen Sie Fälle für jeden möglichen Wert hinzu, der aus dem benutzerdefinierten Feld Kanal stammt. Der mögliche Wert wird im Feld Muster angegeben. Sie möchten, dass das Ausgabefeld einen bestimmten 3-Buchstaben-Code gefolgt von der Referenznummer des Projekts und dann dem Projektnamen enthält.

   **Ihr Zuordnungsbereich sollte wie folgt aussehen:**

   ![Switch-Modul Bild 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Sie können beliebig viele weitere Fälle hinzufügen. Beachten Sie das Feld Else unten. Dies wird verwendet, wenn der Eingabewert keinem der Fälle entspricht.

   **Aktualisieren Sie den Projektnamen in Workfront.**

   ![Switch-Modul Bild 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Fügen Sie ein Workfront-Modul zum Aktualisieren von Datensätzen hinzu.
1. Ordnen Sie im Feld ID die ID aus dem Trigger-Modul zu.
1. Setzen Sie den Record Type auf Project.
1. Wählen Sie im Abschnitt Zu zuordnende Felder auswählen das Feld Name aus und ordnen Sie es der Ausgabe des Switch-Moduls zu.
1. Speichern Sie das Szenario und führen Sie es einmal aus. Zeigen Sie die aktualisierten Projektnamen in Ihrem Testlaufwerk an.

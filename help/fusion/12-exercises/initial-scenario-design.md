---
title: Übung zu ursprünglichem Szenario-Design
description: Hier erhalten Sie einige grundlegende Navigationstipps für die erste Anmeldung bei Workfront Fusion sowie die Erstellung Ihres ersten Szenarios.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
last-substantial-update: 2025-06-02T00:00:00Z
recommendations: noDisplay,catalog
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: 64b23532fba54ac1fbfba807e4b6f0490bfca631
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 97%

---

# Übung zu ursprünglichem Szenario-Design

Hier erhalten Sie einige grundlegende Navigationstipps für die erste Anmeldung bei Workfront Fusion sowie die Erstellung Ihres ersten Szenarios.

## Voraussetzungen

1. Für diese Übung ist ein Workfront-Testlaufwerk erforderlich. Sie können eins anfordern, indem Sie [dieses Formular](https://forms.office.com/r/f1J8HRGrNY) ausfüllen. Wenn Sie nicht auf das Formular zugreifen können, senden Sie Ihren Namen, Ihre E-Mail-Adresse und Ihren Firmennamen an wfttstdr@adobe.com.
1. Bei Fusion-Übungen wird davon ausgegangen, dass Sie das Erläuterungsvideo zur entsprechenden Übung angesehen haben. In diesem Fall ist es [Anleitung zum anfänglichen Szenario-Design](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/understand-the-basics/initial-scenario-design-walkthrough.html?lang=de).


## Übungsübersicht

Erstellen Sie für jede Zeile in der CSV-Datei der Projektliste ein neues Projekt in Workfront.

![Ursprüngliches Szenario-Design Bild 1](../12-exercises/assets/initial-scenario-design-1.png)

## Zu befolgende Schritte

1. Erstellen Sie im Abschnitt „Szenario“ einen Ordner mit dem Namen „Fusion-Aktivierungsübung“.
1. Klicken Sie in den Ordner und dann auf „Neues Szenario erstellen“.

   ![Ursprüngliches Szenario-Design Bild 2](../12-exercises/assets/initial-scenario-design-2.png)

1. Suchen Sie auf der nächsten Seite nach Workfront und wählen Sie diese Anwendung aus. Klicken Sie dann auf „Weiter“.
1. Benennen Sie oben links im Bildschirm „Szenario-Designer“ Ihr Szenario in „Anfängliches Szenario-Design“ um
1. Klicken Sie auf das leere Trigger-Modul in der Mitte des Bildschirms und wählen Sie die Workfront-App und dann das Modul „Dokument herunterladen“ aus.

   **Authentifizieren Sie die Verbindung des Moduls zu Ihrem Workfront-Konto.**

1. Um zum ersten Mal eine Verbindung zu erstellen, klicken Sie auf die Schaltfläche „Hinzufügen“.

   ![Ursprüngliches Szenario-Design Bild 3](../12-exercises/assets/initial-scenario-design-3.png)

1. Geben Sie der Verbindung einen Namen, z. B. „Mein Workfront 2020“.

   ![Ursprüngliches Szenario-Design Bild 4](../12-exercises/assets/initial-scenario-design-4.png)

1. Geben Sie die URL **Ihres Testlaufwerkkontos für Workfront** ein und klicken Sie dann auf Weiter.

   ![Ursprüngliches Szenario-Design Bild 5](../12-exercises/assets/initial-scenario-design-5.png)

1. Geben Sie Ihr Kennwort ein und klicken Sie auf „Anmelden“.

   **Die Verbindung wird hergestellt. Geben Sie nun die ID des Dokuments ein, das Sie aus Workfront herunterladen möchten.**

   ![Ursprüngliches Szenario-Design Bild 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Gehen Sie zurück zu Workfront. Wählen Sie im Ordner „Fusion-Übungsdateien“ die Datei „_Fusion2020_Project List.csv“ aus und klicken Sie im linken Bedienfeld auf „Dokumentdetails“. Kopieren Sie die Dokument-ID aus der URL-Adresse (dies ist die erste lange Nummer in der URL).

   ![Ursprüngliches Szenario-Design Bild 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Gehen Sie zurück zu Fusion, fügen Sie die Nummer in das Feld „Dokument-ID“ ein und klicken Sie auf „OK“.
1. Es ist eine Best Practice, Module bei ihrer Erstellung umzubenennen. Machen Sie dazu einen Rechtsklick auf das Workfront-Modul und wählen Sie „Umbenennen“. Nennen Sie das Modul „Projektliste abrufen“.

   **Als Nächstes werden Sie die soeben heruntergeladene CSV-Datei analysieren, damit Sie auf jede Zeile der Datei zugreifen können. Anhand dieser Informationen werden Sie ein Projekt aus jeder Zeile erstellen.**

1. Klicken Sie auf die rechte Seite des Workfront-Moduls, um ein weiteres Modul hinzuzufügen. Suchen Sie nach der CSV-App und wählen Sie das Modul „CSV-Analyse“ aus.
1. Richten Sie die CSV-Analyse mit 6 Spalten, in CSV enthaltenen Kopfzeilen und kommagetrenntem Inhalt ein und geben Sie Daten in das CSV-Feld ein. Klicken Sie dann auf „OK“.

   ![Ursprüngliches Szenario-Design Bild 9](../12-exercises/assets/initial-scenario-design-9.png)

1. Benennen Sie dieses Modul in „Analyseprojektliste“ um.
1. Klicken Sie unten im Szenario-Designer auf „Speichern“, um Ihr Szenario zu speichern.
1. Klicken Sie auf „Einmal ausführen“, um die Ausgabe anzuzeigen.

   >[!NOTE]
   >
   >Ignorieren Sie die Warnung, dass ein Transformator nicht das letzte Modul sein sollte (das stimmt zwar, spielt aber für diesen Test keine Rolle). Klicken Sie auf „Trotzdem ausführen“.

   ![Ursprüngliches Szenario-Design Bild 10](../12-exercises/assets/initial-scenario-design-10.png)

1. Öffnen Sie den Ausführungsinspektor des Moduls „CSV-Analyse“, um die Ein- und Ausgaben des Moduls anzuzeigen. Es gibt ein Bündel (eine CSV-Datei) als Eingabe und mehrere Bündel als Ausgabe (ein Bündel für jede Zeile in der CSV-Datei). Sie sollte in etwa so aussehen:

   ![Ursprüngliches Szenario-Design Bild 11](../12-exercises/assets/initial-scenario-design-11.png)

   **Fügen Sie ein Modul hinzu, um ein Projekt für jede Zeile in der CSV-Datei zu erstellen.**

1. Fügen Sie ein weiteres Modul hinzu. Wählen Sie die Workfront-App aus und dann das Modul „Eintrag erstellen“.
1. Legen Sie als Eintragstyp „Projekt“ fest.

   >[!TIP]
   >
   >Suchen Sie danach, indem Sie einige Buchstaben eingeben, z. B. *proj*, um direkt darauf zuzugreifen.

1. Verwenden Sie dann Cmd/Strg+G, um nach dem Namen (Projektnamen) zu suchen. Markieren Sie das Kontrollkästchen neben „Name“. Das Feld erscheint jetzt darunter.
1. Kreuzen Sie nun die Kontrollkästchen neben „Geplanter Starttermin“ und „Priorität“ an.
1. Klicken Sie in das Feld „Name“, um das Zuordnungsfenster zu öffnen. Klicken Sie auf das Feld „Spalte 1“ im Modul „CSV-Analyse“, um es zum Feld „Name“ hinzuzufügen. Dies ist der Projektname aus der CSV-Datei.
1. Klicken Sie unter „Geplantes Startdatum“ auf „Spalte 5“ im Modul „CSV-Analyse“.
1. Wählen Sie unter „Priorität“ aus dem Dropdown-Menü „Normal“.

   **Ihr Zuordnungsfenster sollte wie folgt aussehen:**

   ![Ursprüngliches Szenario-Design Bild 12](../12-exercises/assets/initial-scenario-design-12.png)

1. Klicken Sie auf „OK“.

   >[!NOTE]
   >
   >Wenn Sie nicht auf „OK“, sondern versehentlich zurück in den Designer klicken, wird Ihre Arbeit nicht gespeichert und Sie müssen die Zuordnung erneut vornehmen.

1. Machen Sie einen Rechtsklick auf das Workfront-Modul und benennen Sie es um in „Workfront-Projekte erstellen“.
1. Speichern Sie Ihr Szenario und klicken Sie auf die Schaltfläche „Einmal ausführen“.
1. Klicken Sie auf den Ausführungsinspektor oben rechts im letzten Modul.

   + Sie werden sehen, dass 20 Vorgänge ausgeführt wurden. Für jeden Vorgang wurde ein Bündel, d. h. eine Zeile, aus der CSV-Datei als Eingabe benutzt und ein Bündel aus Ausgabe, d. h. ein in Workfront erstelltes Projekt. Die Projekt-ID des erstellten Projekts wird mit dem Ausgabe-Bündel angezeigt.

   ![Ursprüngliches Szenario-Design Bild 13](../12-exercises/assets/initial-scenario-design-13.png)

   **Verwenden von Notizen**

1. Notizen tragen dazu bei, das Szenario-Design transparenter zu machen. Um zum Modul „Workfront-Projekte erstellen“ eine Notiz hinzuzufügen, machen Sie einen Rechtsklick und wählen Sie „Notiz hinzufügen“. Auf der rechten Seite des Designer-Fensters öffnet sich ein Fenster, in dem Sie eine Notiz zum Modul hinzufügen können. Geben Sie „Erstellen eines Projekts mit Name, geplantem Startdatum und Priorität aus der CSV-Datei“ ein.
1. Fügen Sie eine weitere Notiz hinzu, um zu beschreiben, was das Trigger-Modul (das erste Workfront-Modul) tut.
1. Schließen Sie das Notizenfeld, indem Sie auf das X oben rechts klicken.

   + Greifen Sie erneut auf die Notizen zu, indem Sie auf die Schaltfläche „Notizen“ in der unteren Symbolleiste oder mit der rechten Maustaste auf ein beliebiges Modul klicken und eine neue Notiz hinzufügen.
   + Die Notizen sind in chronologischer Reihenfolge sortiert.
   + Sobald Notizen hinzugefügt wurden, wird ein orangefarbener Punkt auf der Schaltfläche „Notizen“ angezeigt.

   ![Ursprüngliches Szenario-Design Bild 14](../12-exercises/assets/initial-scenario-design-14.png)

1. Speichern Sie das Szenario, indem Sie in der Symbolleiste der Steuerelemente auf „Speichern“ klicken.
1. Sie können die in Ihrer Workfront-Instanz erstellten Projekte anzeigen.

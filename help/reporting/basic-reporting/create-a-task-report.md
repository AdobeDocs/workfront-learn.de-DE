---
title: Erstellen eines Aufgabenberichts
description: In diesem Video erfahren Sie, wie Sie einen Aufgabenbericht mit einem komplexen Filter in Workfront erstellen und die von Ihnen erstellten Berichte finden. Aktivität – einen Notizbericht mit Eingabeaufforderungen erstellen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 0f2a8c6855398759890fad1282ced3c28615f7f5
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 40%

---

# Erstellen eines Aufgabenberichts

In diesem Video lernen Sie Folgendes:

* Erstellen eines Aufgabenberichts mit einem komplexen Filter
* Suchen nach den von Ihnen erstellten Berichten

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)



>[!TIP]
>
>Brechen Sie Ihre Spatulas aus und mischen Sie Ihre Schüsseln und bereiten Sie sich darauf vor, die &quot;Rezepte&quot; in unserem [Adobe Workfront Customer Reporting-Cookie](/help/assets/workfront-customer-reporting-cookbook.pdf). Im Inneren finden Sie Schritt-für-Schritt-Anweisungen für 10 Berichte, die Ihnen heute in Ihrer Umgebung zur Verfügung stehen.
><br>
>Wir haben Lieblingsberichte von Kunden gesammelt und in einem kleinen, leicht verdaulichen Kochbuch zusammengestellt, in dem Sie Ihre Workfront-Küche wieder ausprobieren können.
><br>
>Diese 10 Berichte stammen von Kunden, die genau wie Sie sind. Verteilen wir uns über Branchen, Abteilungen, Teams, Positionen und alle in verschiedenen Unternehmen, schulden wir Ihnen ein großes Dankeschön an die unglaublichen Kunden, die einen ihrer Lieblingsberichte teilen. Einige Berichte sind einfach (aber unglaublich nützlich) und einige sind komplexer, um Ihre Berichterstellung auf die nächste Ebene zu bringen.



## Aktivität 1: Erstellen eines Berichts mit Eingabeaufforderungen

Erstellen Sie einen Notizbericht, mit dem Sie nach Benutzernotizen (d. h. Kommentaren oder Aktualisierungen) oder Systemnotizen auf Grundlage des Inhalts, der Autorin oder des Autors, des Eingabedatums, des Projektnamens oder der Überprüfungsart suchen können. Nennen Sie den Bericht &quot;Notizsuche&quot;.

Bei Verwendung der Eingabeaufforderung für den Notiztext sucht dieser Bericht in den Aktualisierungs-Threads, um schnell alle zu extrahieren, die den in den Eingabeaufforderungen angegebenen Kriterien entsprechen. Wenn Sie den Bericht ausführen, müssen Sie nicht jede Eingabeaufforderung ausfüllen, nur die, die Ihnen wichtig sind. Leere Felder werden automatisch ignoriert.

Die Ansicht sollte Spalten für Folgendes enthalten:

* Notiztext
* Audit-Text
* Eingabedatum
* Eigentümer: Name
* Prüfungstyp
* Aufgabenname
* Name des Problems

Lassen Sie die Registerkarte „Filter“ leer.

Gruppe zum Projektnamen.

Schließen Sie Aufforderungen zu Folgendem ein:

* Audit-Text
* Notiztext
* Name der Eigentümerin bzw. des Eigentümers
* Eingabedatum
* Projektname
* Prüfungstyp

## Antwort zu Aktivität 1

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf das Menü **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Notiz]**.
1. Unter **[!UICONTROL Spalten (Ansicht)]** können Sie Ihre Spalten einrichten:

   ![Ein Screenshot des Bildschirms zum Erstellen von Spalten für Notizberichte](assets/note-report-columns.png)

   * [!UICONTROL Notiz] > [!UICONTROL Notiztext]
   * [!UICONTROL Notiz] > [!UICONTROL Prüftext]
   * [!UICONTROL Notiz] > [!UICONTROL Eingabedatum]
   * [!UICONTROL Eigentümer] > [!UICONTROL Name]
   * [!UICONTROL Notiz] > [!UICONTROL Prüfungstyp]
   * [!UICONTROL Aufgabe] > [!UICONTROL Name]
   * [!UICONTROL Problem] > [!UICONTROL Name]

1. Wählen Sie die Spalte **[!UICONTROL Eingabedatum]** und ändern Sie die Option **[!UICONTROL Absteigend sortieren]**.
1. Legen Sie auf der Registerkarte **[!UICONTROL Gruppierungen]** fest, dass der Bericht nach [!UICONTROL Projekt] > [!UICONTROL Name] gruppiert werden soll.

   ![Ein Screenshot des Bildschirms zum Erstellen von Notizberichtsgruppierungen](assets/note-report-groupings.png)

1. Lassen Sie das Feld [!UICONTROL Filter] leer.
1. Öffnen **[!UICONTROL Berichtseinstellungen]** und benennen Sie den Bericht &quot;Notizsuche&quot;.
1. Im [!UICONTROL Beschreibung] -Feld ein, z. B. &quot;Suchen Sie basierend auf dem ausgewählten Audittyp und anderen Eingabeaufforderungen nach System- oder Benutzernotizen. Systemnotizen werden in der Spalte &quot;Audit Text&quot;und Benutzerhinweise in der Spalte Hinweis Text angezeigt.&quot;

   ![Ein Screenshot des Bildschirms zum Erstellen von Notizberichtseinstellungen](assets/note-report-report-options.png)

1. Wählen Sie die Registerkarte **[!UICONTROL Details]**, damit sie beim Laden des Berichts angezeigt wird.
1. Richten Sie den Bericht so ein, dass 200 Elemente angezeigt werden, wenn der Bericht in ein Dashboard aufgenommen wird.
1. Klicken Sie auf **[!UICONTROL Berichteingabeaufforderungen]** und fügen Sie Folgendes hinzu:

   ![Ein Screenshot des Bildschirms zum Erstellen von Notizberichts-Eingabeaufforderungen](assets/note-report-report-prompts.png)

   * [!UICONTROL Notiz] > [!UICONTROL Prüftext]
   * [!UICONTROL Notiz] > [!UICONTROL Notiztext]
   * [!UICONTROL Eigentümer] > [!UICONTROL Name]
   * [!UICONTROL Notiz] > [!UICONTROL Eingabedatum]
   * [!UICONTROL Projekt] > [!UICONTROL Name]
   * [!UICONTROL Notiz] > [!UICONTROL Prüfungstyp]

1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Eingabeaufforderungen in Dashboards anzeigen]**.
1. Speichern und schließen Sie den Bericht.

## Aktivität 2: Erstellen eines Feedback-Berichts für das Admin-Team

Dieser Problembericht zeigt alle Probleme aus einer Feedback-Anforderungswarteschlange an, die für Systemadministratoren erstellt wurde. Sie können sehen, wie Sie diese Anforderungswarteschlange in der [Erstellen einer Feedback-Anforderungswarteschlange für Systemadministratoren](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html) Tutorial.

Dieser Bericht verwendet auch ein benutzerdefiniertes Formular. Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Benutzerdefiniertes Formular erstellen und freigeben](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) Tutorial.

Dieses benutzerdefinierte Formular sollte wie folgt erstellt werden:

Name: Feedback zum Admin-Prozess

1. Prozesstyp (Dropdown-Feld)
   * Zugriffsstufen
   * Validierungsprozess (nur global)
   * E-Mail-Benachrichtigungen
   * Layoutvorlage
   * Milestone-Pfad
   * Projektvorlage
   * Erinnerungsbenachrichtigungen
   * Anforderungswarteschlange
1. Prozessname (einzeiliges Textfeld)
1. Prozessqualität (Dropdown-Feld)
   * 1 - völlig nutzlos
   * 2 - nicht sehr nützlich
   * 3 - gut, aber besser
   * 4 - hervorragend
1. Problem oder gute Nachrichten (Absatztextfeld)

Erstellen Sie einen Problembericht mit dem Namen **Feedback-Bericht des Administrators**.

Die Ansicht sollte die folgenden Spalten enthalten:

* Problem: Name
* Primärer Ansprechpartner: Name
* Problem: Prozesstyp
* Problem: Prozessname
* Problem: Process Grade
* Problem: Problem oder gute Nachrichten
* Problem: Eingangsdatum
* Problem: Alter
* Problem: Zuweisungen
* Problem: Status

Gruppe für den Prozesstyp.

Filtern Sie nach der ID des Anforderungswarteschlangenprojekts, in dem sich die Feedback-Probleme befinden.


![Ein Screenshot des Feedback-Berichts des Admin-Teams](assets/create-a-system-admin-feedback-request-queue.png)



## Antwort zu Aktivität 2

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf **[!UICONTROL Neuer Bericht]** Menü und wählen Sie **[!UICONTROL Problem]**.
1. Unter **[!UICONTROL Spalten (Ansicht)]** können Sie Ihre Spalten einrichten:

   ![Ein Bild des Bildschirms zur Erstellung von Spalten in Problemberichten](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problem] > [!UICONTROL Name]
   * [!UICONTROL Primärer Kontakt] > [!UICONTROL Name]
      * Hinweis: Dies wird mit &quot;Owner:Name&quot;als Spaltenbezeichnung angezeigt. Sie können dies in &quot;Gemeldet von&quot;ändern, indem Sie auf Erweiterte Optionen klicken und in die Variable **Eigene Spaltenbeschriftung** -Feld.
   * [!UICONTROL Problem] > [!UICONTROL Prozesstyp]
   * [!UICONTROL Problem] > [!UICONTROL Prozessname]
   * [!UICONTROL Problem] > [!UICONTROL Prozessqualität]
   * [!UICONTROL Problem] > [!UICONTROL Problem oder gute Nachrichten]
   * [!UICONTROL Problem] > [!UICONTROL Datum der Einsendung]
   * [!UICONTROL Problem] > [!UICONTROL Alter]
   * [!UICONTROL Problem] > [!UICONTROL Zuweisungen]
   * [!UICONTROL Problem] > [!UICONTROL Status]

1. Wählen Sie die Spalte **[!UICONTROL Eingabedatum]** und ändern Sie die Option **[!UICONTROL Absteigend sortieren]**.
1. Im **[!UICONTROL Gruppierungen]** -Registerkarte, legen Sie für den Bericht eine Gruppierung nach **[!UICONTROL Problem] > [!UICONTROL Prozesstyp]**.

   ![Ein Bild des Bildschirms zur Erstellung von Problemberichtsgruppen](assets/task-report-activity-2-2.png)

1. Im **[!UICONTROL Filter]** Registerkarte einen Filter für die **[!UICONTROL Problem] > [!UICONTROL Projekt-ID]** , um das Anforderungswarteschlangenprojekt zu entsprechen, in dem sich die Feedback-Probleme befinden.

   ![Ein Bild des Bildschirms zur Erstellung von Problemberichtsfiltern](assets/task-report-activity-2-3.png)

1. Speichern und schließen Sie den Bericht.

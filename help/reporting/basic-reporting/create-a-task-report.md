---
title: Erstellen eines Aufgabenberichts
description: Erfahren Sie, wie Sie einen Aufgabenbericht mit einem komplexen Filter erstellen und die in Workfront erstellten Berichte finden.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
last-substantial-update: 2025-06-11T00:00:00Z
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: e10995fb5e3c452df3177a4a29e187e862a1b4a5
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 77%

---

# Erstellen eines Aufgabenberichts

Das Video enthält eine schrittweise Anleitung zum Erstellen eines benutzerdefinierten Berichts, um späte Aufgaben zu verfolgen, die dem angemeldeten Benutzer zugewiesen wurden. Zunächst wird erklärt, dass benutzerdefinierte Berichte erforderlich sind, wenn vorhandene Filter, Ansichten oder integrierte Berichte bestimmte Anforderungen nicht erfüllen. &#x200B; Der Bericht trägt den Namen „Verspätete Aufgaben, die mir zugewiesen wurden“ und wird aus Gründen der Klarheit mit einer Beschreibung hinzugefügt. &#x200B;

Der resultierende Bericht hilft Benutzern, sich auf verspätete Aufgaben zu konzentrieren, bietet Einblicke in Abhängigkeiten und vereinfacht die Navigation zu den Host-Projekten. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Die wichtigsten Punkte

* **Erstellung benutzerdefinierter Berichte:** Wenn vorhandene Filter und integrierte Berichte Ihre Anforderungen nicht erfüllen, können Sie einen benutzerdefinierten Bericht von Grund auf neu erstellen, um sich auf bestimmte Daten zu konzentrieren, z. B. zugewiesene verspätete Aufgaben. &#x200B;
* **Filtereinrichtung:** Verwenden Sie Filter, um Berichtskriterien zu definieren, einschließlich verspäteter Aufgaben, unvollständiger Aufgaben, aktueller Projekte und Aufgaben, die dem angemeldeten Benutzer zugewiesen wurden. &#x200B;
* **Spalten für Kontext:** Fügen Sie Spalten wie „Kann beginnen“ hinzu, um Abhängigkeitsprobleme zu identifizieren, und „Projektname“ mit Hyperlinks, um die Navigation zu verwandten Projekten zu erleichtern. &#x200B;
* **Nach Priorität sortieren** Sortieren Sie Aufgaben nach der Spalte „Fällig am“ in aufsteigender Reihenfolge, um die am häufigsten überfälligen Aufgaben oben im Bericht zu priorisieren. &#x200B;
* **Barrierefreiheit:** Sie den Bericht, heften Sie ihn an oder markieren Sie ihn als Favoriten für den schnellen Zugriff, um eine effiziente Nachverfolgung und Verwaltung von verspäteten Aufgaben sicherzustellen.


## Aktivitäten zum Erstellen eines Aufgabenberichts

>[!TIP]
>
>Holen Sie Ihre Spachtel und Rührschüsseln hervor und machen Sie sich bereit, die „Rezepte“ in unserem [Adobe Workfront Customer Reporting-Kochbuch](/help/assets/workfront-customer-reporting-cookbook.pdf) auszuprobieren. Darin finden Sie Schritt-für-Schritt-Anweisungen für 10 Berichte, die Ihnen heute in Ihrer Umgebung zur Verfügung stehen.
>&#x200B;>Wir haben Lieblingsberichte von Kundinnen und Kunden gesammelt und in einem kleinen, leicht verdaulichen Kochbuch zusammengestellt, in dem Sie Ihre Workfront-Küche wieder ausprobieren können.
>&#x200B;>Diese 10 Berichte stammen von Kundinnen und Kunden, die genau wie Sie sind. Verteilt auf verschiedene Branchen, Abteilungen, Teams, Positionen und alle in verschiedenen Unternehmen, schulden wir den unglaublichen Kundinnen und Kunden, die einen ihrer Lieblingsberichte geteilt haben, ein riesiges Dankeschön. Einige Berichte sind einfach (aber unglaublich nützlich) und einige sind komplexer, um Ihre Berichterstellung auf die nächste Ebene zu bringen.


### Aktivität 1: Erstellen eines Notizberichts mit Eingabeaufforderungen

Erstellen Sie einen Notizbericht, mit dem Sie nach Benutzernotizen (d. h. Kommentaren oder Aktualisierungen) oder Systemnotizen auf Grundlage des Inhalts, der Autorin oder des Autors, des Eingabedatums, des Projektnamens oder der Überprüfungsart suchen können. Nennen Sie den Bericht „Notizsuche“.

Bei Verwendung der Eingabeaufforderung für den Notiztext sucht dieser Bericht in den Aktualisierungs-Threads, um schnell alle zu extrahieren, die den in den Eingabeaufforderungen angegebenen Kriterien entsprechen. Um den Bericht auszuführen, müssen Sie nicht jede Eingabeaufforderung ausfüllen, sondern nur diejenigen, die Ihnen wichtig sind. Leere Felder werden automatisch ignoriert.

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

### Antwort 1

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
1. Öffnen Sie die **[!UICONTROL Berichtseinstellungen]** und nennen Sie den Bericht „Notizsuche“.
1. Geben Sie in das Feld [!UICONTROL Beschreibung] etwas ein wie „Suche nach System- oder Benutzernotizen“ auf Grundlage des ausgewählten Prüfungstyps und anderer Aufforderungen. Systemnotizen erscheinen in der Spalte „Prüftext“ und Benutzernotizen in der Spalte „Notiztext“.

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

### Aktivität 2: Erstellen eines Feedback-Berichts für das Admin-Team

Dieser Problembericht zeigt alle Probleme aus einer Feedback-Anfrage-Warteschlange an, die für System-Admins erstellt wurde. Wie man diese Anfrage-Warteschlange erstellt, können Sie in der Anleitung [Erstellen einer Feedback-Anfrage-Warteschlange für System-Admins](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html?lang=de) sehen.

Dieser Bericht verwendet auch ein benutzerdefiniertes Formular. Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie in der Anleitung [Erstellen und Freigeben eines benutzerdefinierten Formulars](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html?land=de).

Dieses benutzerdefinierte Formular sollte die Objekttypen Projekt und Problem verwenden und wie folgt erstellt werden:

Name: Admin-Prozess-Feedback

1. Prozesstyp (Dropdown-Feld mit Einzelauswahl)
   * Zugriffsebenen
   * Genehmigungsprozess (nur global)
   * E-Mail-Benachrichtigungen
   * Layout-Vorlage
   * Meilensteinpfad
   * Projektvorlage
   * Erinnerungsbenachrichtigungen
   * Anfrage-Warteschlange
1. Prozessname (einzeiliges Textfeld)
1. Prozessqualität (Dropdown-Feld mit Einzelauswahl)
   * 1 - völlig nutzlos
   * 2 - nicht sehr nützlich
   * 3 - gut, aber könnte besser sein
   * 4 - hervorragend
1. Problem oder gute Nachrichten (Absatztextfeld)

Erstellen Sie einen Problembericht mit dem Namen **Admin-Team-Feedback-Bericht**.

Die Ansicht sollte die folgenden Spalten enthalten:

* Problem: Name
* Primärer Kontakt: Name
* Problem: Prozesstyp
* Problem: Prozessname
* Problem: Prozessqualität
* Problem: Problem oder gute Nachricht
* Problem: Eingabedatum
* Problem: Alter
* Problem: Arbeitsaufträge
* Problem: Status

Gruppieren Sie nach dem Prozesstyp.

Filtern Sie nach der ID des Projekts der Anfrage-Warteschlange, in dem sich die Feedback-Probleme befinden.


![Ein Screenshot des Feedback-Berichts des Admin-Teams](assets/create-a-system-admin-feedback-request-queue.png)



### Antwort 2

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf das Menü **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Problem]** aus.
1. Unter **[!UICONTROL Spalten (Ansicht)]** können Sie Ihre Spalten einrichten:

   ![Ein Screenshot des Bildschirms zum Erstellen von Spalten für Problemberichte](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problem] > [!UICONTROL Name]
   * [!UICONTROL Primärer Kontakt] > [!UICONTROL Name]
      * Hinweis: Dies wird mit „Owner:Name“ als Spaltenbezeichnung angezeigt. Sie können dies in „Gemeldet von“ ändern, indem Sie auf „Erweiterte Optionen“ klicken und im Feld **Benutzerdefinierte Spaltenbeschriftung** „Gemeldet von“ eingeben.
   * [!UICONTROL Problem] > [!UICONTROL Prozesstyp]
   * [!UICONTROL Problem] > [!UICONTROL Prozessname]
   * [!UICONTROL Problem] > [!UICONTROL Prozessqualität]
   * [!UICONTROL Problem] > [!UICONTROL Problem oder gute Nachrichten]
   * [!UICONTROL Problem] > [!UICONTROL Eingabedatum]
   * [!UICONTROL Problem] > [!UICONTROL Alter]
   * [!UICONTROL Problem] > [!UICONTROL Zuweisungen]
   * [!UICONTROL Problem] > [!UICONTROL Status]

1. Wählen Sie die Spalte **[!UICONTROL Eingabedatum]** und ändern Sie die Option **[!UICONTROL Absteigend sortieren]**.
1. Legen Sie auf der Registerkarte **[!UICONTROL Gruppierungen]** fest, dass der Bericht nach **[!UICONTROL Problem] > [!UICONTROL Prozesstyp]** gruppiert werden soll.

   ![Ein Screenshot des Bildschirms zum Erstellen von Gruppierungen für Problemberichte](assets/task-report-activity-2-2.png)

1. Fügen Sie auf der Registerkarte **[!UICONTROL Filter]** einen Filter für **[!UICONTROL Problem] > [!UICONTROL Projekt-ID]** hinzu, der dem Projekt der Anfrage-Warteschlange entspricht, in dem sich die Feedback-Probleme befinden.

   ![Ein Screenshot des Bildschirms zur Erstellung von Filtern für Problemberichte](assets/task-report-activity-2-3.png)

1. Speichern und schließen Sie den Bericht.

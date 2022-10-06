---
title: Voreinstellungen für globale Standardprobleme konfigurieren
description: Erfahren Sie, wie Sie Problemvoreinstellungen für konvertierte Probleme, tatsächliche Daten und Problemzugriff festlegen.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Allgemeine Standardeinstellungen für Probleme konfigurieren

Mehrere systemweite Einstellungen legen Standardeinstellungen für das Verhalten von Problemen unter bestimmten Umständen fest. [!DNL Workfront].

Es empfiehlt sich, die globalen Standardeinstellungen unverändert zu lassen und es Projektmanagern zu ermöglichen, die erforderlichen Anpassungen auf Projektebene oder in Projektvorlagen vorzunehmen.

Die globalen Problemvoreinstellungen können angepasst werden. Es wird jedoch empfohlen, dass Sie und Ihre [!DNL Workfront] beraten Sie, welche Einstellungen für die Workflows, Prozesse und Reporting-Anforderungen Ihres Unternehmens erforderlich sind. Ihr Berater kann Ihnen auch helfen zu verstehen, was passieren wird, wenn bestimmte Einstellungen geändert werden.

Mit den Ausgabevoreinstellungen können Systemadministratoren steuern, welche Optionen beim Konvertieren von Problemen in Aufgaben oder Projekte, bei der Berechnung der tatsächlichen Datumswerte und bei der Zuweisung von Problemen für wen der Projektzugriff besteht. Sehen wir uns diese Einstellungen an [!DNL Workfront].

## Konvertierte Ausgabevoreinstellungen

Diese Einstellungen steuern, was mit einem Problem passiert, wenn es in eine Aufgabe oder ein Projekt in [!DNL Workfront].

![[!UICONTROL Aufgaben und Probleme] Voreinstellungsfenster mit [!UICONTROL Probleme] Abschnitt hervorgehoben](assets/admin-fund-issue-prefs-converting.png)

1. Klicken **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** im linken Menübereich.
1. Auswählen **[!UICONTROL Aufgaben und Probleme]**.
1. Scrollen Sie zum **[!UICONTROL Probleme]** Abschnitt.
1. Klicken Sie auf die gewünschten Optionen.
1. Speichern Sie, wenn Sie fertig sind.

Werfen wir einen Blick auf die Optionen in diesem Abschnitt, damit Sie die entsprechenden Optionen für Ihre Organisation auswählen können.

* **[!UICONTROL Automatische Aktualisierung des Status &quot;Behebbares Problem&quot;, wenn der Status der aufgelösten Objektänderungen]**

   Mit dieser Einstellung können Sie die Auflösung des ursprünglichen Problems mit der Auflösung des neuen Objekts (Aufgabe oder Projekt) korrelieren.

   Wenn diese Einstellung aktiviert (aktiviert) ist, können Sie benutzerdefinierte Problemstatus erstellen, die denselben Statusschlüssel wie eine Aufgabe oder einen Projektstatus aufweisen. Wenn die Aufgabe oder das Projekt (das auflösbare Objekt) auf den benutzerdefinierten Status festgelegt ist, wird die Änderung auch beim Problemstatus angezeigt.

   Wenn diese Option deaktiviert ist, wird der aufgelöste Objektstatus automatisch auf den Standardstatus statt auf benutzerdefinierte festgelegt.

   Damit diese Einstellung Auswirkungen haben kann, muss[!UICONTROL Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an die Aufgabe]Die Option muss ausgewählt sein.

* **[!UICONTROL Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an die Aufgabe/das Projekt]**

   Wenn das Problem konvertiert wird, gibt dies Folgendes an: [!DNL Workfront] , um die ursprünglichen Probleme beizubehalten. Der Status des Problems ändert sich, wenn der Status der Aufgabe oder des Projekts geändert wird. Sobald die Aufgabe oder das Projekt als abgeschlossen markiert wurde, wird das Problem als behoben markiert.

   Wenn diese Option nicht aktiviert ist, wird das ursprüngliche Problem gelöscht und nur die konvertierte Aufgabe oder das konvertierte Projekt bleibt erhalten.

   Diese Einstellung wirkt sich auf die Berichterstellung zu Problemen aus, die ursprünglich in einem Projekt protokolliert wurden oder durch [!DNL Workfront] Anforderungswarteschlange.

* **[!UICONTROL Primären Kontakt Zugriff auf die Aufgabe/das Projekt gewähren]**

   Dadurch erhält die Person, die das ursprüngliche Problem erstellt hat, Zugriff auf die Aufgabe oder das Projekt, die bzw. das während der Konvertierung erstellt wurde. Sie können die Arbeit überprüfen, Aktualisierungen vornehmen und über ihre Fortschritte auf dem Laufenden bleiben.

* **[!UICONTROL Das Ändern dieser Einstellungen während der Konvertierung zulassen]**

   Bei Auswahl dieser Option stehen die Standardeinstellungen für[!UICONTROL Ursprüngliche Ausgabe beibehalten]&quot; und &quot;[!UICONTROL Primären Kontakt zulassen]&quot; kann vom Benutzer geändert werden, der das Problem konvertiert. Wenn die Standardwerte unverändert bleiben sollen, deaktivieren Sie diese Option.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Voreinstellungen für tatsächliche Datumswerte

Es gibt mehrere Arten von Daten, die in [!DNL Workfront]. Die tatsächlichen Daten sind ein &quot;Zeitstempel&quot;, der [!DNL Workfront] wird generiert, wenn bestimmte Statusänderungen auftreten.

Die [!UICONTROL Tatsächliches Startdatum] Der Zeitstempel wird erstellt, wenn sich der Problemstatus von Neu in einen anderen Status ändert. Die [!UICONTROL Tatsächliches Abschlussdatum] timestamp ist der Zeitpunkt, zu dem sich der Problemstatus in einen Status ändert, der angibt, dass es geschlossen ist.

Beachten Sie, dass diese Voreinstellung die tatsächlichen Datumseinstellungen für Aufgaben und Probleme steuert.

![[!UICONTROL Aufgaben und Probleme] Voreinstellungsfenster mit [!UICONTROL Tatsächliche Datumswerte] Abschnitt hervorgehoben](assets/admin-fund-issue-prefs-actual-dates.png)

1. Klicken **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** im linken Menübereich.
1. Auswählen **[!UICONTROL Aufgaben und Probleme]**.
1. Scrollen Sie zum **[!UICONTROL Tatsächliche Datumswerte]** Abschnitt.
1. Wählen Sie die gewünschte Option für die **[!UICONTROL Tatsächliches Startdatum]** — [!UICONTROL Jetzt] (Datum und Uhrzeit) oder [!UICONTROL Das geplante Startdatum] (der [!UICONTROL Tatsächliches Startdatum] entspricht dem in den Problemdetails festgelegten Startdatum).
1. Wählen Sie nun die Option für die **[!UICONTROL Tatsächliches Abschlussdatum]** — [!UICONTROL Jetzt] (Datum und Uhrzeit) oder [!UICONTROL Das geplante Abschlussdatum] (der [!UICONTROL Tatsächliches Startdatum] entspricht dem in den Problemdetails festgelegten Datum).
1. Speichern Sie, wenn Sie fertig sind.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Zugriff auf Probleme

Die [!UICONTROL Zugriff] Die Einstellungen für Probleme steuern, welchen Zugriff ein Benutzer erhält, wenn ihm in Workfront ein Problem zugewiesen wird. Diese Einstellungen steuern den Zugriff auf das Problem selbst, zusätzlich zum Zugriff auf das Projekt, mit dem das Problem verknüpft ist.

Bevor Sie diese Einstellungen ändern, besprechen Sie jeden Workflow oder jeden Prozess mit Ihrem [!DNL Workfront] Berater und Ihr internes Governance-Team.

![[!UICONTROL Aufgaben und Probleme] Voreinstellungsfenster mit [!UICONTROL Wenn jemand einem PROBLEM zugewiesen ist] Abschnitt hervorgehoben](assets/admin-fund-issue-prefs-access-1.png)

1. Klicken **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** im linken Menübereich.
1. Auswählen **[!UICONTROL Aufgaben und Probleme]**.
1. Scrollen Sie zum **[!UICONTROL Zugriff]** und suchen Sie nach &quot;[!UICONTROL Wenn jemand einem PROBLEM zugewiesen ist]&quot;.
1. Legen Sie den Freigabezugriff für das Problem selbst fest — [!UICONTROL Ansicht], [!UICONTROL Beitragen]oder [!UICONTROL Verwalten]. [!DNL Workfront] empfiehlt, die erweiterten Optionen unverändert zu lassen.
1. Aktivieren Sie das Kästchen, wenn der Problemverantwortliche auch Zugriff auf das Projekt haben sollte.
1. Wählen Sie dann den Freigabezugriff für das Projekt aus — [!UICONTROL Ansicht], [!UICONTROL Beitragen]oder [!UICONTROL Verwalten]. Wenn Sie [!UICONTROL Erweiterte Optionen]Beachten Sie die Workflows und Zugriffsanforderungen Ihres Unternehmens.
1. Speichern Sie, wenn Sie fertig sind.

![[!UICONTROL Zugriff] Fensteranzeige [!UICONTROL Beitragen] options](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->

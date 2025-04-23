---
title: Konfigurieren der globalen standardmäßigen Problemvoreinstellungen
description: Erfahren Sie, wie Sie Problemvoreinstellungen für konvertierte Probleme, tatsächliche Daten und Problemzugriff festlegen.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 75%

---

# Konfigurieren der globalen standardmäßigen Problemvoreinstellungen

Mehrere systemweite Einstellungen legen standardmäßig fest, wie sich Probleme unter bestimmten Umständen in [!DNL Workfront] verhalten.

Best Practice ist es, die globalen Standardeinstellungen so zu belassen, wie sie sind, und den Projekt-Managerinnen und -Managern die Möglichkeit zu geben, die erforderlichen Anpassungen auf Projektebene oder in Projektvorlagen vorzunehmen.

Die globalen Problemeinstellungen können angepasst werden. Es wird jedoch empfohlen, dass Sie und Ihr [!DNL Workfront] besprechen, welche Einstellungen für die Workflows, Prozesse und Reporting-Anforderungen Ihres Unternehmens erforderlich sind. Ihre Beraterin bzw. Ihr Berater kann Ihnen auch erklären, was passiert, wenn bestimmte Einstellungen geändert werden.

Mit den Problemvoreinstellungen können Systemadmins steuern, wann Probleme in Aufgaben oder Projekte konvertiert werden, wie tatsächliche Daten berechnet werden und wer bei der Zuweisung von Problemen Zugang zum Projekt erhält. Sehen wir uns an, wo sich diese Einstellungen [!DNL Workfront] befinden.

## Voreinstellungen für konvertierte Probleme

Diese Einstellungen steuern, was mit einem Problem geschieht, wenn es in [!DNL Workfront] in eine Aufgabe oder ein Projekt konvertiert wird.

Voreinstellungen-Fenster ![[!UICONTROL Aufgaben und Probleme] mit hervorgehobenem Abschnitt [!UICONTROL Probleme]](assets/admin-fund-issue-prefs-converting.png)

1. Klicken Sie auf **[!UICONTROL Setup]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** in der linken Menüleiste.
1. Wählen Sie **[!UICONTROL Aufgaben und Probleme]**.
1. Scrollen Sie zum Abschnitt **[!UICONTROL Probleme]**.
1. Wählen Sie die gewünschten Optionen.
1. Speichern, wenn Sie fertig sind.

Sehen wir uns die Optionen in diesem Abschnitt an, damit Sie die entsprechenden Optionen für Ihr Unternehmen auswählen können.

* **[!UICONTROL Status für „“ automatisch aktualisieren, wenn sich der Status für „Problemlösendes Objekt“ ändert]**

  Mit dieser Einstellung können Sie die Lösung des ursprünglichen Problems mit der Lösung des neuen Objekts (Aufgabe oder Projekt) in Beziehung setzen.

  Wenn diese Einstellung aktiviert ist (Haken gesetzt), können Sie benutzerdefinierte Problemstatus erstellen, die denselben Statusschlüssel haben wie ein Aufgaben- oder Projektstatus. Wenn die Aufgabe oder das Projekt (das Lösungsobjekt) auf den benutzerdefinierten Status festgelegt ist, wird die Änderung auch beim Problemstatus angezeigt.

  Wenn diese Option deaktiviert ist, wird der Status des Lösungsobjekts automatisch auf den Standardstatus statt auf benutzerdefinierte Status festgelegt.

  Damit diese Einstellung wirksam wird, muss die Option &quot;[!UICONTROL Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen] ausgewählt werden.

* **[!UICONTROL Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen]**

  Wenn das Problem konvertiert ist, weiß [!DNL Workfront], dass die ursprünglichen Probleme beibehalten werden sollen. Der Status des Problems ändert sich, wenn der Status der Aufgabe oder des Projekts geändert wird. Sobald die Aufgabe oder das Projekt als abgeschlossen markiert wurde, wird das Problem als behoben markiert.

  Wenn diese Option nicht aktiviert ist, wird das ursprüngliche Problem gelöscht und nur die konvertierte Aufgabe oder das konvertierte Projekt bleibt erhalten.

  Diese Einstellung wirkt sich auf die Berichterstellung zu Problemen aus, die ursprünglich in einem Projekt protokolliert wurden oder über eine Anfrage-Warteschlange von [!DNL Workfront] eingehen.

* **[!UICONTROL Dem primären Kontakt Zugriff auf die Aufgabe bzw. das Projekt erteilen]**

  Dadurch erhält die Person, die das ursprüngliche Problem erstellt hat, Zugriff auf die Aufgabe oder das Projekt, die bzw. das während der Konvertierung erstellt wurde. Sie können die Arbeit überprüfen, Aktualisierungen vornehmen und über ihre Fortschritte auf dem Laufenden bleiben.

* **[!UICONTROL Das Ändern dieser Einstellungen während der Konvertierung zulassen]**

  Wenn diese Option ausgewählt ist, können die Standardeinstellungen für &quot;[!UICONTROL Ursprüngliches Problem beibehalten] und &quot;[!UICONTROL Primären Kontakt zulassen] geändert werden, wenn der Benutzer das Problem konvertiert. Wenn die Standardwerte unverändert bleiben sollen, deaktivieren Sie diese Option.

<!--
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
-->

## Voreinstellungen für tatsächliche Datumswerte

Es gibt mehrere Arten von Daten, die in [!DNL Workfront] verwendet werden. Die tatsächlichen Daten sind ein „Zeitstempel“, der [!DNL Workfront] generiert, wenn bestimmte Statusänderungen auftreten.

Der Zeitstempel [!UICONTROL Tatsächliches Startdatum] wird erstellt, wenn sich der Problemstatus von „Neu“ in einen anderen Status ändert. Der Zeitstempel [!UICONTROL Tatsächliches Abschlussdatum] ist der Zeitpunkt, zu dem sich der Problemstatus in einen Status ändert, der angibt, dass die Aufgabe bzw. das Problem geschlossen ist.

Beachten Sie, dass diese Voreinstellung die tatsächlichen Datumseinstellungen für Aufgaben und Probleme steuert.

Das Fenster der Voreinstellungen für ![[!UICONTROL Aufgaben und Probleme], mit Hervorhebung des Abschnitts [!UICONTROL Tatsächliche Datumswerte]](assets/admin-fund-issue-prefs-actual-dates.png)

1. Klicken Sie auf **[!UICONTROL Setup]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** in der linken Menüleiste.
1. Wählen Sie **[!UICONTROL Aufgaben und Probleme]** aus.
1. Scrollen Sie zum Abschnitt **[!UICONTROL Tatsächliche Datumswerte]**.
1. Wählen Sie die gewünschte Option für das **[!UICONTROL tatsächliche Startdatum aus]** – [!UICONTROL Jetzt] (das aktuelle Datum und die aktuelle Uhrzeit) oder das [!UICONTROL geplante Startdatum] (das [!UICONTROL tatsächliche Startdatum] entspricht dem in den Problemdetails festgelegten Startdatum).
1. Wählen Sie nun die Option für das **[!UICONTROL tatsächliche Abschlussdatum aus]** – [!UICONTROL Jetzt] (das aktuelle Datum und die aktuelle Uhrzeit) oder das [!UICONTROL geplante Abschlussdatum] (das [!UICONTROL tatsächliche Startdatum] entspricht dem in den Problemdetails festgelegten Datum).
1. Speichern, wenn Sie fertig sind.


<!--
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
-->

## Zugriff auf Probleme

Die [!UICONTROL Zugriff]-Einstellungen für Probleme steuern, welcher Zugriff einem Benutzer gewährt wird, wenn ihm ein Problem in Workfront zugewiesen wird. Diese Einstellungen steuern den Zugriff auf das Problem selbst, zusätzlich zum Zugriff auf das Projekt, mit dem das Problem verknüpft ist.

Bevor Sie diese Einstellungen ändern, besprechen Sie Anforderungen für Workflows oder Prozesse mit Ihren [!DNL Workfront]-Beraterinnen und -Beratern und Ihrem internen Governance-Team.

Das Voreinstellungsfenster ![[!UICONTROL Aufgaben und Probleme], mit Hervorhebung des Abschnitts [!UICONTROL Wenn eine Person einem PROBLEM zugeteilt wird]](assets/admin-fund-issue-prefs-access-1.png)

1. Klicken Sie auf **[!UICONTROL Setup]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** in der linken Menüleiste.
1. Wählen Sie **[!UICONTROL Aufgaben und Probleme]** aus.
1. Scrollen Sie zum Abschnitt **[!UICONTROL Zugriff]** und suchen Sie die Option &quot;[!UICONTROL Wenn jemand einem PROBLEM zugewiesen ]&quot;.
1. Legen Sie den Freigabezugriff für das Problem selbst fest – [!UICONTROL Anzeigen], [!UICONTROL Mitwirken] oder [!UICONTROL Verwalten]. [!DNL Workfront] empfiehlt, die erweiterten Optionen unverändert zu lassen.
1. Aktivieren Sie das Kontrollkästchen, wenn die Person, der das Problem zugeteilt wird, auch Zugriff auf das Projekt haben soll
1. Wählen Sie dann den Freigabezugriff für das Projekt aus – [!UICONTROL Anzeigen], [!UICONTROL Mitwirken] oder [!UICONTROL Verwalten]. Beachten Sie bei der Festlegung [!UICONTROL  „Erweiterte Optionen] die Workflows und Zugriffsanforderungen Ihres Unternehmens.
1. Speichern, wenn Sie fertig sind.

Das Fenster ![[!UICONTROL Zugriff], in dem die Option [!UICONTROL Mitwirken] zu sehen ist](assets/admin-fund-issue-prefs-access-2.png)

<!--
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
-->

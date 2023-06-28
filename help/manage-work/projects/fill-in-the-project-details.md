---
title: Füllen Sie die Projektdetails aus.
description: Erfahren Sie, welche 12 Felder für Projektdetails [!DNL  Workfront] empfiehlt, beim Erstellen eines Projekts auszufüllen.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# Füllen Sie die Projektdetails aus.

Keine Sorge ... Sie müssen nicht jedes Feld und Kontrollkästchen in den Projektdetails mit jedem Projekt ausfüllen, das Sie in erstellen [!DNL  Workfront]. Verwenden Sie Vorlagen zum Vorausfüllen von Informationen und wenden Sie sich dann an die 12 wichtigsten Felder mit Projektdetails, die unten aufgeführt sind.

1. **Name**

   Ein beschreibender Projektname hilft jedem, den Zweck des Projekts zu identifizieren. Achten Sie darauf, die Namenskonvention für Projekte in Ihrem Unternehmen zu befolgen. Möglicherweise müssen im Projektnamen bestimmte Informationen enthalten sein (z. B. eine Referenznummer, einen Abteilungsnamen oder eine Kategorieanzeige).


1. **Beschreibung**

   Wenn mehrere Personen an einem Projekt arbeiten, müssen Sie - als Projektmanager - sicherstellen, dass jeder mit dem Ziel und den Erwartungen des Projekts Schritt hält.

   Erstellen Sie hierzu eine Projektbeschreibung, die grundlegende Informationen enthält und Fragen beantwortet und es dem Projektteam ermöglicht, seine Arbeit fortzusetzen. Beispiel: &quot;Eine Kampagne, die darauf abzielt, die Ertragsarbeit um 50 % zu steigern&quot; oder &quot;Neues System-Upgrade zur Verbesserung der Effizienz in der gesamten Abteilung&quot;.

   Einige Workfront-Kunden enthalten ein Beispiel dafür, wie eine Projektbeschreibung in ihren Projektvorlagen aussehen sollte.

1. **Status**

   Der Status wird in Workfront verwendet, um anzugeben, wo oder zu welchem Zeitpunkt im Workflow ein Projekt steht. Der Status wird in vielen Workfront-Berichten verwendet, um den Fortschritt der Arbeit zu verfolgen.

   Workfront empfiehlt, den Status auf Planung festzulegen, während Sie den Projektplan ausdehnen und abschließen. Das Wichtigste beim Planungsstatus ist, dass Workfront-Benachrichtigungen nicht an Aufgabenverantwortliche gesendet werden, während sie sich in diesem Status befinden.

   Sobald das Projekt live geschaltet werden kann, ändern Sie den Status in Aktuell . Dadurch kann Workfront Benachrichtigungen über neue Aufgaben senden, denen sie zugewiesen sind. Es werden jedoch keine Benachrichtigungen für die Aufgaben gesendet, die Benutzern zugewiesen wurden, während sich das Projekt im Planungsstatus befand.

   >[!TIP]
   >
   >  Wenn Sie Änderungen am Projekt vornehmen, z. B. das Ändern des Fälligkeitsdatums, können Sie den Status zurück in die Planung setzen oder die Funktion Automatisches Speichern deaktivieren, um zu verhindern, dass Benachrichtigungen gesendet werden, bis Änderungen abgeschlossen sind.

   Der Planungsstatus kann von Ihrem Systemadministrator als globale Workfront-Standardeinstellung für neue Projekte festgelegt werden.

1. **Zeitplanmodus**

   Workfront-Projekte können von einem Start- oder einem Abschlussdatum an geplant werden. Diese wichtige Auswahl bestimmt, wie die geplanten Daten jeder Aufgabe berechnet werden.

   Die Option Startdatum berechnet anhand des von Ihnen eingegebenen Startdatums für das Projekt sowie der Dauer und den Vorgängern der jeweiligen Aufgabe den Zeitpunkt, zu dem das Projekt abgeschlossen sein wird. Workfront empfiehlt die Verwendung dieser Option, da sie am häufigsten verwendet wird und die Planung von Projektdaten erleichtert.

   Sie können jedoch ein Abschlussdatum verwenden. Workfront untersucht das Enddatum (von Ihnen eingegeben) und die zu leistende Arbeit (basierend auf Dauern und Vorgängern) und berechnet dann das Projektstartdatum rückwärts. Workfront empfiehlt, das Fertigstellungsdatum abzuwarten, nachdem ein bestimmtes Maß an Kompetenz in Workfront erreicht wurde.

   Vergessen Sie nicht, für welche Option Sie sich entscheiden, ein Datum aus dem Popup-Kalender auszuwählen.

   Die Option Planmodus kann in der Vorlage festgelegt werden.

1. **Gruppe**

   Eine Gruppe ist eine Organisationseinheit in Workfront, die häufig einer Abteilung zugeordnet wird. Dieses Feld kann in der Projektvorlage festgelegt werden. Ist dies nicht der Fall, wird das Feld automatisch auf die Startseite der Person gesetzt, die das Projekt erstellt. Sie können die Gruppe nach Bedarf ändern.

   Im Allgemeinen stammen die meisten Menschen, die an dem Projekt arbeiten, aus dieser Gruppe. Dies schränkt jedoch nicht die Arbeit anderer Gruppen ein, denen im Projekt Arbeit zugewiesen wurde.

   Die Gruppe für das Projekt bestimmt außerdem, welche Projekt-, Aufgaben- und Problemeinstellungen das Projekt verwendet. Diese Voreinstellungen, z. B. ein benutzerdefinierter Status für eine bestimmte Gruppe, werden vom Systemadministrator oder einem Gruppenadministrator festgelegt.

   Die Gruppeneinstellung ist eine bequeme Möglichkeit, durch Berichte alle Projekte anzuzeigen, an denen eine Abteilung arbeitet.

1. **Projektbesitzer**

   Der Projekteigentümer ist der Begriff von Workfront für den Projektmanager. Dies ist die für die Planung und/oder Verwaltung des Projekts verantwortliche Person.

   Damit der Projekteigentümer über vollständige Verwaltungsberechtigungen für das Projekt verfügen kann, muss er über eine Planungslizenz verfügen.

   Normalerweise wird dieses Feld in der Vorlage leer gelassen und automatisch mit dem Namen der Person ausgefüllt, die das Projekt erstellt. Wenn ein Name in die Vorlage eingegeben wird, ist dies der Standardeigentümer des Projekts.

1. **Projektsponsor**

   Der Projektsponsor ist nicht erforderlich, aber bei Verwendung dieser ist in der Regel die Person, die das Projekt angefordert hat. Dies ist häufig ein interner Verantwortlicher, z. B. ein Manager oder eine Führungskraft, der bzw. die für das Projekt insgesamt verantwortlich ist.

   Der Sponsor erhält automatisch Anzeigeberechtigungen für das Projekt und muss ein von Workfront lizenzierter Benutzer sein.

   Der Projektsponsor kann in der Vorlage festgelegt werden.

1. **Ressourcenmanager**

   Die in diesem Feld aufgelisteten Workfront-Benutzer können die Tools zur Ressourcenplanung und -verwaltung in Workfront für die spezifischen Projekte verwenden, in denen sie aufgeführt sind. Im Feld Ressourcen-Manager können bis zu 30 Namen aufgeführt werden, von denen jeder über eine Planlizenz verfügen muss.

   Das Feld Ressourcen-Manager kann in der Vorlage festgelegt werden.

1. **Benutzerdefinierte Formulare**

   Workfront stellt native Felder für Elemente wie Projektname und Startdatum bereit. Es gibt jedoch zusätzliche Informationen, die Sie als Projektmanager benötigen oder die das Projektteam benötigen wird. Ihre eindeutigen Daten sind gleichermaßen wichtig und können in diesen Formularen leicht gespeichert werden. Details wie Veröffentlichungsdaten, Größe von Druck-Assets, Versandkanäle usw.

   Benutzerdefinierte Formulare können diese Informationen erfassen und in Listen und Berichten in Workfront enthalten sein, wodurch die Informationen einfach angezeigt und bearbeitet werden können.

   Benutzerdefinierte Formulare können vorzeitig an Ihre Vorlagen angehängt werden.

1. **Zeitplan**

   Arbeiten finden rund um die Uhr statt, da viele Unternehmen Mitarbeiter auf der ganzen Welt haben.

   Mit Workfront können Sie einen gemeinsamen Zeitplan auf Projekte anwenden. Diese werden von Ihrem Systemadministrator erstellt. Die Zeitpläne spiegeln die Arbeitstage und Stunden Ihrer Teams sowie die Tage wider, an denen Mitarbeiter nicht arbeiten (z. B. Feiertage).

   Stellen Sie als Planer sicher, dass Sie den richtigen Zeitplan auf das richtige Projekt anwenden. Die Zeitplaneinstellungen wirken sich auf Zeitleistenberechnungen aus und berücksichtigen dabei die Zeitzonen und Zeitzonen.

   Der dem Projekt zugewiesene Zeitplan sollte derjenige sein, der für den Großteil der Aufgabe gilt. Wenn für das Projekt kein Zeitplan angegeben ist, wird der als Standard markierte Zeitplan verwendet.

   Der Zeitplan kann in der Vorlage festgelegt werden.

1. **Ressourcenpools**

   Ressourcen-Pools sind Sammlungen von Workfront-Benutzern, die gleichzeitig für den Abschluss von Projekten in Ihrem Unternehmen benötigt werden. Ein Ressourcen-Pool kann mehreren Projekten zugewiesen werden, d. h. Sie haben Projekte, die um Ressourcen konkurrieren.

   Die Zuweisung von Ressourcenpools zu einem Projekt ist eine Voraussetzung für die Verwendung des Ressourcenplaners und anderer Tools zur Ressourcenverwaltung in Workfront.

   In der Vorlage kann ein standardmäßiger Ressourcen-Pool festgelegt werden.

1. **Zugriff auf das Projekt für Viewer und Mitarbeiter**

   Wenn jemand über die Freigabe Zugriff auf ein Projekt erhält, können ihm drei Berechtigungsstufen zugewiesen werden: Anzeigen, Beiträge und Verwalten. Jede Berechtigungsebene ermöglicht es dem Benutzer, bestimmte Dinge mit dem Projekt anzuzeigen und zu tun.

   Zum Beispiel gibt es Leute, die vielleicht Zugriff auf das Projekt haben, aber die finanziellen Informationen nicht sehen sollten. So können Sie die Option Finanzen anzeigen für sie deaktivieren.

   Die Zugriffseinstellungen können in der Vorlage festgelegt werden.

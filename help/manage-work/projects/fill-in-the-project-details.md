---
title: Ausfüllen der Projektdetails
description: Erfahren Sie, welche 12 Felder für Projektdetails Sie gemäß den Empfehlungen von [!DNL  Workfront] ausfüllen sollten, wenn Sie ein Projekt erstellen.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Beginner
recommendations: noDisplay,noCatalog
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: c2ba2ddfbbc642398a0136ecbf7c3613208080c4
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 97%

---

# Ausfüllen der Projektdetails

Keine Sorge, Sie müssen nicht bei jedem Projekt, das Sie in [!DNL  Workfront] erstellen, alle Felder und Kontrollkästchen in den Projektdetails ausfüllen. Verwenden Sie Vorlagen zum Vorausfüllen von Informationen und richten Sie Ihre Aufmerksamkeit auf die 12 wichtigsten Felder mit Projektdetails, die unten aufgeführt sind.

1. **Name**

   Ein beschreibender Projektname hilft allen, den Zweck des Projekts zu erkennen. Achten Sie darauf, die Namenskonvention für Projekte in Ihrem Unternehmen zu befolgen. Möglicherweise müssen im Projektnamen bestimmte Informationen enthalten sein (z. B. eine Referenznummer, ein Abteilungsname oder eine Kategorieanzeige).


1. **Beschreibung**

   Wenn mehrere Personen an einem Projekt arbeiten, müssen Sie – als Projektleitung – sicherstellen, dass jeder mit dem Ziel und den Erwartungen des Projekts Schritt hält.

   Dies geschieht mithilfe einer Projektbeschreibung, die grundlegende Informationen liefert, Fragen beantwortet und es dem Projekt-Team ermöglicht, mit der Arbeit fortzufahren. Beispiel: „Eine Kampagne, die darauf abzielt, die Ertragsarbeit um 50 % zu steigern“ oder „Neues System-Upgrade zur Verbesserung der Effizienz in der gesamten Abteilung“.

   Einige Workfront-Kundinnen und -Kunden schließen in ihren Projektvorlagen ein Beispiel dafür ein, wie eine Projektbeschreibung aussehen sollte.

1. **Status**

   Der Status wird in Workfront verwendet, um anzuzeigen, wo bzw. in welchem Stadium sich ein Projekt im Arbeitsablauf befindet. Der Status wird in vielen Workfront-Berichten verwendet, um den Fortschritt der Arbeit zu verfolgen.

   Workfront empfiehlt, den Status auf „in Planung“ zu setzen, während Sie den Projektplan ausarbeiten und fertigstellen. Das Wichtigste beim Planungsstatus ist, dass Workfront-Benachrichtigungen nicht an Aufgabenverantwortliche gesendet werden, während sich das Projekt in diesem Status befinden.

   Wenn das Projekt dann live geschaltet werden kann, ändern Sie den Status in „Aktuell“. Dadurch kann Workfront Benachrichtigungen über neue Aufgaben an Personen senden, denen sie zugewiesen sind. Es werden jedoch keine Benachrichtigungen für die Aufgaben gesendet, die Benutzenden zugewiesen wurden, während sich das Projekt im Planungsstatus befand.

   >[!TIP]
   >
   >  Wenn Sie Änderungen am Projekt vornehmen, z. B. das Ändern des Fälligkeitsdatums, können Sie den Status zurück auf „In Planung“ setzen oder die Funktion „Automatisches Speichern“ deaktivieren, um zu verhindern, dass Benachrichtigungen gesendet werden, bis Änderungen abgeschlossen sind.

   Der Status „In Planung“ kann von Systemadmins als globale Workfront-Standardeinstellung für neue Projekte festgelegt werden.

1. **Zeitplanmodus**

   Workfront-Projekte können vom Startdatum aus oder vom Fertigstellungsdatum aus geplant werden. Diese wichtige Auswahl bestimmt, wie die geplanten Termine jeder Aufgabe berechnet werden.

   Mit der Option „Startdatum“ können Sie anhand des von Ihnen eingegebenen Startdatums für das Projekt sowie der Dauer und der Vorgänger der einzelnen Aufgaben berechnen, wann das Projekt abgeschlossen sein wird. Workfront empfiehlt die Verwendung dieser Option, da sie am häufigsten verwendet wird und die Planung von Projektdaten erleichtert.

   Sie können jedoch auch ein Fertigstellungsdatum verwenden. Workfront betrachtet in diesem Fall das (von Ihnen eingegebene) Enddatum und die zu erledigende Arbeit (auf der Grundlage von Zeiträumen und Vorgängern) und arbeitet dann rückwärts, um das Startdatum des Projekts zu berechnen. Workfront empfiehlt, mit der Verwendung des Fertigstellungsdatums zu warten, bis ein bestimmtes Maß an Kompetenz in Workfront erreicht wurde.

   Für welche Option Sie sich auch entscheiden, vergessen Sie nicht, ein Datum aus dem Popup-Kalender auszuwählen.

   Die Option „Planmodus“ kann in der Vorlage festgelegt werden.

1. **Gruppe**

   Eine Gruppe ist in Workfront eine organisatorische Einheit, die oft einer Abteilung entspricht. Dieses Feld kann in der Projektvorlage festgelegt werden. Wird es nicht festgelegt, wird das Feld automatisch auf die Hauptgruppe der Person festgelegt, die das Projekt erstellt. Sie können die Gruppe nach Bedarf ändern.

   In der Regel kommen die meisten der an dem Projekt beteiligten Personen aus dieser Gruppe. Dies verhindert jedoch nicht die Möglichkeit, dass auch Personen aus anderen Gruppen mit der Arbeit an dem Projekt betraut werden.

   Die Projektgruppe bestimmt auch, welche Voreinstellungen für Projekte, Aufgaben und Probleme das Projekt verwenden soll. Diese Voreinstellungen, z. B. ein benutzerdefinierter Status für eine bestimmte Gruppe, werden von Systemadmins oder Gruppenadmins festgelegt.

   Die Gruppeneinstellung ist eine bequeme Möglichkeit, durch das Reporting alle Projekte anzuzeigen, an denen eine Abteilung arbeitet.

1. **Projektbesitzer**

   „Projektbesitzer“ ist der Begriff für die Projektleitung in Workfront. Dies ist die für die Planung und/oder Verwaltung des Projekts verantwortliche Person.

   Damit diese Person über vollständige Verwaltungsberechtigungen für das Projekt verfügen kann, muss sie über eine Planlizenz verfügen.

   Normalerweise wird dieses Feld in der Vorlage leer gelassen und automatisch mit dem Namen der Person ausgefüllt, die das Projekt erstellt. Wenn ein Name in die Vorlage eingegeben wird, ist dies der Standardbesitzer bzw. die Standardbesitzerin des Projekts.

1. **Projektsponsor**

   Der Projektsponsor ist nicht erforderlich, aber wenn er verwendet wird, ist dies im Allgemeinen die Person, die das Projekt beantragt hat. Dies ist häufig ein interner Stakeholder, z. B. eine Managerin bzw. ein Manager oder eine Führungskraft, die für das Projekt insgesamt verantwortlich ist.

   Der Sponsor erhält automatisch Anzeigeberechtigungen für das Projekt und muss zu den lizenzierten Workfront-Benutzenden gehören.

   Der Projektsponsor kann in der Vorlage festgelegt werden.

1. **Ressourcenmanager**

   Die in diesem Feld aufgeführten Workfront-Benutzenden können die Tools zur Ressourcenplanung und -verwaltung in Workfront für die spezifischen Projekte, für die sie aufgeführt sind, nutzen. Im Feld „Ressourcen-Manager“ können bis zu 30 Namen aufgeführt werden, von denen jeder über eine Planlizenz verfügen muss.

   Das Feld „Ressourcen-Manager“ kann in der Vorlage festgelegt werden.

1. **Benutzerdefinierte Formulare**

   Workfront bietet native Felder für Optionen wie Projektname und Startdatum. Als Projektleiterin bzw. Projektleiter benötigen Sie und das Projekt-Team aber noch weitere Informationen. Ihre individuellen Daten sind ebenso wichtig und lassen sich in diesen Formularen leicht speichern. Details wie Veröffentlichungsdaten, Größe von Druck-Assets, Versandkanäle usw.

   Benutzerdefinierte Formulare können diese Informationen erfassen und in Listen und Berichten in Workfront aufgenommen werden, sodass sie einfach angezeigt und bearbeitet werden können.

   Benutzerdefinierte Formulare können vorzeitig an Ihre Vorlagen angehängt werden.

1. **Zeitplan**

   Da viele Unternehmen Mitarbeitende auf der ganzen Welt haben, wird rund um die Uhr irgendwo gearbeitet.

   Workfront ermöglicht es Ihnen, gemeinsame Projektzeitpläne zu verwenden. Diese werden von Ihren Systemadmins erstellt. Die Zeitpläne spiegeln die Arbeitstage und Stunden Ihrer Teams sowie die arbeitsfreien Tage wider (z. B. Feiertage).

   Stellen Sie beim Planen sicher, dass Sie den richtigen Zeitplan auf das richtige Projekt anwenden. Die Zeitplaneinstellungen wirken sich auf Berechnungen der Zeitleiste aus und berücksichtigen dabei die Ausfallzeiten und Zeitzonen.

   Der dem Projekt zugewiesene Zeitplan sollte derjenige sein, der für die Mehrheit der mit Aufgaben Beauftragten gilt. Wenn für das Projekt kein Zeitplan angegeben ist, wird der als Standard markierte Zeitplan verwendet.

   Der Zeitplan kann in der Vorlage festgelegt werden.

1. **Ressourcenpools**

   Ressourcen-Pools sind Sammlungen von Workfront-Benutzenden, die zur gleichen Zeit für die Durchführung von Projekten in Ihrem Unternehmen benötigt werden. Ein Ressourcen-Pool kann mehreren Projekten zugewiesen werden, sodass Projekte um Ressourcen konkurrieren können.

   Die Zuweisung von Ressourcen-Pools zu einem Projekt ist eine Voraussetzung für die Verwendung des Ressourcenplaners und anderer Tools zum Ressourcen-Management in Workfront.

   In der Vorlage kann ein standardmäßiger Ressourcen-Pool festgelegt werden.

1. **Zugriff auf das Projekt für Betrachtende und Mitwirkende**

   Wenn einer Person über die Freigabe Zugriff auf ein Projekt gewährt wird, gibt es drei Berechtigungsstufen: Anzeigen, Mitwirken und Verwalten. Jede Berechtigungsstufe ermöglicht es der Person, bestimmte Dinge anzuzeigen und mit dem Projekt zu tun.

   So gibt es beispielsweise Personen, die zwar Zugang zu dem Projekt haben, aber die Finanzinformationen nicht sehen sollten. So können Sie die Option „Finanzen anzeigen“ für sie deaktivieren.

   Die Zugriffseinstellungen können in der Vorlage festgelegt werden.

## Empfohlene Tutorials zu diesem Thema

* [Grundlegendes zur Projekterstellung](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-basic-project-creation)
* [Navigieren zur Projektseite](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/navigate-the-project-page)
* [Vier Möglichkeiten zum Erstellen eines Projekts](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-other-ways-to-create-projects)
* [Erste Schritte bei der Projektplanung](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/getting-started-plan-a-project)

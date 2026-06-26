---
title: Erkunden von Projektzeitleisten in Workfront
description: Erfahren Sie, wie Sie Aufgaben zuweisen, Gantt-Diagramme und Funktionen für kritische Pfade verwenden, Projekte über Ansichten überwachen, Aufgaben effizient planen und Einschränkungen für eine optimale Projektplanung anwenden.
activity: use
feature: Work Management
thumbnail: 335213.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: '2024-11-01T00:00:00.000Z'
recommendations: noDisplay,catalog
jira: KT-8953
exl-id: ba993197-9f84-4fc0-86cc-cf849c889f56
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:48:54.364Z'
source-git-commit: df1a568be7d42893910e1c0afde8bbba213a7803
workflow-type: tm+mt
source-wordcount: 700
ht-degree: 74%

---

# Erkunden von Projektzeitleisten in Workfront

Was Sie lernen werden:

* Sie erhalten einen Überblick über die Planung und das Management von Projekten mit Workfront. Sie erfahren, wie Sie durch übergeordnete Aufgaben mehrere Unteraufgaben zusammen gruppieren, die Aufgabengebieten und später Benutzenden mit den erforderlichen Kenntnissen zugewiesen werden. Vorgänger geben sequenzielle Beziehungen zwischen Aufgaben an, während Aufgaben ohne Vorgänger parallel ausgeführt werden können. Das Gantt-Diagramm bietet eine visuelle Timeline und die Funktion „Kritischer Pfad“ hebt Aufgaben hervor, die das Projekt bei Nichterfüllung verzögern könnten.
* Es stehen verschiedene Ansichten in Workfront zur Verfügung, z. B. die Standardansicht für die Planung und die Statusansicht für die Überwachung. Diese enthalten Flags für Fortschritt, Kommentare, Dokumente, Probleme, Genehmigungen, kritische Pfade und Meilensteine. Die letzten Aktivitäten können nachverfolgt werden, um Aktualisierungen und Notizen anzuzeigen.
* Die Planung kann ab einem Start- oder Fertigstellungsdatum erfolgen. Workfront berechnet dabei die entsprechenden Daten anhand der Aufgabenlaufzeiten und Vorgänger. Im Video wird empfohlen, bei kritischen Fertigstellungsdaten ausgehend von einem Startdatum zu planen, um einen gewissen Spielraum zu ermöglichen. Aufgabenbeschränkungen wie „So bald wie möglich“ und „So spät wie möglich“ werden ebenfalls behandelt, einschließlich einer Beschreibung, wie sich diese auf die Aufgabenplanung auswirken. Es können benutzerdefinierte Ansichten erstellt werden, um Aufgabenbeschränkungen anzuzeigen.

>[!VIDEO](https://video.tv.adobe.com/v/3435844/?captions=ger&quality=12&learn=on&enablevpops=1)

>[!IMPORTANT]
>
>Eine ausführlichere Erläuterung zu Dauertypen und Aufgabenbeschränkungen finden Sie unter [Verstehen und Verwalten von Dauertypen und Aufgabenbeschränkungen](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md).

## Die wichtigsten Punkte

* **Aufgabenverwaltung und -zuweisung** Übergeordnete Aufgaben gruppieren mehrere Unteraufgaben, die Aufgabengebieten und später Benutzern mit den erforderlichen Kenntnissen zugewiesen werden. &#x200B; Vorgänger geben sequenzielle Beziehungen an, während Aufgaben ohne Vorgänger parallel ausgeführt werden können. 
* **Gantt-Diagramm und Kritischer Pfad:** Das Gantt-Diagramm zeigt eine visuelle Zeitleiste des Projekts an, und die Funktion Kritischer Pfad zeigt Aufgaben auf, die das Projekt verzögern könnten, wenn sie verrutschen. &#x200B;
* **Ansichten und Überwachung:** Verschiedene Ansichten in Workfront, z. B. die Standardansicht für die Planung und die Statusansicht für die Überwachung, enthalten Flags für Fortschritt, Kommentare, Dokumente, Probleme, Genehmigungen, kritische Pfade und Meilensteine. Auch kürzlich durchgeführte Aktivitäten können verfolgt werden. 
* **Planungsoptionen:** Projekte können ab einem Start- oder Abschlussdatum geplant werden. Workfront berechnet die entsprechenden Termine anhand der Aufgabendauer und der Vorgänger. &#x200B; Planung ab einem Startdatum wird für kritische Abschlussdaten empfohlen, um gewisse Lücken zu schließen. 
* **Aufgabenbeschränkungen:** Aufgabenbeschränkungen wie „so bald wie möglich“ und „so spät wie möglich“ wirken sich auf die Aufgabenplanung aus. &#x200B; Das Ändern des Zeitplanmodus nach der Projekterstellung kann sich auf Aufgabenbeschränkungen und geplante Termine auswirken. &#x200B; können benutzerdefinierte Ansichten erstellt werden, um Aufgabenbeschränkungen anzuzeigen. 


## Was für und was gegen eine Änderung der Datumsangaben in Projektzeit-Timelines spricht

| VORTEILE (Datumsänderung) | NACHTEILE (Datumsänderung) | VORTEILE (keine Datumsänderung) | NACHTEILE (keine Datumsänderung) |
|---------------------------|---------------------------|---------------------------|---------------------------|
| <ul><li>Stressreduzierung/Kommunikation aktueller Erwartungen an Benutzende – „_Kreative wüssten nicht, was real ist_“</li><li>Präzise Ressourcenzuweisung, insbesondere im Workload Balancer</li><li>Verwenden von Berichten mit Journaleinträgen (oder zur Projektdauer), um auf Datumsänderungen hinzuweisen</li><li>Verwenden einer Bedingung, um anzuzeigen, ob das Projekt nicht wie geplant läuft</li><li>Hinzufügen eines benutzerdefinierten Formulars (oder Verwenden von Problemen) möglich, um Änderungen nachzuverfolgen – warum der Termin von wem und für wie lange verschoben wurde</li></ul> | <ul></li><li>Irreführende Daten, da Berichte nicht den wahren Zustand widerspiegeln</li><li>Falsche Wahrnehmung des Fortschritts – die Illusion, alles sei auf Kurs</li><li>Fördern einer Kultur, dass Timelines immer weiter nach hinten verschoben werden, anstatt die eigentlichen Ursachen anzugehen</li><li>Verlust des Vertrauens der Stakeholder oder der Wahrnehmung des Teams im Hinblick auf die Einhaltung von Fristen </li></ul> | <ul></li><li>Präzise Darstellung der Projekt-Timeline – Daten können für Analysen und zur genauen Schilderung des Geschehens verwendet werden</li><li>Option zum Ändern der Dauer oder Hinzufügen einer Verzögerung gegenüber Vorgänger</li><li>Einfaches Ermitteln möglicher Prozessverbesserungen für zukünftige Projektplanung und zukünftiges Risiko-Management</li><li>Option zur Nutzung von Baselines zum Erfassen des ursprünglichen Projektplans und zum Verwenden dieses Plans als Vergleich</li><li>Falls Personal fehlt, um Aufgaben in allen Bereichen zu erledigen, besser bleiben lassen</li></ul> | <ul></li><li>Verwirrung und/oder Frustration bei den Benutzenden – eine Fülle von „verspäteten“ Aufgaben, obwohl sie gerade erst benachrichtigt wurden</li><li>Ressourcen waren gemäß dem ursprünglichen Plan effektiv zugewiesen, sind jetzt aber aufgrund von Arbeitsverzögerungen überlastet</li><li>Projekt-Timeline kann nicht verwendet werden, um den Stakeholdern Aktualisierungen klar mitzuteilen</li></ul> |


## Empfohlene Tutorials zu diesem Thema

* [Verfolgen Sie den Fortschritt mit den Statuswerten „Prozent abgeschlossen“ und „Fortschritt“](/help/manage-work/project-timelines/track-work-progress-from-the-project-timeline.md)
* [Grundlegendes zu Datumstypen und zum Fortschrittsstatus](/help/manage-work/project-timelines/understand-task-dates-and-progress-status.md)
* [Master-Dauertypen und Aufgabenbeschränkungen](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)



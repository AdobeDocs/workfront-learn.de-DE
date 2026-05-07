---
title: Erkunden von Berichtskomponenten in Workfront
description: Die Reporting-Komponenten von Workfront verfeinern die Datenvisualisierung mit objektbasierten Filtern, dynamischen Ansichten, strukturierten Gruppierungen und Platzhalterfunktionen für maßgeschneiderte Erkenntnisse.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: '2025-04-28T00:00:00.000Z'
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:18:15.845Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 539
ht-degree: 54%

---

# Erkunden von Berichtskomponenten in Workfront

In diesem Video wird das Konzept der Reporting-Komponenten in Workfront beschrieben, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. Zu den wichtigsten Komponenten zählen:

* **Objekttyp:** Gibt das Workfront-Objekt an, das verarbeitet wird, z. B. ein Projekt, eine Aufgabe oder einen Stundeneintrag. &#x200B; Filter, Ansichten und Gruppierungen sind spezifisch für den Objekttyp. &#x200B;
* **Source-Feld und Feldname:** Die Feldquelle ist das Element in Workfront, an das Informationen angehängt sind, und der Feldname ist die spezifische Information (z. B. „Beschreibung“ für ein Projekt). &#x200B;
* **Wertfeld** Stellt den Inhalt eines Felds dar, z. B. „niedrig“, „normal“, „hoch“ oder „dringend“ für das Prioritätsfeld. &#x200B;
* **Filterkennzeichner:**, welche Werte in einen Bericht ein- oder ausgeschlossen werden sollen, z. B. das Anzeigen von Aufgaben mit der Priorität „Hoch“. &#x200B;


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on&enablevpops=0)

## Wichtige Schlussfolgerungen

* **Reporting-Komponenten:** Zu den Reporting-Komponenten in Workfront gehören Objekttyp, Feldquelle, Feldname, Filterqualifizierer und Wertfelder, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. &#x200B;
* **Objekttyp-Spezifität:** Filter, Ansichten und Gruppierungen sind an bestimmte Objekttypen wie Projekte, Aufgaben oder Stundeneinträge gebunden, sodass Berichte auf die relevanten Daten zugeschnitten sind. &#x200B;
* **Filterregeln:** Filter verwenden Feldquelle, Feldnamen, Kennzeichner und Werte, um Kriterien zu definieren. &#x200B;. B. zeigt der Filter „Meine Projekte“ nur aktuelle Projekte an, bei denen der angemeldete Benutzer Teil des Projektteams ist. &#x200B;
* **Ansichten und Gruppierungen:** Ansichten zeigen Kombinationen aus Feldquelle und Feldname in Spalten an (z. B. „Name des Inhabers„), während Gruppierungen Daten basierend auf bestimmten Kriterien organisieren (z. B. „Firmenname„). &#x200B;
* **Platzhalterverwendung:** Platzhalter in Filtern ermöglichen eine dynamische Zuordnung, z. B. die Identifizierung angemeldeter Benutzer innerhalb eines Projektteams und eine bessere Personalisierung des Reportings. &#x200B;

## Kurzer Überblick zu Reporting-Komponenten

![Ein Screenshot des Bildschirms zum Erstellen eines Filters](assets/reporting-components-1.png)

**A – Feldquelle**

Die Optionen für die Feldquelle hängen vom ausgewählten Objekttyp ab. Häufig ist die Feldquelle das Element in Workfront, zu dem eine bestimmte Information (d. h. der Feldname) gehört. Manchmal ist die Feldquelle mit dem Objekttyp identisch.
Die Feldquelle bestimmt, welche Feldnamen verfügbar sind.

Beispiele: [!UICONTROL Projekt], [!UICONTROL Aufgabe], [!UICONTROL Problem], [!UICONTROL Zugewiesen an]

**B – Feldname**

Feldnamen sind Informationen, die für die ausgewählte Feldquelle verfügbar sind.

Dabei kann es sich um von Ihnen ausgefüllte Workfront-Felder, Felder aus einem benutzerdefinierten Formular oder Informationen handeln, die von Workfront automatisch erfasst werden.

Feldnamen steuern die Optionen des Wertfeldes.

Beispiele: [!UICONTROL Fortschrittsstatus], [!UICONTROL Beschreibung], [!UICONTROL Geplantes Abschlussdatum], Benutzerdefinierte Formularfelder

**C – Filterqualifizierer**

Filterqualifizierer helfen bei der Eingrenzung der möglichen Ergebnisse, die unter der ausgewählten Feldquelle und dem ausgewählten Feldnamen angezeigt werden können.

Sie geben an, wie die Feldquelle und der Feldname mit dem Wertfeld in Beziehung stehen.

Beispiele: Gleich, Enthält, Null, Weniger als

**D – Wert**

Der Wert ist die Information, die in das Feld eingegeben wird, das durch den Feldnamen spezifiziert wird.

Die Optionen für den Wert werden durch die Feldquelle und den Feldnamen bestimmt.

Im Wert können Platzhalter für Benutzende und Daten sowie Freiformtext verwendet werden.

Beispiele: Neu, Aktuell, $$TODAYbw, Beschreibung

>[!TIP]
>
>Weitere Informationen zu bestimmten Feldnamen in Workfront finden Sie im [Glossar der Adobe Workfront-Terminologie](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=de).


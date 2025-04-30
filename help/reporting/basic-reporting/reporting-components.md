---
title: Grundlegendes zu Reporting-Komponenten
description: Die Berichtskomponenten von Workfront verfeinern die Datenvisualisierung mit objektbasierten Filtern, dynamischen Ansichten, strukturierten Gruppierungen und Platzhalterfunktionen für maßgeschneiderte Einblicke.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: 2025-04-28T00:00:00Z
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: af53d11fcf3e81c8ea0176f4db9dcec77e9195ed
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 45%

---

# Grundlegendes zu Reporting-Komponenten

In diesem Video wird das Konzept der Reporting-Komponenten in Workfront erläutert, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. Zu den wichtigsten Komponenten gehören:

* **Objekttyp:** Gibt das Workfront-Objekt an, das verarbeitet wird, z. B. ein Projekt, eine Aufgabe oder einen Stundeneintrag. &#x200B; Filter, Ansichten und Gruppierungen sind spezifisch für den Objekttyp. &#x200B;
* **Source-Feld und Feldname:** Die Feldquelle ist das Element in Workfront, an das Informationen angehängt sind, und der Feldname ist die spezifische Information (z. B. „Beschreibung“ für ein Projekt). &#x200B;
* **Wertfeld** Stellt den Inhalt eines Felds dar, z. B. „niedrig“, „normal“, „hoch“ oder „dringend“ für das Prioritätsfeld. &#x200B;
* **Filterkennzeichner:** Definiert, welche Werte in einen Bericht ein- oder ausgeschlossen werden sollen, z. B. das Anzeigen von Aufgaben mit der Priorität „Hoch“. &#x200B;


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on)

## Die wichtigsten Punkte

* **Reporting-Komponenten:** Zu den Reporting-Komponenten in Workfront gehören Objekttyp, Feldquelle, Feldname, Filterqualifizierer und Wertfelder, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. &#x200B;
* **Objekttyp-Spezifität:** Filter, Ansichten und Gruppierungen sind an bestimmte Objekttypen wie Projekte, Aufgaben oder Stundeneinträge gebunden, sodass Berichte auf die relevanten Daten zugeschnitten sind. &#x200B;
* **Filterregeln:** Filter verwenden Feldquelle, Feldnamen, Kennzeichner und Werte, um Kriterien zu definieren. &#x200B; Der Filter „Meine Projekte“ zeigt beispielsweise nur aktuelle Projekte an, bei denen der angemeldete Benutzer Teil des Projektteams ist. &#x200B;
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


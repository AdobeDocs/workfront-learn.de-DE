---
title: Grundlegendes zu Reporting-Komponenten
description: Die Reporting-Komponenten von Workfront verfeinern die Datenvisualisierung mit objektbasierten Filtern, dynamischen Ansichten, strukturierten Gruppierungen und Platzhalterfunktionen für maßgeschneiderte Erkenntnisse.
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
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 100%

---

# Grundlegendes zu Reporting-Komponenten

In diesem Video wird das Konzept der Reporting-Komponenten in Workfront beschrieben, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. Zu den wichtigsten Komponenten zählen:

* **Objekttyp:** Gibt das Workfront-Objekt an, das verarbeitet wird, z. B. ein Projekt, eine Aufgabe oder ein Stundeneintrag. Filter, Ansichten und Gruppierungen sind spezifisch für den Objekttyp.
* **Feldquelle und Feldname:** Die Feldquelle ist das Element in Workfront, an das Informationen angehängt sind, und der Feldname ist die spezifische Information (z. B. „Beschreibung“ für ein Projekt). 
* **Wertefeld:** Stellt den Inhalt eines Felds dar, z. B. „Niedrig“, „Normal“, „Hoch“ oder „Dringend“ für das Prioritätsfeld. 
* **Filterqualifizierer:** Definiert, welche Werte in einen Bericht ein- oder daraus ausgeschlossen werden sollen, z. B. das Anzeigen von Aufgaben mit der Priorität „Hoch“.


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on&enablevpops=0)

## Die wichtigsten Punkte

* **Reporting-Komponenten:** Zu den Reporting-Komponenten in Workfront gehören Objekttyp, Feldquelle, Feldname, Filterqualifizierer und Wertfelder, die für die Erstellung von Filtern, Ansichten und Gruppierungen unverzichtbar sind. 
* **Objekttyp-Spezifität:** Filter, Ansichten und Gruppierungen sind an bestimmte Objekttypen wie Projekte, Aufgaben oder Stundeneinträge gebunden, um sicherzustellen, dass Berichte auf die relevanten Daten zugeschnitten werden.
* **Filterregeln:** Filter verwenden Feldquelle, Feldnamen, Qualifizierer und Werte, um Kriterien zu definieren. Der Filter „Meine Projekte“ zeigt beispielsweise nur aktuelle Projekte an, bei denen die angemeldete Person Teil des Projekt-Teams sind.
* **Ansichten und Gruppierungen:** Ansichten zeigen Kombinationen aus Feldquelle und Feldname in Spalten an (z. B. „Name des Inhabers“), während Gruppierungen Daten basierend auf bestimmten Kriterien organisieren (z. B. „Firmenname“).
* **Verwendung von Platzhaltern:** Platzhalter in Filtern ermöglichen eine dynamische Zuordnung, z. B. die Identifizierung angemeldeter Benutzender innerhalb eines Projekt-Teams, wodurch die Personalisierung beim Reporting optimiert wird. 

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


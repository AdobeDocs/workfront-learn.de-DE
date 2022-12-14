---
title: Grundlegendes zur Navigation und Überprüfung von Projekten in [!UICONTROL Verbesserte Analytics]
description: Erfahren Sie, wie Sie die Flugplan-Grafik in Workfront lesen.
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Grundlegendes zur Navigation und Überprüfung von Projekten in [!UICONTROL Verbesserte Analytics]

In diesem Video erfahren Sie:

* So lesen Sie die Flugplan-Grafik

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12)

## Flugplan-Diagramm

![Ein Bild eines Flugplan-Diagramms mit Zahlen, die den unten stehenden Aufzählungszeichen entsprechen](assets/section-2-1.png)

Im Diagramm sehen Sie Folgendes:

1. Die Projektnamen befinden sich auf der linken Seite.
1. Die Datumsangaben werden unten angezeigt.
1. Die vertikale blaue Linie zeigt das spezifische Datum an, an dem die Maus bewegt wird.
1. Horizontale blaue Linien zeigen das geplante Start- und Enddatum des Projekts an.
1. Grüne Linien zeigen an, dass das Projekt On Target ist.
1. Orangefarbene Linien weisen darauf hin, dass das Projekt gefährdet ist.
1. Rote Linien zeigen an, dass das Projekt in Schwierigkeiten ist.

Wenn Sie diese Informationen zu Ihren Projekten anzeigen, können Sie Folgendes feststellen:

* Welche Ereignisse verlängern ein Projekt nach dem geplanten Abschlussdatum.
* Wenn bei einem Projekt Probleme auftreten.
* Wie viele Projekte im selben Zeitraum geöffnet sind.
* Anzahl der aktiven Projekte.
* Welche Projekte benötigen besondere Aufmerksamkeit oder Unterstützung?

## Bedingung basiert auf dem Fortschrittsstatus

Die Projektbedingung ist eine visuelle Darstellung des Projektfortschritts. Workfront bestimmt die Bedingung anhand des Fortschrittsstatus von Aufgaben innerhalb des Projekts.

![Ein Bild möglicher Fortschrittsstatus](assets/section-2-2.png)

Die Bedingung eines Projekts kann festgelegt werden:

* **Manuell** durch Benutzer mit Zugriff auf das Projekt, wenn der Bedingungstyp des Projekts auf &quot;Manuell&quot;festgelegt ist. Dadurch können Sie die Bedingung des Projekts unabhängig vom kritischen Pfad festlegen.
* **Automatisch** von Workfront, wenn der Bedingungstyp des Projekts auf Fortschrittsstatus gesetzt ist.

Workfront empfiehlt, den Bedingungstyp auf Fortschrittsstatus festzulegen, damit Sie anhand des Fortschritts Ihrer Aufgaben einen klaren Hinweis auf den tatsächlichen Fortschritt des Projekts erhalten.

![Ein Bild möglicher Fortschrittsstatus](assets/section-2-3.png)

In diesem Fall kann die Projektbedingung wie folgt lauten:

* **In Target**—Wenn der Fortschrittsstatus der letzten Aufgabe auf dem kritischen Pfad &quot;Einschaltzeit&quot;lautet, lautet die Bedingung des Projekts &quot;On Target&quot;. Das Projekt ist auf dem richtigen Weg, um es planmäßig fertigzustellen.
* **Risiko**—Wenn der Fortschrittsstatus der letzten Aufgabe auf dem kritischen Pfad &quot;Hinter&quot;oder &quot;Risiko&quot;lautet, ist die Bedingung des Projekts &quot;In Gefahr&quot;. Das Projekt ist auf dem Weg zu Ende zu sein, aber noch nicht zu spät.
* **In Schwierigkeiten**—Wenn der Fortschrittsstatus der letzten Aufgabe auf dem kritischen Pfad &quot;Late&quot;ist, ist die Bedingung des Projekts &quot;In Schwierigkeiten&quot;. Das Fälligkeitsdatum liegt in der Vergangenheit und das Projekt ist jetzt zu spät.

>[!NOTE]
>
>Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie mehr als drei Optionen finden können oder die Namen sich von denen oben unterscheiden können. Informationen zum Anpassen von Bedingungen finden Sie im Artikel Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung .

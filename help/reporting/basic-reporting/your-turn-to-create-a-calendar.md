---
title: 'Aktivität: Erstellen eines Kalenderberichts'
description: Schrittweise Anweisungen zum Erstellen eines Kundenkalenders, der Ihre nicht abgeschlossenen Aufgaben und Probleme anzeigt.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
last-substantial-update: '2025-06-23T00:00:00.000Z'
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: c6584858-4838-4ce3-ab7f-7292f37179f4
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:16:18.343Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 100%

---

# Aktivität: Erstellen eines Kalenderberichts

Erstellen Sie einen Kundenkalender mit dem Namen „Meine nicht abgeschlossene Arbeit“.

Fügen Sie eine Kalendergruppe mit dem Namen „Nicht abgeschlossene Aufgaben“ ein, in der alle unvollständigen Aufgaben angezeigt werden, die Ihnen unter „Aktuelle Projekte“ zugewiesen sind.

Wählen Sie als Farbe für diese Elemente Rot aus.

Fügen Sie eine weitere Kalendergruppe mit dem Namen „Nicht abgeschlossene Probleme“ hinzu, die alle nicht abgeschlossenen Probleme enthält, die Ihnen unter „Aktuelle Projekte“ zugewiesen sind. Wählen Sie als Farbe für diese Elemente Blau aus.

## Antwort

1. Navigieren Sie im Hauptmenü zum Bereich „Kalender“.
1. Klicken Sie auf die Schaltfläche „Neuer Kalender“ und nennen Sie den Kalender „Meine nicht abgeschlossene Arbeit“.
1. Klicken Sie auf die Schaltfläche „Dem Kalender hinzufügen“ und dann auf „Weitere Objekte hinzufügen“.
1. Nennen Sie im sich öffnenden Fenster „Elemente zum Kalender hinzufügen“ die Gruppe „Nicht abgeschlossene Aufgaben“.
1. Wählen Sie als Farbe Rot aus.
1. Ändern Sie das Datumsfeld zu „Geplante Datumsangaben“.
1. Legen Sie das Feld „Im Kalender dieses Feld anzeigen“ auf „Enddatum“ fest.
1. Setzen Sie das Feld „Wenn verfügbar, zu tatsächlichen Daten wechseln“ auf „Nein“.
1. Wählen Sie im Abschnitt „Was möchten Sie zum Kalender hinzufügen?“ die Option „Aufgaben“ aus. Klicken Sie dann auf die Schaltfläche „Aufgaben hinzufügen“.
1. Fügen Sie drei Filterregeln hinzu:

   * Projekt > Status entspricht > Gleich > Aktuell
   * Arbeitsauftrag – Benutzer > ID > Gleich > $$USER.ID
   * Aufgabe > Ist abgeschlossen > Gleich > Falsch

1. Klicken Sie auf Speichern.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Elementen zu einem Kalender](assets/calendar-activity-1.png)

1. Erstellen Sie eine zweite Gruppierung, indem Sie auf „Dem Kalender hinzufügen“ und dann auf „Weitere Objekte hinzufügen“ klicken.
1. Nennen Sie in dem sich öffnenden Fenster „Elemente zum Kalender hinzufügen“ die Gruppe „Nicht abgeschlossene Probleme“.
1. Wählen Sie als Farbe Blau aus.
1. Ändern Sie das Datumsfeld zu „Geplante Datumsangaben“.
1. Legen Sie das Feld „Im Kalender dieses Feld anzeigen“ auf „Enddatum“ fest.
1. Setzen Sie das Feld „Wenn verfügbar, zu tatsächlichen Daten wechseln“ auf „Nein“.
1. Wählen Sie im Abschnitt „Was möchten Sie zum Kalender hinzufügen?“ die Option „Probleme“ aus. Klicken Sie dann auf die Schaltfläche „Probleme hinzufügen“.
1. Fügen Sie die folgenden drei Filterregeln hinzu:

   * Projekt > Status entspricht > Gleich > Aktuell
   * Arbeitsauftrag – Benutzer > ID > Gleich > $$USER.ID
   * Problem > Ist abgeschlossen > Gleich > Falsch

1. Klicken Sie auf Speichern.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Elementen zu einem Kalender](assets/calendar-activity-2.png)

Da Sie „$$USER.ID“ in den Filtern verwendet haben, können Sie diesen Kalender für andere freigeben, sodass sie ihre eigenen unvollständigen Aufgaben und Probleme sehen können.

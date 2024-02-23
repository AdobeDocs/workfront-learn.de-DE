---
title: Übung zu Aspekten über die grundlegende Zuordnung hinaus
description: Erfahren Sie, wie Sie Felder, die an ein Modul gesendet werden, mit den Formeln des Zuordnungsfelds bearbeiten und konvertieren können.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,noCatalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '314'
ht-degree: 100%

---

# Übung zu Aspekten über die grundlegende Zuordnung hinaus

Erfahren Sie, wie Sie Felder, die an ein Modul gesendet werden, mit den Formeln des Zuordnungsfelds bearbeiten und konvertieren können.

## Übungsübersicht

Ändern Sie den Projektnamen, das geplante Startdatum und die Priorität aus der Übung „Weiterführende Zuordnung – Walkthrough“ mithilfe der Formeln im Zuordnungsfeld.

![Weiterführende Zuordnung Bild 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Zu befolgende Schritte

**Erstellen Sie einen Klon Ihres Szenarios für den Entwurf des Anfangsszenarios.**

1. Wählen Sie die Option „Klonen“ rechts neben dem Entwurf des Ausgangsszenarios im Abschnitt „Szenario“, wie unten dargestellt. Nennen Sie es „Weiterführende Zuordnung“.

   ![Weiterführende Zuordnung Bild 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Jetzt werden wir das Zuordnungsfeld im Modul „Workfront-Projekte erstellen“ verwenden, um den Projektnamen, das geplante Startdatum und die Prioritätsfelder zu konfigurieren.**

1. Klicken Sie auf das Modul „Workfront-Projekte erstellen“, um die Einstellungen zu bearbeiten. Ändern Sie im Zuordnungsfeld das Feld „Name“ in [Mein Projektname] nach [Sponsor] um.

   + Die [Mein Projektname] ist Spalte 1 des Moduls „CSV-Analyse“ und [Sponsor] ist Spalte 6. Das Wort „nach“ wird einfach zwischen die beiden geschrieben.

1. Gehen Sie dann zu „Geplanter Starttermin“ und verwenden Sie die Formel „addDays“, um zum Feld 15 Tage hinzuzufügen, wie in dem Video „Weiterführende Zuordnung“ beschrieben.
1. Suchen Sie das Feld „Priorität“ und aktivieren Sie die Schaltfläche „Zuordnen“ oben rechts im Feld. Das Auswahllisten-Menü ändert sich in eine Zahl. Erstellen Sie eine if-Anweisung, um ein Projekt als hohe Priorität (4) zu kennzeichnen, wenn die Vertrauenseinstufung in der CSV-Datei weniger als 100 beträgt, andernfalls kann es als normal (2) eingestuft werden.

   + Die Vertrauensbewertung ist in Spalte 4 enthalten.

   **An dieser Stelle sollte Ihr Zuordnungsfeld wie folgt aussehen:**

   ![Weiterführende Zuordnung Bild 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Klicken Sie auf „OK“ und dann auf „Einmalig ausführen“.
1. Suchen Sie das Projekt in Ihrer Workfront-Instanz, um sicherzustellen, dass alles korrekt zugeordnet wurde.
1. Speichern Sie Ihr Szenario.

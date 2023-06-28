---
title: Einführung in die Übung "iterators"
description: Erfahren Sie, wie Sie Auflistungs-Apps verwenden und Aktionen für jedes Informationsbündel durchführen können.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Einführung in Iteratoren

Erfahren Sie, wie Sie Auflistungs-Apps verwenden und Aktionen für jedes Informationsbündel durchführen können.

## Übungsübersicht

Sehen Sie sich ein bestimmtes Projekt in Workfront an und sehen Sie sich dann alle Aufgaben in diesem Projekt an. Sie verwenden das Inkrement-Tool-Modul, um die Anzahl der Aufgaben innerhalb des Projekts zu zählen. Schließlich verwenden Sie das Variablenmodul Set , um die Anzahl der untergeordneten Elemente von der Anzahl der offenen Probleme zu subtrahieren und für jedes der Aufgabenbundles einen numerischen Wert zu generieren.

![Einführung in Iteratoren Bild 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

**Lesen Sie ein Projekt und zugehörige Aufgaben.**

1. Starten Sie ein neues Szenario. Nennen Sie es &quot;Einführung in die Iteration&quot;.
1. Wählen Sie Workfront als Trigger-Modul und lesen Sie einen Datensatz.
1. Wählen Sie für &quot;Record Type&quot;die Option &quot;Project&quot;.
1. Wählen Sie für Ausgaben ID, Name und Beschreibung aus.
1. Geben Sie im Feld ID die Projekt-ID des Northstar Fashion Exhibitors Booth-Projekts von Ihrer Workfront-Testlaufwerksinstanz ein.
1. Benennen Sie dieses Modul &quot;WF-Projekte suchen&quot;um.
1. Fügen Sie ein weiteres Workfront-Modul hinzu, um die Aufgaben im Zusammenhang mit diesem Projekt zu lesen. Wählen Sie das Modul Verwandte Datensätze lesen aus.
1. Wählen Sie für &quot;Record Type&quot;die Option &quot;Project&quot;.
1. Wählen Sie für die übergeordnete Datensatz-ID die ID aus dem Modul Datensatz lesen aus.
1. Wählen Sie für Sammlungen die Option &quot;Aufgaben&quot;.
1. Wählen Sie für Ausgaben ID, Name, Beschreibung, Anzahl der untergeordneten Elemente, Anzahl offener Probleme und Arbeit aus.
1. Benennen Sie dieses Modul &quot;Aufgaben des Projekts lesen&quot;um.
1. Speichern Sie das Szenario und klicken Sie dann auf Einmal ausführen , um die Ausgaben anzuzeigen.

   + Klicken Sie auf den Ausführungsinspektor und Sie sehen ein Bundle als Eingabe (das Projekt) und 28 Bundles als Ausgabe (die Aufgaben).

   **Zählung und Verarbeitung iterierter Bundles.**

1. Fügen Sie ein weiteres Modul nach Read Related Records hinzu. Wählen Sie ein Tool-Modul für Inkrementierungs-Funktionen.

   + Belassen Sie das Feld Wert zurücksetzen auf Nie und klicken Sie auf OK.

1. Benennen Sie dieses Modul um &quot;Zählung der Anzahl der Aufgaben&quot;.
1. Fügen Sie ein Set-Variablenmodul hinzu. Setzen Sie den Variablennamen auf &quot;Zufällige Übereinstimmung&quot;.
1. Ziehen Sie im Feld Variablenwert die Anzahl offener untergeordneter Elemente von der Anzahl offener opTasks ab.

   **Sie sollte wie folgt aussehen:**

   ![Einführung in Iteratoren Bild 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Benennen Sie dieses Modul &quot;Random Math&quot;um.
1. Speichern Sie das Szenario und klicken Sie einmal auf Ausführen .

Für jede vom Iterator Read Related Records erzeugte Aufgabe führte Workfront Fusion 28 Ausführungen durch. Diese 28 Bundles werden während des gesamten Szenarios weiterhin verarbeitet, es sei denn, zum Schließen des Kreislaufs wird ein Aggregator hinzugefügt.

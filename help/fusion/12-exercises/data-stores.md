---
title: Datenspeicher
description: Erfahren Sie, wie Sie Firmennamen zwischen zwei Systemen synchronisieren. (Sollte zwischen 60 und 160 Zeichen lang sein, ist jedoch 59 Zeichen lang)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '878'
ht-degree: 100%

---

# Datenspeicher

Erfahren Sie, wie Sie Firmennamen zwischen zwei Systemen synchronisieren.

## Übungsübersicht

Dies ist der erste Teil einer unidirektionalen Synchronisierung von Firmen in Workfront und einem anderen System. Derzeit wird nur zwischen einem Fusion-Datenspeicher und Workfront synchronisiert. Eine Tabelle in einem Datenspeicher verfolgt die Workfront-ID (WFID) und die Firmen-ID in der CSV-Datei (CID) für jede Firma. Dies ermöglicht eine bidirektionale Synchronisierung zu einem späteren Zeitpunkt.

![Datenspeicher – Bild 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Zu befolgende Schritte

**Laden Sie die Datei von Workfront herunter.**

1. Wählen Sie im Ordner „Fusion-Übungsdateien“ die Datei „_Companies.csv“ aus und klicken Sie auf „Dokumentdetails“.
1. Kopieren Sie die erste ID-Nummer aus der URL-Adresse.
1. Erstellen Sie in Fusion ein neues Szenario mit dem Namen „Datenspeicher zur Datensynchronisierung verwenden“.
1. Wählen Sie als Trigger-Modul das Workfront-Modul „Dokument herunterladen“ aus.
1. Richten Sie Ihre Workfront-Verbindung ein und fügen Sie die Dokument-ID ein, die Sie aus der Workfront-URL kopiert haben.
1. Nennen Sie dieses Modul „Firmendatei abrufen“.
1. Fügen Sie jetzt das Modul „CSV-Analyse“ hinzu.
1. Geben Sie für das Feld „Spaltenanzahl“ den Wert 2 ein.
1. Ordnen Sie Daten aus dem Modul „Dokument herunterladen“ im CSV-Feld zu.
1. Nennen Sie dieses Modul „Firmendatei analysieren“.
1. Speichern Sie das Szenario und klicken Sie auf „Einmal ausführen“.

   **Erstellen Sie einen Datenspeicher und eine Datenstruktur.**

1. Fügen Sie das Datenspeicher-Modul „Einträge suchen“ hinzu.
1. Erstellen Sie einen neuen Datenspeicher mit dem Namen „Firmensynchronisierung“.
1. Erstellen Sie im Datenspeicher eine Datenstruktur mit dem Namen „Firmensynchronisierung (Struktur)“.
1. Erstellen Sie vier Felder.

   + CID – Die Firmen-ID in der CSV-Datei
   + Firmenname
   + WFID – Die Firmen-ID in Workfront
   + Erstellungsdatum – Stellen Sie sicher, dass der Datentyp „Datum“ ist

   ![Datenspeicher – Bild 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Klicken Sie für die Datenstruktur auf „Speichern“, legen Sie dann die Datenspeichergröße auf 1 fest und speichern Sie den Datenspeicher.
1. Weiter im Datenspeicher-Modul: Richten Sie einen Filter ein, dass die CID mit der Firmen-ID aus dem Modul „CSV-Analyse“ (Spalte 1) übereinstimmen soll.
1. Klicken Sie auf „Erweiterte Einstellungen anzeigen“ und wählen Sie die Option „Ausführung des Szenarios oder der Route fortsetzen, auch wenn dieses Modul keine Ergebnisse zurückgibt“.

   ![Datenspeicher – Bild 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Benennen Sie dieses Modul in „Firmen abgleichen“ um.
1. Fügen Sie das Workfront-Modul „Einträge suchen“ hinzu.
1. Wählen Sie als Eintragstyp „Firma“ aus.
1. Das Suchkriterium ist, dass der Firmenname in Workfront gleich dem Firmenname in der CSV-Datei ist.
1. Wählen Sie für Ausgaben den Firmennamen und die ID aus.

   ![Datenspeicher – Bild 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Klicken Sie auf „OK“ und benennen Sie dieses Modul in „Firmen abgleichen“ um.

   **Erstellen Sie unterschiedliche Pfade, je nachdem, ob die Firma in Workfront oder im Datenspeicher vorhanden ist.**

   **Routing-Pfad 1 – Erstellen einer Firma.**

1. Fügen Sie rechts neben dem Workfront-Modul „Einträge suchen“ ein Router-Modul hinzu.
1. Fügen Sie dem obersten Pfad das Workfront-Modul „Eintrag erstellen“ hinzu.
1. Setzen Sie den Eintragstyp auf „Firma“.
1. Wählen Sie „Name“ aus den zuzuordnenden Feldern aus. Ordnen Sie das Namensfeld der Ausgabe aus dem Modul „CSV-Analyse“ (Spalte 2) zu.
1. Benennen Sie dieses Modul in „Firma erstellen“ um.

   ![Datenspeicher – Bild 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Fügen Sie nach dem Router einen Filter hinzu, damit eine Firma nur erstellt wird, wenn sie noch nicht in Workfront vorhanden ist. Nennen Sie ihn „Nicht in Workfront“.
1. Legen Sie die Bedingung auf die ID aus dem Workfront-Modul „Suchen“ und auf „existiert nicht“ fest.

   ![Datenspeicher – Bild 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Im nächsten Pfad werden Sie den Datenspeicher aktualisieren.**

1. Fügen Sie am Ende des obersten Pfads das Modul „Variable festlegen“ hinzu.
1. Legen Sie den Variablennamen auf „Workfront-ID“ fest.
1. Legen Sie den Variablenwert auf die ID aus dem Modul „Firma erstellen“ fest.
1. Benennen Sie dieses Modul in „Workfront-ID festlegen“ um.

   **Routing-Pfad 2 – Aktualisieren des Datenspeichers.**

1. Erstellen Sie einen Filter für Routing-Pfad 2. Nennen Sie ihn „Nicht im Datenspeicher“.

1. Legen Sie die Bedingung auf den Schlüssel aus dem Modul „Datenspeicher“ und auf „existiert nicht“ fest.

   ![Datenspeicher – Bild 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. Das erste Modul in diesem Pfad ist das Modul „Variable abrufen“.
1. Legen Sie den Variablennamen auf „Workfront-ID“ fest.
1. Benennen Sie dieses Modul in „Workfront-ID abrufen“ um.
1. Fügen Sie ein weiteres Modul aus der Datenspeicher-App hinzu: „Eintrag hinzufügen/ersetzen“.
1. Wählen Sie im Feld „Datenspeicher“ die Option „Firmensynchronisierung“ aus. Dies ist der Datenspeicher, den Sie zuvor erstellt haben.
1. Lassen Sie das Feld „Schlüssel“ leer.
1. Ordnen Sie das CID-Feld aus Spalte 1 im Modul „CSV-Analyse“ zu.
1. Ordnen Sie das Feld „Firmenname“ aus Spalte 2 im Modul „CSV-Analyse“ zu.
1. Ordnen Sie das Feld „WFID“ aus dem Modul „Workfront-ID abrufen“ zu.
1. Verwenden Sie für das Feld „Erstellungsdatum“ die Funktion „formatDate“ von der Registerkarte „Datum und Uhrzeit“, um das aktuelle Datum als MM/TT/JJJJ zu formatieren.

   ![Datenspeicher – Bild 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Klicken Sie auf „OK“ und benennen Sie dieses Modul in „Firmeneintrag erstellen“ um.

   **Routing-Pfad 3 – Synchronisieren des Datenspeichers zwischen Systemen.**

1. Erstellen Sie zunächst einen Filter für Routing-Pfad 3. Nennen Sie ihn „Firma vorhanden, nicht im Datenspeicher“.
1. Legen Sie die Bedingung auf den Schlüssel aus dem Datenspeicher-Modul „Einträge suchen“ und „existiert nicht“ fest.
1. Klicken Sie auf die Schaltfläche „UND-Regel hinzufügen“ und geben Sie an, dass der Firmenname aus der CSV-Datei (Spalte 2) dem Firmennamen aus dem Workfront-Modul „Suchen“ entspricht.

   ![Datenspeicher – Bild 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Fügen Sie nun ein weiteres Modul, „Eintrag hinzufügen/ersetzen“, hinzu, indem Sie das Modul am Ende des Routing-Pfads 2 klonen.
1. Ziehen Sie das geklonte Modul am Ende des Routing-Pfads 3 an die vorgesehene Stelle. Löschen Sie das leere Modul, das dort vorhanden war.
1. Klicken Sie auf das geklonte Modul. Alle Felder sollten gleich bleiben, mit Ausnahme des Felds „WFID“. Ordnen Sie es aus dem Suchmodul „Firmen abgleichen“ zu.

   ![Datenspeicher – Bild 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Klicken Sie auf „OK“ und benennen Sie dieses Modul in „Firmeneintrag erstellen“ um.

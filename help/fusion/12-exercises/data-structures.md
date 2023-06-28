---
title: Datenstrukturen
description: Umwandeln von Daten aus einer Quelldatei in eine Zieldatei. (Sollte zwischen 60 und 160 Zeichen lang sein, jedoch 58 Zeichen lang sein)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11054
thumbnail: KT11054.png
exl-id: 06a39a87-23f3-4d4a-995e-d32fb9c5f50d
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Datenstrukturen

Umwandeln von Daten aus einer Quelldatei in eine Zieldatei.

## Übungsübersicht

Öffnen Sie eine CSV-Datei, die eine Liste mit Zeiteinträgen enthält. Diese Zeiteinträge beziehen sich auf Minuten, die von mehreren Benutzern an bestimmten Tagen protokolliert werden. Ziel ist es, diese Informationen zu nehmen und eine neue CSV-Datei zu erstellen, die die Gesamtzeit (in Stunden) anzeigt, die jeder Benutzer täglich protokolliert.

![Datenstrukturen Bild 1](../12-exercises/assets/data-structures-walkthrough-1.png)

![Datenstrukturen Bild 2](../12-exercises/assets/data-structures-walkthrough-2.png)


In diesem Szenario öffnen Sie eine Datei mit einer Liste der Zeiteinträge für die Minuten, in denen gearbeitet wurde, einschließlich Datum und Uhrzeit, Anzahl der Minuten und E-Mail-Adresse des Einsenders. Es gibt 100 Zeiteinträge, von denen einige von denselben Personen gemacht wurden und einige am selben Tag wie andere.

Gehen Sie wie folgt vor, um eine Datei zu erstellen, die die Gesamtzeit (in Stunden) anzeigt, die jeder einzelne Tag verbringt:

1. Rufen Sie im Trigger-Modul eine -Datei aus dem Ordner &quot;Workfront&quot;ab. Laden Sie die Datei herunter.
1. Im ersten CSV-Modul analysieren Sie die Zeiteingabedaten, um für jeden Zeiteintrag ein Bundle auszugeben. Das ist ein Iterator.
1. Das erste Tool-Modul ist ein numerischer Aggregator. Dadurch werden alle Minuten SUM und die Zeilen nach E-Mail-Adresse und dann nach Datum gruppiert. Das Ergebnis ist die Gesamtzahl der täglich verarbeiteten Minuten nach E-Mail-Adresse.
1. Das zweite Tool-Modul ist ein Set Variable-Modul. Auf diese Weise können Sie die Minuten so formatieren, dass sie durch 60 und 2 Dezimalstellen geteilt werden.
1. Richten Sie im zweiten CSV-Modul die Ausgabedatei ein.
1. Laden Sie im endgültigen Modul die CSV-Datei in Workfront hoch.

## Schritte, die ausgeführt werden müssen

**Laden Sie die Datei von Workfront herunter.**

1. Wählen Sie im Ordner &quot;Fusion Exercise Files&quot;von Workfront die Option &quot;_Fusion1.0JanTime.csv&quot;und klicken Sie auf &quot;Document Details&quot;.
1. Kopieren Sie die erste ID-Nummer aus der URL-Adresse.
1. Erstellen Sie ein neues Szenario. Nennen Sie es &quot;Erstellen und Verwenden von Datenstrukturen&quot;.
1. Beginnen Sie mit dem Modul Dokument von der Workfront-App herunterladen .
1. Richten Sie Ihre Workfront-Verbindung ein und fügen Sie die Dokument-ID ein, die Sie aus der Workfront-URL kopiert haben.

   ![Datenstrukturen Bild 3](../12-exercises/assets/data-structures-walkthrough-3.png)

   **Analysieren Sie die Zeiteingabedaten.**

1. Fügen Sie ein weiteres Modul hinzu, indem Sie CSV analysieren auswählen.
1. Richten Sie die CSV-Analyse für 7 Spalten ein. Aktivieren Sie das Kontrollkästchen CSV enthält Kopfzeilen . Wählen Sie den Trennzeichentyp Komma aus und geben Sie Daten in das CSV-Feld ein.

   ![Datenstrukturen Bild 4](../12-exercises/assets/data-structures-walkthrough-4.png)

1. Klicken Sie auf Einmal ausführen , um die Ausgabe anzuzeigen.
1. Öffnen Sie den Ausführungsinspektor, um die Eingaben und Ausgaben des Parse CSV-Moduls anzuzeigen. Es gibt ein Bundle (eine CSV-Datei) als Eingabe und mehrere Bundles als Ausgabe (ein Bundle für jede Zeile in der CSV-Datei). Sie sollte ungefähr so aussehen:

   ![Datenstrukturen Bild 5](../12-exercises/assets/data-structures-walkthrough-5.png)

   **Wandeln Sie anschließend die Daten in das gewünschte Ausgabeformular um, wobei die aggregierten Zeitsummen in Stunden anstelle von Minuten ausgedrückt werden.**

1. Fügen Sie ein Tool-Modul &quot;Numerischer Aggregator&quot;hinzu.
1. Wählen Sie das Quellmodul aus, das das CSV-Modul &quot;Parse&quot;ist.
1. Wählen Sie SUM für die Aggregatfunktion aus.
1. Das Feld Wert ist die Spalte 7 aus der CSV-Datei. Dies sind die Minuten, die von jedem Benutzer protokolliert werden.
1. Um die Felder nach Gruppe zu summieren, klicken Sie auf Erweiterte Einstellungen und legen Sie Gruppe nach E-Mail fest (Spalte 4), Datum (Spalte 5).

   + Diese Summe wird für jede Kombination aus E-Mail und Datum berechnet. Stellen Sie sicher, dass Sie ein Komma zwischen Spalte 4 und Spalte 5 einfügen. Dies wird später als Trennzeichen verwendet.

   **Ihr Zuordnungsbereich sollte wie folgt aussehen:**

   ![Datenstrukturen Bild 6](../12-exercises/assets/data-structures-walkthrough-6.png)

1. Klicken Sie auf Einmal ausführen , um die Aggregationsausgabe zu überprüfen.

   **Die Ausgabebundles sollten wie folgt aussehen:**

   ![Datenstrukturen Bild 7](../12-exercises/assets/data-structures-walkthrough-7.png)

   **Konvertieren Sie nun die aggregierten Minuten in Stunden.**

1. Fügen Sie ein weiteres Tool-Modul hinzu, indem Sie Variable festlegen auswählen.
1. Nennen Sie die Variable &quot;Hours&quot;.
1. Setzen Sie den Variablenwert auf formatNumber(result/60;2;.;

   **Ihr Zuordnungsbereich sollte wie folgt aussehen:**

   ![Datenstrukturen Bild 8](../12-exercises/assets/data-structures-walkthrough-8.png)

   **Rufen Sie als Nächstes die Werte für die Ausgabedatei auf. Sie möchten die userID und den Datumswert für die Gruppierungen verwenden. Sie möchten auch die Stunden, die berechnet wurden.**

1. Fügen Sie mithilfe des Aggregators CSV erstellen (erweitert) ein weiteres Modul-CSV-Modul hinzu.
1. Das Quellmodul ist der Tools - Numerische Aggregator.
1. Klicken Sie im Feld Datenstruktur auf Hinzufügen und nennen Sie unsere Datenstruktur &quot;Zeit protokolliert Tägliche Summe&quot;.
1. Klicken Sie auf Element hinzufügen , um das erste Element zu erstellen.
1. Nennen Sie das Element &quot;UserID&quot;und legen Sie den Typ auf Text fest. Klicken Sie auf Hinzufügen.
1. Klicken Sie erneut auf Element hinzufügen , um das zweite Element zu erstellen.
1. Nennen Sie das Element &quot;Datum&quot;, legen Sie den Typ auf &quot;Datum&quot;fest und klicken Sie auf &quot;Hinzufügen&quot;.
1. Klicken Sie erneut auf Element hinzufügen .
1. Nennen Sie das Element &quot;Stunden&quot;, legen Sie den Typ auf &quot;Zahl&quot;fest und klicken Sie auf &quot;Hinzufügen&quot;.

   **Ihre Datenstruktur sollte wie folgt aussehen:**

   ![Datenstrukturen Bild 9](../12-exercises/assets/data-structures-walkthrough-9.png)

1. Klicken Sie auf Speichern , um die Datenstruktur der Zeit protokolliert Tägliche Summe abzuschließen.

   **Geben Sie nun die Werte für die drei soeben erstellten Felder an. Diese drei Felder sollten im Bedienfeld CSV-Zuordnung angezeigt werden.**

1. Klicken Sie in das Feld UserID und wählen Sie im Tab Allgemeine Funktionen die Option GET aus. Fügen Sie im ersten Parameter SPLIT aus der Registerkarte &quot;Text- und Binärfunktionen&quot;ein. Der erste Parameter für die SPLIT-Funktion ist das Schlüsselfeld. Fügen Sie ein Komma als Trennzeichen und 1 als Index hinzu. Dies zeigt an, dass das GET das erste Feld im Schlüssel-Array abrufen soll.
1. Kopieren Sie diesen Ausdruck in das Feld Datum . Ändern Sie den Index von 1 zu 2 in den zweiten Wert im Array.
1. Fügen Sie für das Feld Stunden das Feld Stunden aus dem Tool Variable festlegen hinzu.

   **Ihr Bedienfeld für die CSV-Zuordnung sollte wie folgt aussehen:**

   ![Datenstrukturen Bild 10](../12-exercises/assets/data-structures-walkthrough-10.png)

   **Wenn Sie das Szenario jetzt ausführen, sollte diese Ausgabe angezeigt werden:**

   ![Datenstrukturen Bild 11](../12-exercises/assets/data-structures-walkthrough-11.png)

   **Fügen Sie nun ein Modul hinzu, um diese Ausgabe zu erstellen und als Dokument in ein vorhandenes Projekt in Workfront hochzuladen.**

1. Öffnen Sie das Projekt in Workfront und kopieren Sie die Projekt-ID aus der URL.
1. Gehen Sie zurück zum Szenario in Fusion und fügen Sie ein weiteres Modul hinzu: das Modul &quot;Dokument hochladen&quot;aus der Workfront-App.
1. Fügen Sie die Projekt-ID in das Feld Zugehörige Datensatz-ID ein.
1. Wählen Sie Projekt für den Typ Zugehörige Datensätze .
1. Wählen Sie die Option Zuordnung für die Quelldatei aus.
1. Verwenden Sie für den Dokumentnamen den Dateinamen, den Sie heruntergeladen haben, und fügen Sie &quot;Aktualisiert &quot;davor ein.
1. Verwenden Sie für den Dateiinhalt die Textausgabe aus dem Modul CSV erstellen .

   **Ihr Zuordnungsbereich sollte wie folgt aussehen:**

   ![Datenstrukturen Bild 12](../12-exercises/assets/data-structures-walkthrough-12.png)

1. Klicken Sie auf OK und speichern Sie das Szenario.
1. Klicken Sie auf Einmal ausführen , um das Szenario auszuführen.

   **Überprüfen Sie den Ausführungsinspektor im Modul Dokument hochladen , um zu bestätigen, dass das Dokument hochgeladen wurde.**

   ![Datenstrukturen Bild 13](../12-exercises/assets/data-structures-walkthrough-13.png)

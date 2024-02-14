---
title: Einführung in die universelle Connector-Übung
description: Erfahren Sie mehr über die Arbeit mit universellen REST-Connectoren und mit den zurückgegebenen Daten.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
recommendations: noDisplay,noCatalog
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 98%

---

# Einführung in die universelle Connector-Übung

Erfahren Sie mehr über die Arbeit mit universellen REST-Connectoren und mit den zurückgegebenen Daten.

## Übungsübersicht

Rufen Sie mithilfe eines Pokemon-Charakters in einer Tabelle die Poke-API über einen HTTP-Connector auf, um weitere Informationen über diesen Charakter zu sammeln und zu veröffentlichen.

![Einführung in universelle Connectoren Bild 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Zu befolgende Schritte

**Laden Sie die CSV-Datei aus Workfront herunter.**

1. Wählen Sie im Workfront-Ordner „Fusion-Übungsdateien“ die Datei „_Fusion2020_Shipping Manifest.csv“ aus und klicken Sie auf „Dokumentdetails“.
1. Kopieren Sie die erste ID-Nummer aus der URL-Adresse.
1. Erstellen Sie ein neues Szenario in Workfront Fusion. Nennen Sie es „Universelle Connectoren verwenden“.
1. Beginnen Sie mit dem Modul „Dokument herunterladen“ in der Workfront-App.
1. Richten Sie Ihre Workfront-Verbindung ein und fügen Sie die Dokument-ID ein, die Sie aus der Workfront-URL kopiert haben.
1. Benennen Sie dieses Modul in „Versandmanifest herunterladen“ um.

   ![Einführung in universelle Connectoren Bild 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analysieren Sie die Versandmanifestdaten.**

1. Fügen Sie ein weiteres Modul hinzu und wählen Sie „CSV-Analyse“.
1. Richten Sie die CSV-Analyse für 11 Spalten ein. Markieren Sie das Kontrollkästchen „CSV enthält Kopfzeilen“. Wählen Sie als Trennzeichen „Komma“ aus und fügen Sie Daten aus dem Modul „Dokument herunterladen“ in das CSV-Feld ein.

   ![Einführung in universelle Connectoren Bild 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Benennen Sie dieses Modul in „Versandmanifest analysieren“ um.
1. Speichern Sie das Szenario und klicken Sie auf „Einmal ausführen“, damit Sie in den nächsten Schritten Daten aus der CSV-Datei sehen können.

   **Rufen Sie die Pokemon-Daten über den universellen Connector ab.**

1. Fügen Sie ein HTTP-Anfragemodul hinzu.
1. Verwenden Sie im URL-Feld `https://pokeapi.co/api/v2/pokemon/[Character]`, wobei [Zeichen] der Spalte 3 des Moduls „CSV-Analyse“ zugewiesen ist.
1. Aktivieren Sie das Kontrollkästchen „Antwort analysieren“.
1. Wählen Sie „Erweiterte Einstellungen anzeigen“ und aktivieren Sie dann das Kontrollkästchen neben „Alle Status als Fehler auswerten“.
1. Klicken Sie auf „OK“ und benennen Sie das Modul in „Pokemon-Informationen abrufen“ um.

   **Ihr Zuordnungsfenster sollte wie folgt aussehen:**

   ![Einführung in universelle Connectoren Bild 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **In diesem Teil der Übung werden Sie nur mit Zeile 1 in der CSV-Datei arbeiten.**

1. Fügen Sie vor Ihrem Pokemon-Infomodul einen Filter ein. Nennen Sie ihn „Nur Zeile 1“.
1. Legen Sie die Bedingung so fest, dass nur ID-Nummer 1 zugelassen wird. ID-Nummer 1 befindet sich in Zeile 1 und das ID-Feld in Spalte 1 der CSV-Datei.

   ![Einführung in universelle Connectoren Bild 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Speichern Sie das Szenario.
1. Klicken Sie auf „Einmal ausführen“ und beobachten Sie die Fehlermeldung, die Sie im HTTP-Anfragemodul erhalten.

   >[!IMPORTANT]
   >
   >Beachten Sie, dass im URL-Feld für die Eingabedaten der Zeichenname großgeschrieben wird. Dies funktioniert nicht für diesen API-Aufruf, da Zeichennamen in Kleinbuchstaben geschrieben werden müssen.

   ![Einführung in universelle Connectoren Bild 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Verwenden Sie das Zuordnungsfenster des HTTP-Felds „URL anfordern“, um für das Feld [Zeichen] mithilfe der Funktion **Kleinschreibung** nur Kleinbuchstaben zuzulassen.

   ![Einführung in universelle Connectoren Bild 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Geben Sie Informationszuordnungen mithilfe des Moduls „Mehrere Variablen festlegen“ von der API zurück.**

1. Fügen Sie das Modul „Mehrere Variablen festlegen“ hinter „Pokemon-Info abrufen“ hinzu. Ordnen Sie Name, Größe, Gewicht und Fähigkeiten zu.
1. Da das Feld „Fähigkeiten“ ein Array ist, sollten Sie die Funktion „zuordnen“ verwenden, um auf den Namen jeder Fähigkeit im Array zuzugreifen.

   ![Einführung in universelle Connectoren Bild 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Führen Sie das Szenario ohne Filter aus, um einen weiteren Fehler zu erkennen.**

1. Um alle Zeilen in der CSV-Datei zu verarbeiten, löschen Sie den Filter mit der Bezeichnung „Nur Zeile 1“:

   + Klicken Sie auf das Filtersymbol, um den Filter zu bearbeiten.
   + Löschen Sie die Filterbeschriftung.
   + Löschen Sie die Bedingung.
   + Klicken Sie auf „OK“.

1. Speichern Sie das Szenario und klicken Sie auf „Einmal ausführen“.
1. Im Modul „Pokemon-Informationen abrufen“ tritt ein Fehler auf. Sie sehen, dass ein Superhelden-Charakter an die Pokemon-API übergeben wurde.

   >[!NOTE]
   >
   >In der Anleitung zu Routern erfahren Sie, wie Sie diesen Fehler beheben können, indem Sie einen separaten Pfad zum Verarbeiten von Superhelden erstellen.

   ![Einführung in universelle Connectoren Bild 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)

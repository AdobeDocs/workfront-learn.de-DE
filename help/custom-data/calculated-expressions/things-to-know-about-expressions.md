---
title: Informationen zu berechneten Feldausdrücken
description: Hier erhalten Sie einen Einblick in eine Liste von Konzepten, die Sie beim Arbeiten mit benutzerdefinierten berechneten Feldern in [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Informationen zu berechneten Feldausdrücken

Im Folgenden finden Sie eine Liste von Konzepten, die beim Arbeiten mit benutzerdefinierten berechneten Feldern in [!DNL Workfront].

## Das Casing spielt in Ausdrucksnamen keine Rolle

Bei den Ausdrucksnamen spielt Groß-/Kleinschreibung keine Rolle. Sie können Groß- und Kleinschreibung oder eine Mischung aus beidem verwenden. Mit dem Ausdruck ISBLANK(Description) kann das &quot;ISBLANK&quot;wie folgt geschrieben werden:

* ISBLANK
* isBlblank
* IsBlank
* isBLANK

Sie werden alle funktionieren.

## Stunden werden in Minuten gespeichert

Stunden in [!DNL Workfront’s] -Datenbank in Minuten gespeichert. Wenn Sie auf Felder wie &quot;Geplante Stunden&quot;oder &quot;Tatsächliche Stunden&quot;verweisen, teilen Sie sie durch 60, um die Zeit in Stunden und nicht in Minuten anzuzeigen.

## Leerzeichen wirken sich nicht auf Ausdrücke aus

Die empfohlene Methode zum Schreiben von Ausdrücken besteht darin, zwischen den einzelnen Ausdrücken nur wenig bis gar keinen Abstand zu haben.

* IF(ISBLANK(Description),&quot;No Description&quot;,&quot;Has Description&quot;)

Wenn der Abstand Ihnen jedoch zeigt, was vor sich geht, können die Ausdrücke um einige Abstände erweitert werden. Die zusätzlichen Leerzeichen sollten nicht verhindern, dass der Ausdruck einen Wert in [!DNL Workfront].

* IF (ISBLANK (Description),&quot;No Description&quot;,&quot;Has Description&quot;)

## Anführungszeichen müssen gerade sein

Achten Sie bei Verwendung von Anführungszeichen in einem Ausdruck darauf, dass die Anführungszeichen gerade (&quot;) sind. Wenn die Anführungszeichen gekrümmt sind (&quot;), wird die [!DNL Workfront] -System zeigt weiterhin die Meldung &quot;Benutzerdefinierter Ausdruck ungültig&quot;an.

## Berechnungen werden beim Speichern und Bearbeiten von Formularen aktualisiert

Dies ist ein wichtiger Aspekt der berechneten Felder.

In einem berechneten Feld angezeigte Informationen bleiben unverändert, es sei denn, das benutzerdefinierte Formular wurde neu berechnet. Ausdrücke können aktualisiert werden, indem Sie die Option Ausdrücke neu berechnen im Menü Mehr für ein Objekt verwenden.

Sie möchten sehen, wie viele Tage ein Problem geöffnet war. Erstellen Sie ein berechnetes Feld namens &quot;Days Open&quot;mit dem Ausdruck DATEDIFF.

* Feldname = Öffnungen
* Ausdruck = DATEDIFF(Entry Date,$$TODAY)

Nach dem Speichern die Anzahl der Tage zwischen der ersten Erstellung des Problems oder der Eingabe in [!DNL Workfront]und das heutige Datum kann auf der Detailseite eines Objekts oder in einer Berichtsansicht angezeigt werden.

Wenn Sie am folgenden Tag dieselbe Detailseite oder Berichtsansicht anzeigen, wird diese Zahl voraussichtlich um 1 inkrementiert. Wenn die Zahl heute 5 ist, sollte sie morgen 6 sein. Der nächste Tag sollte 7, dann 8 usw. sein.

Das Feld zeigt jedoch weiterhin täglich 5 an. Das Feld muss erneut ausgeführt oder neu berechnet werden, um die Informationen zu aktualisieren.

So aktualisieren Sie ein Feld mit der Option Ausdrücke neu berechnen :

* Klicken Sie auf den Namen des Objekts, um es zu öffnen.
* Klicken Sie auf das Menü Mehr .
* Wählen Sie in der Liste die Option Ausdrücke neu berechnen aus.

Sie können mehrere Ausdrücke gleichzeitig neu berechnen, indem Sie die Funktion &quot;Massenbearbeitung&quot;in einer Liste oder einem Bericht verwenden. Angenommen, Sie haben einen Bericht erstellt, der eine Liste von Problemen mit der Berechnung der Öffnungen in einer Spalte anzeigt. Wenn Sie alle Probleme gleichzeitig neu berechnen möchten:

* Wählen Sie alle Probleme im Bericht aus.
* Wählen Sie die Bearbeitungsoption aus, um alle ausgewählten Probleme stapelweise zu bearbeiten.
* Klicken Sie links auf die Beschriftung Benutzerdefinierte Forms , um zum Abschnitt für benutzerdefinierte Formulare zu blättern.
* Aktivieren Sie unten im Abschnitt Benutzerdefinierte Forms die Option Benutzerdefinierte Ausdrücke neu berechnen .
* Klicken Sie auf Änderungen speichern.

Der Bildschirm wird aktualisiert und zeigt aktualisierte Informationen im berechneten Feld an.

**Hinweis**: Es gibt zwar andere Möglichkeiten, Ausdrücke in einem berechneten Feld zu aktualisieren oder neu zu berechnen, aber dies ist die schnellste und einfachste Methode.

## Berechnungen können von Formular zu Formular innerhalb desselben Felds variieren

Sobald ein berechnetes Feld in einem benutzerdefinierten Formular gespeichert und das benutzerdefinierte Formular gespeichert wird, wird das berechnete Feld der Feldbibliothek hinzugefügt, damit es in anderen benutzerdefinierten Formularen verwendet werden kann.

Wenn Sie jedoch ein berechnetes Feld in Formular A und dasselbe berechnete Feld in Formular B haben, besteht der ursprüngliche Gedanke darin, dass die Berechnungen genau gleich sind. Das ist nicht immer der Fall. Das berechnete Feld in Formular A kann in Formular B völlig anders berechnet werden.

Wenn ein berechnetes benutzerdefiniertes Feld aus der Feldbibliothek ausgewählt und einem benutzerdefinierten Formular hinzugefügt wird, wird das Feld hinzugefügt, die Berechnung ist jedoch leer. Ein Grund dafür ist, dass sich die Berechnung möglicherweise auf Felder bezieht, die für einen anderen Objekttyp nicht vorhanden sind.

Sie haben beispielsweise das berechnete Feld &quot;Tage bis zum Abschluss&quot;erstellt, um zu bestimmen, wie lange es dauerte, bis eine Aufgabe in einem Projekt abgeschlossen war.

* WEEKDAYDIFF(Tatsächliches Startdatum, tatsächliches Abschlussdatum)

Du willst dasselbe für eine Iteration tun. Sie können denselben Ausdruck verwenden. Die für ein Aufgabenobjekt verfügbaren Felder sind jedoch nicht immer für ein Iterationsobjekt verfügbar. Also [!DNL Workfront] gibt Ihnen die Möglichkeit, die Berechnung mit den richtigen Objektfeldern zu erstellen.

**Pro-Tipp**: Kopieren Sie den berechneten Ausdruck aus dem Feld Berechnung in das Feld Anweisungen , wenn Sie benutzerdefinierte Felder erstellen. Dieses Feld wird nicht gelöscht, wenn dem benutzerdefinierten Formular aus der Feldbibliothek ein berechnetes benutzerdefiniertes Feld hinzugefügt wird.

Je nach Bedarf können berechnete Felder in benutzerdefinierten Formularen ganz einfach oder sehr komplex sein. Ausdrücke können andere Ausdrücke und Werte einbetten oder verschachteln, um die Detailgenauigkeit zu gewährleisten, die für ein besseres Bild der Arbeit in Ihrer Organisation erforderlich ist.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->

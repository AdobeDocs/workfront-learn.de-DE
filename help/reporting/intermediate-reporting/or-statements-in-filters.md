---
title: Erstellen von OR-Anweisungen in Filtern
description: Erfahren Sie, wie Sie mit einer OR-Anweisung Workfront mitteilen, dass Sie dieses ODER in Ihrem Bericht sehen möchten.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
kt: 9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Erstellen von OR-Anweisungen in Filtern

Wenn Sie einen Filter mit mehreren Kriterienzeilen erstellen, setzt standardmäßig ein UND zwischen jeder Zeile. Dies bedeutet, dass jedes Ergebnis in der Liste, wenn Sie diesen Filter verwenden, alle Filterregeln erfüllt.

In diesem Beispiel haben wir drei Kriterien bzw. Regeln für einen Projektfilter:

1. Das Projekt muss einen geplanten Abschlussdatum haben, der in den aktuellen Monat fällt.
1. Das Projekt muss sich im Ereignismarketing-Portfolio befinden.
1. Das Projekt muss ein aktives Projekt sein, d. h., es muss den Status &quot;Aktuell&quot;haben.

![Ein Bild zum Erstellen eines Filters mit UND-Anweisungen in [!DNL Workfront]](assets/or-statement-1.png)

Die Projekte in der Ergebnisliste erfüllen alle drei Kriterien und helfen Ihnen dabei, die Suchergebnisse einzugrenzen, sodass Sie genau die benötigten Informationen sehen können.

![Ein Bild einer gefilterten Liste in [!DNL Workfront]](assets/or-statement-2.png)

Es kann jedoch vorkommen, dass die Filterergebnisse verschiedene Kriterien erfüllen sollen, und in diesem Fall können OR-Anweisungen hilfreich sein. Mit einer OR-Anweisung teilen Sie dem Filter mit, dass Sie dieses ODER sehen möchten.

## Verwenden von OR-Anweisungen

ODER-Anweisungen erweitern oder erhöhen die Menge der Informationen, die der Filter findet, da ein Element, um in der Ergebnisliste angezeigt zu werden, nur eine der Filterregeln erfüllen muss, nicht alle.

Sehen wir uns eine einfache ODER-Anweisung an - Projekte, die Sie als Projektleiter (Eigentümer) für von Ihnen erstellte ODER-Projekte sind.

![Ein Bild zum Erstellen eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-3.png)

Nachdem Sie beide Filterregeln eingerichtet haben, klicken Sie auf das UND zwischen ihnen und wechseln Sie zu OR.

![Ein Bild zum Erstellen eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-4.png)

Der ODER zwischen den beiden Filterregeln erweitert Ihre Suchkriterien und teilt Workfront mit, dass Projekte gefunden werden, die die eine oder andere dieser Optionen erfüllen. Ihr Name befindet sich im Feld Projektinhaber oder Sie sind der Ersteller des Projekts.

## Mehrere Filterregeln mit ODER-Anweisungen

Sehen wir uns nun eine OR-Anweisung an, die mehrere Filterregeln auf jeder Seite des ODER enthält. Hierbei werden dieselben beiden Regeln wie zuvor verwendet, es wird jedoch eine Regel hinzugefügt - Projekte müssen auch den Status &quot;Aktuell&quot;haben.

![Ein Bild zum Erstellen eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-5.png)

Beachten Sie, dass Workfront die Filterregeln auf jeder Seite des ODER &quot;gruppiert&quot;hat (um sie herum gibt es einen grauen Rahmen). Dadurch wird Workfront angewiesen, die Regeln auf jeder Seite des ODER gemeinsam auszuführen und Projekte zu finden, die beide Kriterien erfüllen, da sie mit UND verbunden sind.

In diesem Beispiel sucht Workfront nach:

* Projekte mit Ihrem Namen im Feld &quot;Projekteigentümer&quot;, die ebenfalls den Status &quot;Aktuell&quot;haben.
* **PLUS (OR)**
* Von Ihnen erstellte Projekte, die ebenfalls den Status &quot;Aktuell&quot;haben.

Wenn Sie die Regel &quot;Projektstatus gleich Aktuell&quot;auf jeder Seite des ODER platzieren, wird sichergestellt, dass die Regel in Verbindung mit den anderen Regeln funktioniert. Diese gängige Regel wird manchmal als &quot;Konstante&quot;bezeichnet.

>[!NOTE]
>
>Sie sind nicht auf eine wiederholte Filterregel auf jeder Seite des ODER beschränkt. Je nach Ihren Anforderungen können mehrere Workfront empfiehlt, diese wiederholten Regeln auf ein Minimum zu beschränken, um sicherzustellen, dass der Filter die gewünschten Ergebnisse liefert.

## Was passiert ohne die allgemeine Filterregel?

Ohne die gängigen Filterregeln erhalten Sie möglicherweise nicht die erwarteten Suchergebnisse.

Wenn Sie beispielsweise die Regel &quot;Projektstatus gleich Aktuell&quot;nur auf einer Seite des ODER platzieren, funktioniert sie nur mit den anderen Filterregeln in diesem Abschnitt. In der Abbildung unten sehen Sie, dass die Regel &quot;Projektstatus gleich Aktuell&quot;nur im oberen Abschnitt angezeigt wird.

![Ein Bild zum Erstellen eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-6.png)

Dies bedeutet, dass Workfront nach folgenden Kriterien sucht:

* Projekte mit Ihrem Namen im Feld &quot;Projektinhaber&quot;und dem Status &quot;Aktuell&quot;.
* **PLUS (OR)**
* Alle von Ihnen erstellten Projekte.

Wie Sie sehen, liefert Ihnen diese Filtereinrichtung etwas andere Ergebnisse als der Filter mit der wiederholten Filterregel. Deshalb ist es wichtig sicherzustellen, dass der Filter ordnungsgemäß eingerichtet ist, um sicherzustellen, dass Sie die gewünschten und benötigten Ergebnisse erhalten.

Beim Erstellen von Filtern dürfen OR-Anweisungen nicht häufig verwendet werden. Dies kann jedoch dazu beitragen, die Anzahl der Filter zu reduzieren, die Sie erstellen müssen. Stellen Sie sicher, dass Ihre Filter nicht zu viele Ergebnisse zurückgeben. Eine lange Liste kann es für Benutzer erschweren, die benötigten Informationen zu finden.

## ODER-Filteraktivität

Sie möchten unvollständige Aufgaben finden, die Ihnen zugewiesen sind oder die niemandem zugewiesen sind. Sie richten einen Filter ein, der wie der unten stehende aussieht. Wird dieser Filter Ihnen die gewünschten Ergebnisse liefern? Warum oder warum nicht?

![Ein Bild einer falsch erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antworten

Nein, dieser Filter liefert nicht die gewünschten Ergebnisse - Aufgaben, die noch nicht abgeschlossen sind und Ihnen entweder zugewiesen oder keiner zugewiesen sind - da sich die Filterregel für den Aufgabenstatus nur auf einer Seite des ODER befindet.

Stattdessen generiert dieser Filter eine Liste, die Folgendes anzeigt:

* Aufgaben, die Ihnen mit dem Status &quot;Wird ausgeführt&quot;oder &quot;Neu&quot;zugewiesen wurden.
* **PLUS (OR)**
* Alle nicht zugewiesenen Aufgaben, unabhängig vom Status.

Der Filter sollte wie der unten stehende aussehen. Beachten Sie, dass dieser Filter die Filterregel für den Aufgabenstatus auf beiden Seiten des ODER enthält.

![Ein Bild einer ordnungsgemäß erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-2.png)

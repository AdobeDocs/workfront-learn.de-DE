---
title: Erstellen von OR-Anweisungen in Filtern
description: Lernen Sie, wie Sie eine ODER-Anweisung verwenden, um Workfront mitzuteilen, dass Sie entweder dies ODER das in Ihrem Bericht sehen möchten.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 100%

---

# Erstellen von OR-Anweisungen in Filtern

Wenn Sie einen Filter mit mehreren Zeilen von Kriterien erstellen, setzt Workfront standardmäßig ein UND zwischen jede Zeile. Das bedeutet, dass jedes Ergebnis in der Liste, wenn Sie diesen Filter verwenden, alle Filterregeln erfüllt.

In diesem Beispiel haben wir drei Kriterien bzw. Regeln für einen Projektfilter:

1. Das Projekt muss ein geplantes Abschlussdatum haben, das in den laufenden Monat fällt.
1. Das Projekt muss zum Portfolio des Veranstaltungs-Marketings gehören.
1. Das Projekt muss ein aktives Projekt sein, d. h., es muss den Status „Aktuell“ haben.

![Ein Bild der Erstellung eines Filters mit AND-Anweisungen in [!DNL Workfront]](assets/or-statement-1.png)

Die Projekte in der Ergebnisliste erfüllen alle drei Kriterien, was Ihnen dabei hilft, die Suchergebnisse einzugrenzen, sodass Sie genau die benötigten Informationen sehen können.

![Ein Bild einer gefilterten Liste in [!DNL Workfront]](assets/or-statement-2.png)

Es kann jedoch vorkommen, dass Sie möchten, dass die Filterergebnisse verschiedene Kriterien erfüllen. In diesem Fall können ODER-Anweisungen helfen. Mit einer ODER-Anweisung teilen Sie dem Filter mit, dass Sie Dinge sehen wollen, die mit (mindestens) EINER der ODER-Anweisungen übereinstimmen, aber nicht unbedingt mit ALLEN wie für UND-Anweisungen.

## Verwenden von ODER-Anweisungen

ODER-Anweisungen erweitern oder erhöhen die Menge der Informationen, die der Filter findet, denn um in der Ergebnisliste zu erscheinen, muss ein Element nur eine der Filterregeln erfüllen, nicht alle.

Betrachten wir eine einfache ODER-Verknüpfung: Projekte, für die Sie die Projektleitung (Eigentümerin oder Eigentümer) sind, ODER Projekte, die von Ihnen erstellt wurden.

![Ein Bild der Erstellung eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-3.png)

Nachdem Sie beide Filterregeln eingerichtet haben, klicken Sie auf das dazwischen liegende UND und schalten es auf ODER um.

![Ein Bild der Erstellung eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-4.png)

Das ODER zwischen den beiden Filterregeln erweitert Ihre Suchkriterien und weist Workfront an, Projekte zu finden, die eine der beiden Optionen erfüllen – Ihr Name steht im Projektbesitzer-Feld oder Sie sind die Person, die das Projekt erstellt hat.

## Mehrere Filterregeln mit ODER-Anweisungen

Betrachten wir nun eine ODER-Anweisung, die mehrere Filterregeln auf jeder Seite des ODER enthält. Hier werden dieselben zwei Regeln wie zuvor verwendet, aber es wird eine weitere Regel hinzugefügt: Projekte müssen auch den Status „aktuell“ haben.

![Ein Bild der Erstellung eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-5.png)

Beachten Sie, dass Workfront die Filterregeln auf jeder Seite des ODER „gruppiert“ (sie sind von einem grauen Rahmen umgeben). Dadurch wird Workfront angewiesen, die Regeln auf beiden Seiten des ODER zusammen auszuführen, um Projekte zu finden, die beide Kriterien erfüllen, weil sie mit UND verknüpft sind.

In diesem Beispiel sucht Workfront:

* Projekte, bei denen Ihr Name im Feld „Projektbesitzer“ steht und die außerdem den Status „Aktuell“ haben.
* **PLUS (ODER)**
* Projekte, die Sie erstellt haben und die ebenfalls den Status „Aktuell“ haben.

Wenn Sie die Regel „Projektstatus ist gleich aktuell“ auf jeder Seite des ODER platzieren, wird sichergestellt, dass diese Regel in Verbindung mit jeder der anderen Regeln funktioniert. Diese allgemeine Regel wird manchmal auch als „Konstante“ bezeichnet.

>[!NOTE]
>
>Sie sind nicht auf nur eine wiederholte Filterregel auf jeder Seite des ODER beschränkt. Je nach Ihren Bedürfnissen können Sie mehrere haben. Workfront empfiehlt jedoch, diese wiederholten Regeln auf ein Minimum zu beschränken, um sicherzustellen, dass der Filter die gewünschten Ergebnisse liefert.

## Was passiert ohne die gemeinsame Filterregel?

Ohne die gemeinsame(n) Filterregel(n) erhalten Sie möglicherweise nicht die erwarteten Suchergebnisse.

Wenn Sie zum Beispiel die Regel „Projektstatus gleich aktuell“ nur auf einer Seite des ODER platzieren, funktioniert sie nur zusammen mit den anderen Filterregeln in diesem Abschnitt. In der Abbildung unten sehen Sie, dass die Regel „Projektstatus ist gleich aktuell“ nur für den oberen Bereich gilt.

![Ein Bild der Erstellung eines Filters mit ODER-Anweisungen in [!DNL Workfront]](assets/or-statement-6.png)

Das bedeutet, dass Workfront Folgendes suchen wird:

* Projekte, bei denen Ihr Name im Feld „Projektegentümerin oder Projekteigentümer“ steht und die den Status „Aktuell“ haben.
* **PLUS (ODER)**
* Alle von Ihnen erstellten Projekte.

Wie Sie sehen können, führt diese Filtereinstellung zu etwas anderen Ergebnissen als der Filter mit der wiederholten Filterregel. Deshalb ist es wichtig, dass der Filter korrekt eingerichtet ist, damit Sie die gewünschten und erforderlichen Ergebnisse erzielen.

Sie sollten ODER-Anweisungen bei der Erstellung von Filtern nicht häufig verwenden. Allerdings können Sie auf diese Weise die Anzahl der zu erstellenden Filter verringern. Achten Sie nur darauf, dass Ihre Filter nicht zu viele Ergebnisse liefern – eine lange Liste kann es den Benutzenden erschweren, genau die gewünschten Informationen zu finden.

## ODER-Filteraktivität

Sie möchten unvollständige Aufgaben finden, die Ihnen oder niemandem zugewiesen sind. Dazu richten Sie den untenstehenden Filter ein. Wird dieser Filter die gewünschten Ergebnisse liefern? Warum oder warum nicht?

![Bild einer falsch erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antworten

Nein, dieser Filter wird nicht die Ergebnisse liefern, die Sie sich erhoffen (unerledigte Aufgaben, die entweder Ihnen oder niemandem zugewiesen sind), weil die Filterregel für den Aufgabenstatus nur auf einer Seite von ODER steht.

Stattdessen generiert dieser Filter eine Liste, die Folgendes anzeigt:

* Ihnen zugewiesene Aufgaben mit dem Status „In Bearbeitung“ oder „Neu“ haben.
* **PLUS (ODER)**
* Alle nicht zugewiesenen Aufgaben, unabhängig vom Status.

Der Filter sollte stattdessen wie folgt aussehen. Beachten Sie, dass bei diesem Filter die Filterregel für den Aufgabenstatus auf beiden Seiten des ODER steht.

![Bild einer ordnungsgemäß erstellten ODER-Anweisung in [!DNL Workfront]](assets/or-statement-your-turn-2.png)

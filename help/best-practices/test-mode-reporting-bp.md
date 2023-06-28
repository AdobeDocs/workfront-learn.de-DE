---
title: Best Practice - Textmodusberichte
description: Erfahren Sie mehr über Best Practices von Adobe Workfront-Experten zur Einrichtung, Verwaltung und Verwendung von Workfront-Textmodusberichten.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Best Practice - Textmodusberichte

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für die Textmodusberichterstellung

* Verwenden Sie nach Möglichkeit in Spalten des Listenberichts Werteausdrücke aus dem Textmodus anstelle von berechneten benutzerdefinierten Feldern.

* Fügen Sie die in einer Textmodusberechnung verwendeten Berechnungen in die Beschreibung des Berichts ein.

</br>
</br>

## Warum sind diese Best Practices?

**Best Practice**

Verwenden Sie nach Möglichkeit in Spalten des Listenberichts Werteausdrücke aus dem Textmodus anstelle von berechneten benutzerdefinierten Feldern.



**Deshalb**

Die Werte der Textmodi werden zum Zeitpunkt der Berichterstellung berechnet und bei jeder Aktualisierung des Berichts neu berechnet. Das bedeutet, dass Sie stets aktuelle Daten und genaue Berichte haben.



Berechnete benutzerdefinierte Felder (die in benutzerdefinierten Formularen verwendet werden) werden nicht automatisch aktualisiert, wenn Daten in Workfront angezeigt werden. Stattdessen werden die Ergebnisse der letzten in Workfront gespeicherten Berechnung angezeigt. Dies bedeutet, dass diese Werte zu einem bestimmten Zeitpunkt &quot;veraltet&quot;oder &quot;veraltet&quot;sein können. Berechnete benutzerdefinierte Felder müssen manuell aktualisiert werden, entweder durch Neuberechnung des Ausdrucks oder durch Bearbeiten und Speichern des Objekts, das das berechnete Feld enthält. Dies kann zeitaufwendig und leicht zu vergessen sein.


</br>
</br>

**Best Practice**

Fügen Sie die in einer Textmodusberechnung verwendeten Berechnungen in die Beschreibung des Berichts ein.



**Deshalb**

Wenn Sie Textmodusberechnungen in die Beschreibung des Berichts aufnehmen, können andere erkennen, wie die Berechnung erstellt wurde und welche Informationen angezeigt werden sollten. Außerdem werden Systemadministratoren daran erinnert, wie der Bericht erstellt wurde, falls in Zukunft Aktualisierungen erforderlich sind.

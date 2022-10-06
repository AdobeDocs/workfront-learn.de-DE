---
title: Best Practice - Anforderungswarteschlangen
description: Erfahren Sie mehr über Best Practices-Empfehlungen von Adobe Workfront-Experten zum Einrichten, Verwalten und Verwenden von Workfront-Anforderungswarteschlangen.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
kt: 10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Best Practice - Anforderungswarteschlangen

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für Anforderungswarteschlangen

* Fügen Sie eine Beschreibung für jedes Element einer Anforderungswarteschlange ein - das Anforderungswarteschlangenprojekt, Themengruppen, Warteschlangenthemen und Routing-Regeln.

* Erstellen Sie einen Projektstatus mit dem Namen &quot;Anforderungswarteschlange&quot;oder &quot;Operativ&quot;, der mit &quot;Aktuell&quot;übereinstimmt, um Anforderungswarteschlangenprojekte von anderen Projekten zu unterscheiden.

* Wenn Sie beabsichtigen, Problemgenehmigungen für über eine Warteschlange gesendete Anforderungen zu verwenden, erstellen Sie einen Problemstatus namens Abgelehnt .

* Weisen Sie &quot;universelle&quot;benutzerdefinierte Formulare den Anfragewarteschlangen zu, um so viele unternehmensweite konsistente Daten wie möglich zu erfassen.

* Vermeiden Sie die Freigabe von Anforderungswarteschlangen für &quot;alle&quot;. Richten Sie die Einstellungen für die Warteschlangendetails ein, damit Benutzer nur die Warteschlangen sehen, die für ihre Anforderungen relevant sind.

* Erstellen Sie ein Dashboard mit Anforderungswarteschlangenberichten, damit Traffic-Manager, Systemadministratoren oder zugewiesene Benutzer Probleme direkt bearbeiten können.

* Verwenden Sie Layoutvorlagen, um die Einrichtungsoptionen für Anforderungswarteschlangen aus dem Menü des linken Bedienfelds von Projekten für Benutzer zu entfernen, die keine Warteschlangen erstellen müssen.

* Erstellen Sie eine Anforderungswarteschlange für Systemadministratoren, in der Benutzer Workfront-bezogene Fragen stellen, Anforderungen bezüglich der Systemeinrichtung stellen, neue Benutzerschulungen planen usw.

* Prüfen Sie Anforderungswarteschlangen regelmäßig, um nicht verwendete Warteschlangen zu identifizieren und deren Freigabe aufzuheben.

* Verwenden Sie Themengruppen, um mehr als 10 Warteschlangenthemen in einer Anforderungswarteschlange zu organisieren, um kürzere, einfacher zu verwaltende Listen zu erstellen.

* Steuern Sie die Gesamtzahl der für Benutzer verfügbaren Anforderungswarteschlangen, indem Sie eine Anforderungswarteschlange anhand von Themengruppen und Warteschlangenthemen aufschlüsseln, anstatt mehrere Warteschlangen zu erstellen.

* Richten Sie Routing-Regeln für jedes Warteschlangenthema ein. Richten Sie mindestens eine Standard-Routing-Regel ein.

* Nutzen Sie Themengruppen und Warteschlangenthemen, wenn ein selektives Routing erforderlich ist.

* Senden Sie Anfragen an ein Team und nicht an eine Einzelperson.


</br>
</br>


## Warum sind diese Best Practices?


**Best Practice**

Fügen Sie eine Beschreibung für jedes Element einer Anforderungswarteschlange ein - das Anforderungswarteschlangenprojekt, Themengruppen, Warteschlangenthemen und Routing-Regeln.

**Deshalb**

Beschreibungen informieren Gruppenadministratoren, zukünftige Systemadministratoren oder andere, die Anforderungswarteschlangen verwalten, darüber, was genau jeder Teil der Anforderungswarteschlange tut.

Die Beschreibungsinformationen werden auch angezeigt, wenn Sie den Mauszeiger über das Informationssymbol im Feld in der neuen Anforderungsleiste bewegen.

Die Beschreibung muss nicht lang sein, nur ein kurzer Kommentar zum Zweck oder zur Verwendung des Elements.

</br>
</br>

**Best Practice**

Erstellen Sie einen Projektstatus mit dem Namen &quot;Anforderungswarteschlange&quot;oder &quot;Operativ&quot;, der mit &quot;Aktuell&quot;übereinstimmt, um Anforderungswarteschlangenprojekte von anderen Projekten zu unterscheiden.

**Deshalb**

Eine Anforderungswarteschlange &quot;lebt&quot;in einem Projekt und muss sich in einem Status befinden, der dem aktuellen Status entspricht, damit die Warteschlange aktiv ist.

Um eine Anforderung von den tatsächlichen Arbeitsprojekten mit dem Status &quot;Aktuell&quot;zu unterscheiden, erstellen Sie einen Status, der nur in Anforderungswarteschlangen mit dem Namen &quot;Anforderungswarteschlange&quot;oder &quot;Operativ&quot;verwendet werden soll. Anschließend können Sie diesen Status verwenden, um beim Schreiben von Berichten Anforderungswarteschlangenprojekte auszuschließen oder einzuschließen.

</br>
</br>

**Best Practice**

Erstellen Sie bei der Verwendung von Problemgenehmigungen den Fehlerstatus &quot;Abgelehnt&quot;und legen Sie für die Option Bei Abgelehnt den Status &quot;Abgelehnt&quot;fest.

**Deshalb**

Durch die Verwendung des Status &quot;Abgelehnt&quot;wird deutlich, dass der Antrag geprüft und abgelehnt wurde.

</br>
</br>

**Best Practice**

Weisen Sie &quot;universelle&quot;benutzerdefinierte Formulare den Anfragewarteschlangen zu, um so viele unternehmensweite konsistente Daten wie möglich zu erfassen.

**Deshalb**

Ein &quot;universelles&quot;benutzerdefiniertes Formular erfasst die für die Anfrage benötigten Standardinformationen, unabhängig vom Typ der gesendeten Anforderung.

Ein &quot;universelles&quot;benutzerdefiniertes Formular reduziert die Anzahl benutzerdefinierter Formulare, die Sie erstellen und verwalten müssen. Außerdem wird sichergestellt, dass alle Anforderungen dieselben Informationen auf die gleiche Weise erfassen, was zu einer konsistenten Berichterstattung und Datenanalyse führt.

</br>
</br>

**Best Practice**

Vermeiden Sie die Freigabe von Anforderungswarteschlangen für &quot;alle&quot;.  Richten Sie die Einstellungen für die Warteschlangendetails ein, damit Benutzer nur die Warteschlangen sehen, die für ihre Anforderungen relevant sind.

**Deshalb**

In den meisten Fällen muss eine Anforderungswarteschlange nur für bestimmte Personen wie ein Team, einen Anbieter, Kunden usw. freigegeben werden. Wenn Anfragende nur sehen, was sie in der Liste der Anforderungswarteschlangen benötigen, ist es einfach, Dinge zu finden und zu navigieren.

</br>
</br>


**Best Practice**

Erstellen Sie ein Dashboard mit Anforderungswarteschlangenberichten, damit Traffic-Manager, Systemadministratoren oder zugewiesene Benutzer Probleme direkt bearbeiten können.

**Deshalb**

Wenn Benutzer schnell und einfach auf eingehende Anfragen zugreifen können, geht die Arbeit nicht verloren.

</br>
</br>

**Best Practice**

Verwenden Sie Layoutvorlagen, um die Einrichtungsoptionen für Anforderungswarteschlangen aus dem Menü des linken Bedienfelds von Projekten für Benutzer zu entfernen, die keine Warteschlangen erstellen müssen.


**Deshalb**

Dadurch wird sichergestellt, dass alle Anforderungswarteschlangen den richtigen Prozess zur Erstellung durchlaufen (z. B. durch einen Governance-Ausschuss überprüft) und entweder von einem System- oder Gruppenadministrator korrekt eingerichtet werden.

Darüber hinaus hilft dies, die Warteschlangenliste organisiert zu halten und sich auf die Arten von Anforderungen zu konzentrieren, die Ihr Unternehmen benötigt.

</br>
</br>

**Best Practice**

Erstellen Sie eine Anforderungswarteschlange für Systemadministratoren, in der Benutzer Workfront-bezogene Fragen stellen, Anforderungen bezüglich der Systemeinrichtung stellen, neue Benutzerschulungen planen usw.

**Deshalb**

Dies bietet einen zentralen Ort, an dem Benutzer Fragen stellen können und Administratoren Fragen zu Workfront-bezogenen Problemen sammeln, überwachen und beantworten können.

Darüber hinaus können diese Informationen verwendet werden, um die Führungsrolle, den Arbeitsaufwand und den Wert der Systemadministratorrolle sowie einen zusätzlichen Systemadministrator zu rechtfertigen.

</br>
</br>


**Best Practice**

Prüfen Sie Anforderungswarteschlangen regelmäßig, um nicht verwendete Warteschlangen zu identifizieren und deren Freigabe aufzuheben.

**Deshalb**

Eine regelmäßige Prüfung der Setups und Elemente in Ihrem Adobe Workfront-System hilft, das System unübersichtlich und ohne unnötige Elemente zu halten. Wenn eine Warteschlange nicht mehr verwendet oder überwacht wird, stellen Sie sicher, dass Benutzer nicht mehr darauf zugreifen können, damit Arbeitsanforderungen nicht ungültig werden.

</br>
</br>


**Best Practice**

Verwenden Sie Themengruppen, um mehr als 10 Warteschlangenthemen in einer Anforderungswarteschlange zu organisieren, um kürzere, einfacher zu verwaltende Listen zu erstellen.

**Deshalb**

Themengruppen erhöhen die Benutzerakzeptanz und schaffen weniger Verwirrung, indem sie die anfängliche Liste der Optionen verringern, aus denen Sie auswählen können. Dadurch können Benutzer einfach finden, wonach sie suchen, ohne sie beim Senden einer Anfrage zu überfordern.

Darüber hinaus können Systemadministratoren und/oder Anforderungswarteschlangenmanager einen reibungslosen Navigationspfad für Benutzer erstellen und die Organisation und Berichterstellung für die Typen der gesendeten Anforderungen verbessern.

</br>
</br>

**Best Practice**

Steuern Sie die Gesamtzahl der für Benutzer verfügbaren Anforderungswarteschlangen, indem Sie eine Anforderungswarteschlange anhand von Themengruppen und Warteschlangenthemen aufschlüsseln, anstatt mehrere Warteschlangen zu erstellen.

**Deshalb**

Zu viele Anfragewarteschlangen machen es für Benutzer schwierig, das zu finden, was sie benötigen.

Weniger Warteschlangen helfen auch Traffic-Koordinatoren, Systemadministratoren oder anderen, die die Warteschlangen verwalten, damit sie die benötigten Informationen schneller finden können, ohne zu mehreren Projekten in der Anforderungswarteschlange navigieren zu müssen.

Erstellen Sie mehrere Anforderungswarteschlangen, wenn für verschiedene Anforderungswarteschlangen ein anderer Zugriff erforderlich ist oder wenn die Konsolidierung von Warteschlangen für die Benutzer verwirrend wäre.

</br>
</br>

**Best Practice**

Richten Sie Routing-Regeln für jedes Warteschlangenthema ein. Richten Sie mindestens eine Standard-Routing-Regel ein.

**Deshalb**

Routing-Regeln stellen sicher, dass jemandem immer die eingehende Anfrage zugewiesen wird, damit die Arbeit nicht durch die Risse fällt.

</br>
</br>

**Best Practice**

Nutzen Sie Themengruppen und Warteschlangenthemen, wenn ein selektives Routing erforderlich ist.

**Deshalb**

Routing-Regeln können nicht auf Felder eines benutzerdefinierten Formulars angewendet werden. Wenn also unterschiedliche Anforderungstypen an verschiedene Teams/Einzelpersonen weitergeleitet werden müssen, stellen Sie jedem Anfragetyp ein eigenes Themengruppen-/Warteschlangenthema zur Verfügung, damit die Arbeit ordnungsgemäß weitergeleitet werden kann.

</br>
</br>

**Best Practice**

Senden Sie Anfragen an ein Team und nicht an eine Einzelperson.

**Deshalb**

Wenn Anfragen an das Team gesendet werden, erhalten Sie vom gesamten Team einen Einblick in die ausgeführten Anforderungen und die damit verbundenen Aufgaben. Jeder kann sich die Team-Seite auf neue Elemente ansehen oder die neuen Funktionen mit einem Bericht in einem Dashboard verfolgen.

Außerdem wird sichergestellt, dass, wenn der Traffic-Manager oder eine andere Person, die für die Überprüfung oder Zuweisung der eingehenden Anfragen zuständig ist, nicht verfügbar ist, eine Sicherung automatisch verfügbar ist und Zugriff auf die Anfrageinformationen hat.

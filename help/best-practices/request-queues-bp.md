---
title: Best Practice – Anfrage-Warteschlangen
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Anfrage-Warteschlangen empfehlen.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1480'
ht-degree: 100%

---

# Best Practice – Anfrage-Warteschlangen

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Im Bereich „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

</br>
</br>

## Best Practices für Anfrage-Warteschlangen

* Fügen Sie eine Beschreibung für jedes Element einer Anfrage-Warteschlange ein – das Projekt der Anfrage-Warteschlange, Themengruppen, Warteschlangenthemen und Routing-Regeln.

* Erstellen Sie einen Projektstatus mit dem Namen „Anfrage-Warteschlange“ oder „Operativ“, der „Aktuell“ entspricht, um Anfrage-Warteschlangenprojekte von anderen Projekten zu unterscheiden.

* Wenn Sie beabsichtigen, Problemgenehmigungen für über eine Warteschlange gesendete Anfragen zu verwenden, erstellen Sie einen Problemstatus namens „Abgelehnt“.

* Weisen Sie „universelle“ benutzerdefinierte Formulare an Anfrage-Warteschlangen zu, um so viele unternehmensweit konsistente Daten wie möglich zu erfassen.

* Vermeiden Sie die Freigabe von Anfrage-Warteschlangen für „alle“. Richten Sie die Einstellungen für die Warteschlangendetails so ein, dass Benutzende nur die Warteschlangen sehen, die für ihre Bedürfnisse relevant sind.

* Erstellen Sie ein Dashboard mit Anfrage-Warteschlangenberichten, damit Traffic-Managerinnen und -Manager, Systemadmins oder zugewiesene Benutzende Probleme direkt bearbeiten können.

* Verwenden Sie Layout-Vorlagen, um die Einrichtungsoptionen für Anfrage-Warteschlangen aus dem Menü des linken Bedienfelds von Projekten für Benutzende zu entfernen, die keine Warteschlangen erstellen müssen.

* Erstellen Sie eine Anfrage-Warteschlange für Systemadmins, worüber Benutzende Workfront-bezogene Fragen stellen, Anfragen bezüglich der Systemeinrichtung stellen, neue Benutzerschulungen planen können usw.

* Überprüfen Sie die Anfrage-Warteschlangen regelmäßig, um nicht verwendete Warteschlangen zu identifizieren und deren Freigabe aufzuheben.

* Verwenden Sie Themengruppen, um bei mehr als 10 Warteschlangenthemen in einer Anfrage-Warteschlange diese zu organisieren, indem kürzere, einfacher zu verwaltende Listen erstellt werden.

* Steuern Sie die Gesamtzahl der für Benutzende verfügbaren Anfrage-Warteschlangen, indem Sie eine Anfrage-Warteschlange anhand von Themengruppen und Warteschlangenthemen aufschlüsseln, anstatt mehrere Warteschlangen zu erstellen.

* Richten Sie für jedes Warteschlangenthema Routing-Regeln ein. Richten Sie mindestens eine Standard-Routing-Regel ein.

* Nutzen Sie Themengruppen und Warteschlangenthemen, wenn ein selektives Routing erforderlich ist.

* Senden Sie Anfragen an ein Team und nicht an eine Einzelperson.


</br>
</br>


## Warum sind das Best Practices?


**Best Practice**

Fügen Sie eine Beschreibung für jedes Element einer Anfrage-Warteschlange ein – das Projekt der Anfrage-Warteschlange, Themengruppen, Warteschlangenthemen und Routing-Regeln.

**Das sind die Gründe**

Beschreibungen informieren Gruppenadmins, zukünftige Systemadmins oder andere, die Anfrage-Warteschlangen verwalten, darüber, was genau jeder Teil der Anfrage-Warteschlange tut.

Die Beschreibungsinformationen werden auch angezeigt, wenn Sie den Mauszeiger über das Informationssymbol im Feld im Fenster für eine neue Anfrage bewegen.

Die Beschreibung muss nicht lang sein, ein kurzer Kommentar zum Zweck oder zur Verwendung des Elements reicht.

</br>
</br>

**Best Practice**

Erstellen Sie einen Projektstatus mit dem Namen „Anfrage-Warteschlange“ oder „Operativ“, der „Aktuell“ entspricht, um Anfrage-Warteschlangenprojekte von anderen Projekten zu unterscheiden.

**Das sind die Gründe**

Eine Anfrage-Warteschlange „lebt“ in einem Projekt und muss sich in einem Status befinden, der „aktuell“ entspricht, damit die Warteschlange aktiv ist.

Um eine Anfrage von tatsächlichen Arbeitsprojekten mit dem Status „Aktuell“ zu unterscheiden, erstellen Sie einen Status, der nur für Anfragewarteschlangen verwendet wird und etwa „Anfragewarteschlange“ oder „Operativ“ heißt. Anschließend können Sie diesen Status verwenden, um beim Schreiben von Berichten Anfrage-Warteschlangenprojekte aus- oder einzuschließen.

</br>
</br>

**Best Practice**

Erstellen Sie bei der Verwendung von Problemgenehmigungen den Fehlerstatus „Abgelehnt“ und legen Sie für die Option „Wenn abgelehnt“ den Status „Abgelehnt“ fest.

**Das sind die Gründe**

Durch die Verwendung des Status „Abgelehnt“ wird deutlich, dass die Anfrage geprüft und abgelehnt wurde.

</br>
</br>

**Best Practice**

Weisen Sie „universelle“ benutzerdefinierte Formulare an Anfrage-Warteschlangen zu, um so viele unternehmensweit konsistente Daten wie möglich zu erfassen.

**Das sind die Gründe**

Ein „universelles“ benutzerdefiniertes Formular erfasst die für die Anfrage benötigten Standardinformationen, unabhängig vom Typ der gesendeten Anfrage.

Mit einem „universellen“ benutzerdefinierten Formular können Sie die Anzahl der benutzerdefinierten Formulare reduzieren, die Sie erstellen und pflegen müssen. Außerdem wird dadurch sichergestellt, dass alle Anfragen dieselben Informationen auf die gleiche Weise erfassen, was zu einer konsistenten Berichterstellung und Datenanalyse führt.

</br>
</br>

**Best Practice**

Vermeiden Sie die Freigabe von Anfrage-Warteschlangen für „alle“.  Richten Sie die Einstellungen für die Warteschlangendetails so ein, dass Benutzende nur die Warteschlangen sehen, die für ihre Bedürfnisse relevant sind.

**Das sind die Gründe**

In den meisten Fällen muss eine Anfrage-Warteschlange nur für eine bestimmte Gruppe von Personen wie ein Team, einen Lieferanten, Kundinnen und Kunden usw. freigegeben werden. Wenn Menschen, die eine Anfrage starten wollen, in der Liste der Anfrage-Warteschlangen nur das sehen, was sie benötigen, ist es einfach, Dinge zu finden und zu navigieren.

</br>
</br>


**Best Practice**

Erstellen Sie ein Dashboard mit Anfrage-Warteschlangenberichten, damit Traffic-Managerinnen und -Manager, Systemadmins oder zugewiesene Benutzende Probleme direkt bearbeiten können.

**Das sind die Gründe**

Wenn Benutzende schnell und einfach auf eingehende Anfragen zugreifen können, geht keine Arbeit unter.

</br>
</br>

**Best Practice**

Verwenden Sie Layout-Vorlagen, um die Einrichtungsoptionen für Anfrage-Warteschlangen aus dem Menü des linken Bedienfelds von Projekten für Benutzende zu entfernen, die keine Warteschlangen erstellen müssen.


**Das sind die Gründe**

Dadurch wird sichergestellt, dass alle Anfrage-Warteschlangen den richtigen Prozess zur Erstellung durchlaufen (z. B. durch einen Governance-Ausschuss überprüft werden) und entweder von System- oder Gruppenadmins korrekt eingerichtet werden.

Darüber hinaus hilft dies, die Warteschlangenliste organisiert zu halten und sich auf die Arten von Anfragen zu konzentrieren, die Ihr Unternehmen benötigt.

</br>
</br>

**Best Practice**

Erstellen Sie eine Anfrage-Warteschlange für Systemadmins, worüber Benutzende Workfront-bezogene Fragen stellen, Anfragen bezüglich der Systemeinrichtung stellen, neue Benutzerschulungen planen können usw.

**Das sind die Gründe**

Dies bietet einen zentralen Ort, an dem Benutzende Fragen stellen können und Admins Fragen zu Workfront-bezogenen Problemen sammeln, überwachen und beantworten können.

Darüber hinaus können diese Informationen verwendet werden, um gegenüber den Führungskräften die Zeit, den Arbeitsaufwand und den Wert der Systemadministratorrolle oder den Bedarf nach zusätzlichen Systemadmins zu rechtfertigen.

</br>
</br>


**Best Practice**

Überprüfen Sie die Anfrage-Warteschlangen regelmäßig, um nicht verwendete Warteschlangen zu identifizieren und deren Freigabe aufzuheben.

**Das sind die Gründe**

Eine regelmäßige Überprüfung der Einstellungen und Elemente in Ihrem Adobe Workfront-System trägt dazu bei, dass es übersichtlich bleibt und keine überflüssigen Elemente enthält. Wenn eine Warteschlange nicht mehr verwendet oder überwacht wird, stellen Sie sicher, dass Benutzende nicht mehr darauf zugreifen können, damit Arbeitsanfragen nicht ins Leere laufen.

</br>
</br>


**Best Practice**

Verwenden Sie Themengruppen, um bei mehr als 10 Warteschlangenthemen in einer Anfrage-Warteschlange diese zu organisieren, indem kürzere, einfacher zu verwaltende Listen erstellt werden.

**Das sind die Gründe**

Themengruppen erhöhen die Benutzerakzeptanz und sorgen für weniger Verwirrung, da die anfängliche Liste der auszuwählenden Optionen kürzer wird. Dadurch können Benutzende leichter finden, wonach sie suchen, ohne beim Senden einer Anfrage überfordert zu sein.

Darüber hinaus können Systemadmins und/oder Managerinnen und Manager von Anfrage-Warteschlangen einen reibungslosen Navigationspfad für Benutzende erstellen und die Organisation und Berichterstellung für die Typen der gesendeten Anfragen verbessern.

</br>
</br>

**Best Practice**

Steuern Sie die Gesamtzahl der für Benutzende verfügbaren Anfrage-Warteschlangen, indem Sie eine Anfrage-Warteschlange anhand von Themengruppen und Warteschlangenthemen aufschlüsseln, anstatt mehrere Warteschlangen zu erstellen.

**Das sind die Gründe**

Zu viele Anfrage-Warteschlangen machen es für Benutzende schwierig, das zu finden, was sie benötigen.

Weniger Warteschlangen helfen auch Menschen, die Traffic koordinieren, Systemadmins oder anderen, die die Warteschlangen verwalten, damit sie die benötigten Informationen schneller finden können, ohne zu mehreren Projekten in einer Anfrage-Warteschlange navigieren zu müssen.

Erstellen Sie mehrere Anfrage-Warteschlangen, wenn für verschiedene Anfrage-Warteschlangen verschiedene Arten von Zugriff erforderlich sind oder wenn eine Konsolidierung von Warteschlangen für die Benutzenden verwirrend wäre.

</br>
</br>

**Best Practice**

Richten Sie für jedes Warteschlangenthema Routing-Regeln ein. Richten Sie mindestens eine Standard-Routing-Regel ein.

**Das sind die Gründe**

Routing-Regeln stellen sicher, dass die eingehende Anfrage immer jemandem zugewiesen wird, damit keine Arbeit übersehen wird.

</br>
</br>

**Best Practice**

Nutzen Sie Themengruppen und Warteschlangenthemen, wenn ein selektives Routing erforderlich ist.

**Das sind die Gründe**

Routing-Regeln können nicht auf Felder eines benutzerdefinierten Formulars angewendet werden. Wenn also Anfragen unterschiedlicher Arten an verschiedene Teams/Einzelpersonen weitergeleitet werden müssen, erstellen für Sie jeden Anfragetyp ein eigenes Warteschlangenthema oder eine Themengruppe, damit die Arbeit ordnungsgemäß weitergeleitet werden kann.

</br>
</br>

**Best Practice**

Senden Sie Anfragen an ein Team und nicht an eine Einzelperson.

**Das sind die Gründe**

Wenn Anfragen an das Team geschickt werden, erhält das gesamte Team einen Überblick über die gestellten Anfragen und die anstehenden Arbeiten. Jeder kann die Team-Seite auf neue Elemente überprüfen oder die neuen Funktionen mit einem Bericht in einem Dashboard verfolgen.

Außerdem wird sichergestellt, dass, wenn Traffic-Managerinnen und -Manager oder andere Personen, die für die Überprüfung oder Zuweisung der eingehenden Anfragen zuständig sind, nicht verfügbar sind, automatisch eine Sicherung verfügbar ist und Zugriff auf die Anfrageinformationen hat.

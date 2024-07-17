---
title: Best Practice – Textmodusberichte
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Textmodusberichten empfehlen.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# Best Practice – Textmodusberichte

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Im Bereich „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

</br>
</br>

## Best Practices – Textmodusberichte

* Verwenden Sie in den Spalten des Listenberichts möglichst Wertausdrücke im Textmodus anstelle berechneter benutzerdefinierter Felder.

* Fügen Sie die in einer Textmodusberechnung verwendeten Berechnungen in die Beschreibung des Berichts ein.

</br>
</br>

## Warum sind das Best Practices?

**Best Practice**

Verwenden Sie in den Spalten des Listenberichts möglichst Wertausdrücke im Textmodus anstelle berechneter benutzerdefinierter Felder.



**Das sind die Gründe**

Wertausdrücke im Textmodus werden zum Zeitpunkt der Berichtsausführung berechnet und bei jedem Aktualisieren des Berichts neu berechnet. So haben Sie stets aktuelle Daten und genaue Berichte haben.



Berechnete benutzerdefinierte Felder (die in benutzerdefinierten Formularen verwendet werden) werden nicht automatisch aktualisiert, wenn die Daten in Workfront angezeigt werden. Stattdessen zeigen sie die Ergebnisse der letzten in Workfront gespeicherten Berechnung an. Das bedeutet, dass diese Werte zu einem bestimmten Zeitpunkt veraltet sein können. Berechnete benutzerdefinierte Felder müssen manuell aktualisiert werden, entweder durch Neuberechnung des Ausdrucks oder durch Bearbeiten und Speichern des Objekts, das das berechnete Feld enthält. Dies kann zeitaufwendig sein und leicht vergessen werden.


</br>
</br>

**Best Practice**

Fügen Sie die in einer Textmodusberechnung verwendeten Berechnungen in die Beschreibung des Berichts ein.



**Das sind die Gründe**

Die Aufnahme von Textmodusberechnungen in die Berichtsbeschreibung hilft anderen, zu verstehen, wie die Berechnung erstellt wurde und welche Art von Informationen angezeigt werden sollen. Außerdem werden Systemadmins daran erinnert, wie der Bericht erstellt wurde, falls in Zukunft Aktualisierungen erforderlich sind.

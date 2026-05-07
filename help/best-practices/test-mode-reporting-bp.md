---
title: Best Practice – Textmodusberichte
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Textmodusberichten empfehlen.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
TQID: https://experienceleague.adobe.com/k8DYutzVcGrJc7p0x74B2iQ3nkiohWeQu1egOWZ34AI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 90%

---

# Best Practice – Textmodusberichte

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Der Bereich „Warum sind diese Best Practices?“, der nach der allgemeinen Liste zu finden ist, bietet detailliertere Informationen zu einigen der Best Practices und warum sie als Prozess, Tool usw. angesehen werden. Sie sollten die Implementierung mit Ihrer Workfront-Instanz in Betracht ziehen.

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

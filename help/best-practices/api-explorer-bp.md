---
title: Best Practice – API Explorer
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront API Explorer empfehlen.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
TQID: https://experienceleague.adobe.com/RUQeNzEb0eg9DKSKepugb0HD4O2ODql-0mWBn-ptgxk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: bb1dd007-4a34-496d-9d3b-2278fdaadac1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 75%

---

# Best Practice – API Explorer

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Der Bereich „Warum sind diese Best Practices?“, der nach der allgemeinen Liste zu finden ist, bietet detailliertere Informationen zu einigen der Best Practices und warum sie als Prozess, Tool usw. angesehen werden. Sie sollten die Implementierung mit Ihrer Workfront-Instanz in Betracht ziehen.

</br>
</br>

## Best Practices – API Explorer

* Legen Sie eine Benennungskonvention für benutzerdefinierte Felder fest, die mit Integrationen aus Drittanbietersystemen verwendet werden.

* Verfolgen Sie alle benutzerdefinierten Felder, die in Integrationen mithilfe eines Workfront-Projekts verwendet werden.

* Fügen Sie das Feld „Objekt-ID“ zu Berichten hinzu, die von Systemadmins verwendet werden.

</br>
</br>

## Warum sind das Best Practices?

**Best Practice**

Legen Sie eine Benennungskonvention für benutzerdefinierte Felder fest, die mit Integrationen aus Drittanbietersystemen verwendet werden.

**Das sind die Gründe**

Stellen Sie sicher, dass alle Personen, die benutzerdefinierte Formulare erstellen, die Namenskonvention kennen, damit sie nicht versehentlich ein für eine Integration reserviertes Feld verwenden. Abhängig von Ihren Integrationen und Workflows kann die Verwendung desselben Felds auf unterschiedliche Weise dazu führen, dass Daten geändert oder überschrieben werden, und so zu falschen Daten in Berichten führen.

</br>
</br>


**Best Practice**

Verfolgen Sie alle benutzerdefinierten Felder, die in Integrationen mithilfe eines Workfront-Projekts verwendet werden.

**Das sind die Gründe**

Ein Projekt ist der perfekte Ort, um benutzerdefinierte Feldnamen, deren Integration usw. zu protokollieren. Auf diese Weise vermeiden Sie das Erstellen redundanter benutzerdefinierter Felder oder die Verwendung desselben benutzerdefinierten Felds mit mehreren Integrationen.

</br>
</br>


**Best Practice**

Fügen Sie das Feld „Objekt-ID“ zu Berichten hinzu, die von Systemadmins verwendet werden.

**Das sind die Gründe**

Systemadmins müssen sich bei der Verwendung von APIs oder anderen Integrationen häufig durch ihre ID-Nummern auf Objekte in Workfront beziehen. Schließen Sie das Feld ID in die Ansichten der Objekte ein, an denen Sie arbeiten (Projekte, Aufgaben, Probleme, Vorlagen, benutzerdefinierte Formulare usw.) um den Zugriff und das Kopieren zu vereinfachen.

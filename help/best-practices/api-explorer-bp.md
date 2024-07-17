---
title: Best Practice – API Explorer
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront API Explorer empfehlen.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 100%

---

# Best Practice – API Explorer

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Im Bereich „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

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

Ein Projekt ist der perfekte Ort, um die Namen von benutzerdefinierten Feldern, ihre Verwendung in der Integration usw. zu protokollieren. Auf diese Weise vermeiden Sie die Erstellung redundanter benutzerdefinierter Felder oder die Verwendung desselben benutzerdefinierten Felds mit mehreren Integrationen.

</br>
</br>


**Best Practice**

Fügen Sie das Feld „Objekt-ID“ zu Berichten hinzu, die von Systemadmins verwendet werden.

**Das sind die Gründe**

Systemadmins müssen sich bei der Verwendung von APIs oder anderen Integrationen häufig durch ihre ID-Nummern auf Objekte in Workfront beziehen. Fügen Sie das ID-Feld in Ansichten für die Objekte ein, an denen Sie arbeiten (Projekte, Aufgaben, Probleme, Vorlagen, benutzerdefinierte Formulare usw.), um den Zugriff und das Kopieren zu erleichtern.

---
title: Best Practice - API Explorer
description: Erfahren Sie mehr über Best Practices von Adobe Workfront-Experten zur Einrichtung, Verwaltung und Verwendung von Workfront API Explorer.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Best Practice - API Explorer

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für API Explorer

* Legen Sie eine Benennungskonvention für benutzerdefinierte Felder fest, die mit Integrationen aus Drittanbietersystemen verwendet werden.

* Verfolgen Sie alle benutzerdefinierten Felder, die in Integrationen mit einem Workfront-Projekt verwendet werden.

* Fügen Sie das Objekt-ID-Feld zu Berichten hinzu, die vom Systemadministrator verwendet werden.

</br>
</br>

## Warum sind diese Best Practices?

**Best Practice**

Legen Sie eine Benennungskonvention für benutzerdefinierte Felder fest, die mit Integrationen aus Drittanbietersystemen verwendet werden.

**Deshalb**

Stellen Sie sicher, dass alle, die benutzerdefinierte Formulare erstellen, über die Namenskonvention Bescheid wissen, damit sie nicht versehentlich ein für eine Integration reserviertes Feld verwenden. Abhängig von Ihren Integrationen und Workflows kann die Verwendung desselben Felds auf unterschiedliche Weise dazu führen, dass Daten geändert oder überschrieben werden, was zu falschen Daten in Berichten führen kann.

</br>
</br>


**Best Practice**

Verfolgen Sie alle benutzerdefinierten Felder, die in Integrationen mit einem Workfront-Projekt verwendet werden.

**Deshalb**

Ein Projekt ist der perfekte Ort, um benutzerdefinierte Feldnamen zu protokollieren, mit welcher Integration sie verwendet werden usw. Auf diese Weise vermeiden Sie die Erstellung redundanter benutzerdefinierter Felder oder die Verwendung desselben benutzerdefinierten Felds mit mehreren Integrationen.

</br>
</br>


**Best Practice**

Fügen Sie das Objekt-ID-Feld zu Berichten hinzu, die vom Systemadministrator verwendet werden.

**Deshalb**

Systemadministratoren müssen bei der Verwendung von APIs oder anderen Integrationen häufig anhand ihrer ID-Nummer auf Objekte in Workfront verweisen. Schließen Sie das ID-Feld in Ansichten für die Objekte ein, an denen Sie arbeiten (Projekte, Aufgaben, Probleme, Vorlagen, benutzerdefinierte Formulare usw.) um den Zugriff und das Kopieren zu erleichtern.

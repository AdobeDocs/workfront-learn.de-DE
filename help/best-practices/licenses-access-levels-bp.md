---
title: Best Practice - Lizenzen und Zugriffsstufen
description: Erfahren Sie mehr über Best Practices von Adobe Workfront-Experten für die Einrichtung, Verwaltung und Verwendung von Workfront-Lizenzen und -Zugriffsebenen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Best Practice - Lizenzen und Zugriffsstufen

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für Lizenzen und Zugriffsstufen

* Beginnen Sie mit geringerem Zugriff für Benutzer beim Einrichten von Zugriffsebenen.

* Beim Zuweisen von Review- und Anforderungslizenzen wird in der Regel standardmäßig &quot;Überprüfen&quot;verwendet, da der Benutzer mehr Berechtigungen in Adobe Workfront erhält.

* Deaktivieren Sie das Kontrollkästchen &quot;Systemweit freigeben&quot;für jedes Objekt in allen Zugriffsebenen, es sei denn, Sie möchten ausdrücklich, dass diese Benutzer dazu in der Lage sein sollen.

* Erwägen Sie die Aktivierung der Einstellung &quot;Benutzer dürfen Kommentare nie löschen&quot;unter Festlegen zusätzlicher Einschränkungen auf einer Zugriffsebene.

* Beschränken Sie die Anzahl der Systemadministratoren zugunsten von Gruppenadministratoren.

* Kopieren Sie eine vorhandene Zugriffsebene und nehmen Sie Änderungen vor, anstatt eine neue Zugriffsebene von Grund auf neu zu erstellen.

* Dokumentieren Sie im Feld &quot;Beschreibung&quot;die Möglichkeiten jeder Zugriffsebene.

* Beschränken Sie sich auf die Zugriffsebenen, die zur Erreichung Ihrer Arbeitsziele erforderlich sind, idealerweise vier oder fünf, die die Anforderungen der meisten Benutzer im System erfassen.

* Weisen Sie mindestens zwei Benutzern die Zugriffsstufe des globalen Systemadministrators zu.

* Beschränken Sie, was Benutzer mit Workfront-Elementen tun können, indem Sie sie freigeben, anstatt eine Funktion auf einer Zugriffsebene zu entfernen.

</br>
</br>


## Warum sind diese Best Practices?

**Best Practice**

Beginnen Sie mit geringerem Zugriff für Benutzer beim Einrichten von Zugriffsebenen.



**Deshalb**

Beginnen Sie Benutzer mit dem minimalen Zugriff, den sie für ihre Arbeit benötigen. Wenn sie ihre Arbeit aufgrund unzureichender Zugriffsberechtigungen nicht ausführen können, fordern sie normalerweise zusätzlichen Zugriff an. Wird Benutzern sofort zu viel Zugriff gewährt, kann dies zu Sicherheitsproblemen führen. Außerdem ist es immer besser, Benutzern mehr Zugriff zu gewähren, als den Zugriff zu nehmen.

</br>
</br>



**Best Practice**

Beim Zuweisen von Review- und Anforderungslizenzen wird in der Regel standardmäßig &quot;Überprüfen&quot;verwendet, da der Benutzer mehr Berechtigungen in Adobe Workfront erhält.



**Deshalb**

Obwohl die Lizenzen für Review und Request einer unbegrenzten Anzahl von Benutzern in Workfront zugewiesen werden können, beschränken sich die Lizenzen für Anfragen auf das bloße Erstellen und Aktualisieren von Anforderungen. Eine Überprüfungslizenz hat mehr Zugriff auf Projekte und Aufgaben als eine Anforderungslizenz. Sie bietet außerdem die Möglichkeit, Portfolios und Programme anzuzeigen, Dokumente zu bearbeiten und auf Tools zur Ressourcenverwaltung zuzugreifen.

</br>
</br>

**Best Practice**

Deaktivieren Sie das Kontrollkästchen &quot;Systemweit freigeben&quot;für jedes Objekt in allen Zugriffsebenen, es sei denn, es gibt einen bestimmten Grund, warum Benutzer systemweit freigeben können müssen.



**Deshalb**

Die systemweite Freigabe eines Objekts wird häufig als Krücken verwendet, um bestimmten Benutzern die Anzeige von Elementen in Workfront zu ermöglichen. Dies geschieht, wenn die Workfront-Gruppenstruktur fehlt oder die Freigabeberechtigungen nicht vollständig verstanden wurden. Wenn Elemente systemweit freigegeben werden, bedeutet dies, dass jeder das freigegebene Element sehen kann. Je nach Art der im System gespeicherten Informationen kann dies zu Datenschutzproblemen führen.



Beispielsweise können Sie mit mehreren Anbietern in Workfront zusammenarbeiten, um den Fortschritt zu überprüfen, Genehmigungen bereitzustellen usw. Wenn das Kontrollkästchen &quot;Systemweit freigeben&quot;eine Option ist, die als Standard ausgewählt oder festgelegt werden kann, sodass Informationen allen Anbietern zur Verfügung stehen.



Indem Sie die Option ganz deaktivieren, müssen Benutzer, die die Berechtigung zum Freigeben besitzen, die bestimmte(n) Person(en) bestimmen - entweder über ein Unternehmen, eine Gruppe oder ein Team -, für die/das sie das Objekt freigeben möchten.

</br>
</br>

**Best Practice**

Erwägen Sie die Aktivierung der Einstellung &quot;Benutzer dürfen Kommentare nie löschen&quot;unter Festlegen zusätzlicher Einschränkungen auf einer Zugriffsebene.



**Deshalb**

Durch Aktivierung dieser Option wird sichergestellt, dass vergangene Nachrichten nicht aus Workfront entfernt werden. Einige Organisationen verlangen, dass der vollständige Kommentar-Verlauf zu Prüfungszwecken beibehalten wird.

</br>
</br>

**Best Practice**

Beschränken Sie die Anzahl der Systemadministratoren zugunsten von Gruppenadministratoren.



**Deshalb**

Systemadministratoren haben Zugriff auf alles in Workfront, einschließlich globaler Systemeinstellungen. Die für Administratoren der Einstellungsgruppe verfügbaren Administratoren werden vom Systemadministrator kontrolliert und gelten nur für diese spezifische Gruppe.



Mit Gruppenadministratoren können Systemadministratoren viele Aufgaben delegieren, sodass sie sich auf größere Bildelemente konzentrieren können, anstatt sich auf die tägliche Wartung von Workfront zu konzentrieren. Gruppenadministratoren können einfacher mit den Anforderungen ihrer Gruppen in Kontakt bleiben, was den Benutzern einen besseren Service bietet.

</br>
</br>


**Best Practice**

Kopieren Sie eine vorhandene Zugriffsebene und nehmen Sie Änderungen vor, anstatt eine neue Zugriffsebene von Grund auf neu zu erstellen.



**Deshalb**

Das Kopieren einer vorhandenen Zugriffsebene bietet eine konsistente Grundlage für neue Zugriffsebenen, um sicherzustellen, dass die anfänglichen Einstellungen identisch sind. Dies spart auch Zeit, da Systemadministratoren keine völlig neue Zugriffsebene einrichten müssen.

</br>
</br>

**Best Practice**

Dokumentieren Sie im Feld &quot;Beschreibung&quot;die Möglichkeiten jeder Zugriffsebene.



**Deshalb**

Machen Sie sich mit der Beschreibung und den Einstellungen für jeden Objekttyp vertraut. Dies hilft Systemadministratoren - aktuell und zukünftig - genau zu wissen, was jede Zugriffsebene tut, ohne sich in die Zugriffsebene selbst eintauchen zu müssen, um die Einstellungen zu überprüfen.



Dies kann auch den Vergleich von Zugriffsebenen erleichtern, wenn sie in einem Bericht betrachtet werden. Das Beschreibungsfeld kann der Ansicht schnell hinzugefügt werden, um schnell zu sehen, wie sie sich unterscheiden und möglicherweise warum eine andere Zugriffsebene erstellt wurde.

</br>
</br>

**Best Practice**

Beschränken Sie sich auf die Zugriffsebenen, die zur Erreichung Ihrer Arbeitsziele erforderlich sind, idealerweise vier oder fünf, die die Anforderungen der meisten Benutzer im System erfassen.


**Deshalb**

Die Zugriffsebene stellt sicher, dass Benutzer, die ein Workfront-Objekt für einen Benutzer freigeben, über die erforderlichen Berechtigungen zum Bearbeiten, Löschen usw. verfügen. Sie können die Zugriffsebenen allgemeiner gestalten, da die Freigabe für einzelne Elemente so konfiguriert werden kann, dass sie spezifischer sind.


Darüber hinaus kann es durch weniger Zugangsstufen einfacher werden, ein übersichtliches System zu erhalten und eine Strategie zu implementieren, die auch zu einem schnelleren Onboarding führen kann, wenn Personen in den Unternehmens- oder Abteilungen wechseln.

</br>
</br>

**Best Practice**

Weisen Sie mindestens zwei Benutzern die Zugriffsstufe des globalen Systemadministrators zu.

**Deshalb**

Mehr als eine Person sollte verstehen, warum die Workfront so konfiguriert wurde, wie sie war, wie sie sie verwaltet/verwaltet und wie sie Benutzer unterstützt. Wenn eine Person nicht im Büro ist, die Organisation verlässt, beschäftigt ist usw., stellt dies sicher, dass eine andere Person über die Informationen und das Wissen verfügt, um das System erfolgreich zu verwalten.

</br>
</br>

**Best Practice**

Beschränken Sie, was Benutzer mit Workfront-Elementen tun können, indem Sie sie freigeben, anstatt eine Funktion auf einer Zugriffsebene zu entfernen.


**Deshalb**

Die Zugriffsebenen steuern, was Benutzer mit bestimmten Elementen auf globaler Ebene tun können. Die Freigabeberechtigungen für jedes Projekt, jede Aufgabe, jedes Portfolio, jedes Dokument usw. steuern, was ein einzelner Benutzer mit diesem bestimmten Element tun kann. Anstatt eine Funktion für alle Benutzer mit einer bestimmten Zugriffsstufe zu entfernen, passen Sie die Freigabeberechtigungen für bestimmte Elemente an, damit Benutzer über eingeschränkte Steuerelemente verfügen.

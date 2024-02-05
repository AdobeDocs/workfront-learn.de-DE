---
title: Best Practice – Lizenzen und Zugriffsebenen
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Lizenzen und Zugriffsebenen empfehlen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1253'
ht-degree: 100%

---

# Best Practice – Lizenzen und Zugriffsebenen

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Im Bereich „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

</br>
</br>

## Best Practices für Lizenzen und Zugriffsebenen

* Beginnen Sie bei der Einrichtung von Zugriffsebenen mit weniger Zugriffsrechten für die Benutzenden.

* Bei der Zuweisung von Prüf- und Anfragelizenzen wird in der Regel der Standardwert „Überprüfung“ verwendet, da Benutzende dadurch mehr Berechtigungen in Adobe Workfront erhalten.

* Deaktivieren Sie das Kontrollkästchen „systemweite Freigabe“ bei jedem Objekt in allen Zugriffsebenen, es sei denn, Sie möchten ausdrücklich, dass diese Benutzenden sie erhalten.

* Ziehen Sie in Erwägung, die Einstellung „Niemals zulassen, dass Benutzer Kommentare löschen“ unter „Zusätzliche Einschränkungen in einer Zugriffsebene festlegen“ zu aktivieren.

* Begrenzen Sie die Anzahl der Systemadmins zugunsten von Gruppenadmins.

* Kopieren Sie lieber eine vorhandene Zugriffsebene und nehmen Sie Änderungen vor, anstatt eine neue Zugriffsebene von Grund auf neu zu erstellen.

* Dokumentieren Sie im Feld „Beschreibung“, was jede Zugriffsebene tun darf.

* Beschränken Sie sich auf die Zugriffsebenen, die zum Erreichen Ihrer Arbeitsziele notwendig sind, idealerweise vier oder fünf, die die Bedürfnisse der meisten Benutzenden im System abdecken.

* Weisen Sie mindestens zwei Personen die Zugriffsebene „globale Systemadmins“ zu.

* Schränken Sie ein, was Benutzende mit Workfront-Elementen durch Freigabe tun können, anstatt eine Fähigkeit in einer Zugriffsebene zu entfernen.

</br>
</br>


## Warum sind das Best Practices?

**Best Practice**

Beginnen Sie bei der Einrichtung von Zugriffsebenen mit weniger Zugriffsrechten für die Benutzenden.



**Das sind die Gründe**

Geben Sie Benutzenden zuerst nur den Mindestzugang, den sie für ihre Arbeit benötigen. Wenn sie ihre Arbeit aufgrund unzureichender Zugriffsrechte nicht erledigen können, beantragen sie dann in der Regel zusätzlichen Zugriff. Wenn Sie den Benutzenden sofort zu viel Zugriff gewähren, kann dies zu Sicherheitsproblemen führen. Außerdem ist es immer besser, den Benutzenden nachträglich mehr Zugriff zu gewähren, als ihnen einen Zugriff zu entziehen.

</br>
</br>



**Best Practice**

Bei der Zuweisung von Prüf- und Anfragelizenzen wird in der Regel der Standardwert „Überprüfung“ verwendet, da Benutzende dadurch mehr Berechtigungen in Adobe Workfront erhalten.



**Das sind die Gründe**

Obwohl sowohl Überprüfungs- als auch Anfragelizenzen einer unbegrenzten Anzahl von Benutzenden in Workfront zugewiesen werden können, sind die Anfragelizenzen im Wesentlichen auf das Erstellen und Aktualisieren von Anfragen beschränkt. Eine Überprüfungslizenz bietet mehr Zugriff auf Projekte und Aufgaben als eine Anfragelizenz sowie die Möglichkeit, Portfolios und Programme einzusehen, Dokumente zu bearbeiten und auf Ressourcen-Management-Tools zuzugreifen.

</br>
</br>

**Best Practice**

Deaktivieren Sie das Kontrollkästchen „systemweite Freigabe“ für jedes Objekt in allen Zugriffsebenen, es sei denn, es gibt einen bestimmten Grund, warum Benutzende die Möglichkeit haben müssen, etwas systemweit freizugeben.



**Das sind die Gründe**

Die systemweite Freigabe eines Objekts wird oft als Krücke verwendet, um bestimmten Benutzenden zu ermöglichen, Elemente in Workfront zu sehen. Dies geschieht, wenn die Workfront-Gruppenstruktur fehlt oder wenn die Freigabeberechtigungen nicht vollständig verstanden werden. Wenn Elemente systemweit freigegeben werden, bedeutet dies, dass alle das freigegebene Element sehen können. Je nach Art der im System gespeicherten Informationen kann dies zu Datenschutzproblemen führen.



So kann es beispielsweise sein, dass Sie mit mehreren Anbietern innerhalb von Workfront zusammenarbeiten, um den Fortschritt zu überprüfen, Genehmigungen zu erteilen usw. Wenn das Kontrollkästchen „Systemweit freigeben“ eine Option ist, könnte diese ausgewählt oder gar als Standard festgelegt werden, sodass die Informationen für alle Lieferanten verfügbar wären.



Wenn Sie die Option komplett deaktivieren, müssen Benutzende mit der Berechtigung zur Freigabe die Person(en) bestimmen, für die sie das Objekt freigeben möchten – entweder über ein Unternehmen, eine Gruppe oder ein Team.

</br>
</br>

**Best Practice**

Ziehen Sie in Erwägung, die Einstellung „Niemals zulassen, dass Benutzer Kommentare löschen“ unter „Zusätzliche Einschränkungen in einer Zugriffsebene festlegen“ zu aktivieren.



**Das sind die Gründe**

Durch die Aktivierung dieser Option wird sichergestellt, dass frühere Mitteilungen nicht aus Workfront entfernt werden. Einige Organisationen verlangen, dass der vollständige Kommentarverlauf zu Prüfzwecken aufbewahrt wird.

</br>
</br>

**Best Practice**

Begrenzen Sie die Anzahl der Systemadmins zugunsten von Gruppenadmins.



**Das sind die Gründe**

Systemadmins haben Zugriff auf alles in Workfront, einschließlich der globalen Systemeinstellungen. Die Einstellungen, auf die Gruppenadmins zugreifen können, werden von Systemadmins gesteuert und gelten nur für diese spezielle Gruppe.



Gruppenadmins ermöglichen es den Systemadmins, viele Aufgaben zu delegieren, sodass sie sich auf übergeordnete Themen konzentrieren können, anstatt sich um die tägliche Pflege von Workfront zu kümmern. Gruppenadmins können leichter mit den Bedürfnissen ihrer Gruppen in Kontakt bleiben, was einen besseren Service für die Benutzenden bedeutet.

</br>
</br>


**Best Practice**

Kopieren Sie lieber eine vorhandene Zugriffsebene und nehmen Sie Änderungen vor, anstatt eine neue Zugriffsebene von Grund auf neu zu erstellen.



**Das sind die Gründe**

Das Kopieren einer bestehenden Zugriffsebene bietet eine konsistente Grundlage für neue Zugriffsebenen und stellt sicher, dass die Anfangseinstellungen identisch sind. Dies bietet auch eine Zeitersparnis, da die Systemadmins eine Zugriffsebene nicht von Grund auf neu einrichten müssen.

</br>
</br>

**Best Practice**

Dokumentieren Sie im Feld „Beschreibung“, was jede Zugriffsebene tun darf.



**Das sind die Gründe**

Geben Sie eine detaillierte Beschreibung ab, in der Sie die Einstellungen für jeden Objekttyp auflisten. Dies hilft Systemadmins – gegenwärtigen und zukünftigen – genau zu wissen, was die einzelnen Zugriffsebenen bewirken, ohne dass sie in die Zugriffsebene selbst eintauchen müssen, um die Einstellungen zu überprüfen.



Dies kann auch das Vergleichen der Zugriffsebenen erleichtern, wenn sie in einem Bericht angezeigt werden. Das Beschreibungsfeld kann schnell zur Ansicht hinzugefügt werden, um schnell zu sehen, wie sie sich unterscheiden und möglicherweise auch, warum eine andere Zugriffsebene erstellt wurde.

</br>
</br>

**Best Practice**

Beschränken Sie sich auf die Zugriffsebenen, die zum Erreichen Ihrer Arbeitsziele notwendig sind, idealerweise vier oder fünf, die die Bedürfnisse der meisten Benutzenden im System abdecken.


**Das sind die Gründe**

Die Zugriffsebene stellt sicher, dass bei Freigabe eines Workfront-Objekts an Benutzende diese die erforderlichen Rechte zum Bearbeiten, Löschen usw. haben. Sie können die Zugriffsebenen allgemeiner gestalten, da die Freigabe für einzelne Elemente spezifischer konfiguriert werden kann.


Darüber hinaus können weniger Zugriffsebenen die Pflege eines übersichtlichen Systems und die Umsetzung einer Strategie erleichtern, was auch zu einem schnelleren Onboarding führen kann, wenn Mitarbeitende zum Unternehmen stoßen oder die Abteilung wechseln.

</br>
</br>

**Best Practice**

Weisen Sie mindestens zwei Personen die Zugriffsebene „globale Systemadmins“ zu.

**Das sind die Gründe**

Mehr als eine Person sollte verstehen, warum Workfront so konfiguriert wurde, wie es konfiguriert wurde, wie man es verwaltet und pflegt und wie man die Benutzenden unterstützt. Wenn eine Person abwesend ist, die Organisation verlässt, gerade beschäftigt ist usw., ist dadurch sichergestellt, dass eine andere Person über die Informationen und Kenntnisse verfügt, um das System erfolgreich zu verwalten.

</br>
</br>

**Best Practice**

Schränken Sie ein, was Benutzende mit Workfront-Elementen durch Freigabe tun können, anstatt eine Fähigkeit in einer Zugriffsebene zu entfernen.


**Das sind die Gründe**

Zugriffsebenen steuern, was Benutzende allgemein mit bestimmten Elementen tun können. Die Freigabeberechtigungen für jedes Projekt, jede Aufgabe, jedes Portfolio, jedes Dokument usw. steuern, was Einzelpersonen mit diesem spezifischen Element tun können. Anstatt eine Funktion für alle Benutzenden mit einer bestimmten Zugriffsebene zu entfernen, sollten Sie die Freigabeberechtigungen für bestimmte Objekte so anpassen, dass die Benutzenden nur eine begrenzte Kontrolle haben.

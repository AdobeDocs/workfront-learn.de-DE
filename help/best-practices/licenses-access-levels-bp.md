---
title: Best Practice – Lizenzen und Zugriffsebenen
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Lizenzen und Zugriffsebenen empfehlen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
TQID: https://experienceleague.adobe.com/YvTTPwGkach9JpmNHLxuLT3fpQ7KOzYjxtw-kdhFlEI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 1268
ht-degree: 90%

---

# Best Practice – Lizenzen und Zugriffsebenen

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Der Bereich „Warum sind diese Best Practices?“, der nach der allgemeinen Liste zu finden ist, bietet detailliertere Informationen zu einigen der Best Practices und warum sie als Prozess, Tool usw. angesehen werden. Sie sollten die Implementierung mit Ihrer Workfront-Instanz in Betracht ziehen.

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



Sie können beispielsweise mit mehreren Anbietern in Workfront zusammenarbeiten, um den Fortschritt zu überprüfen, Genehmigungen bereitzustellen usw. Wenn das Kontrollkästchen „Systemweit freigeben“ eine Option ist, kann diese als Standard ausgewählt oder festgelegt werden, sodass Informationen für alle Anbieter verfügbar sind.



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

Die Zugriffsebene stellt sicher, dass Benutzende bei der Freigabe eines Workfront-Objekts für Benutzende über die erforderlichen Berechtigungen zum Bearbeiten, Löschen usw. verfügen. Sie können die Zugriffsebenen allgemeiner gestalten, da die Freigabe für einzelne Elemente spezifischer konfiguriert werden kann.


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

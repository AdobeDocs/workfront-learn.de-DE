---
title: Best Practice – Voreinstellungen für Projekte, Aufgaben und Probleme
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Voreinstellungen für Projekte, Aufgaben und Probleme empfehlen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
TQID: https://experienceleague.adobe.com/2Nc0Sj-3xZ-H8ir2OvXLhRJFEEKZu0DM8jIbFvizqlM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 704
ht-degree: 89%

---

# Best Practice – Voreinstellungen für Projekte, Aufgaben und Probleme

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Der Bereich „Warum sind diese Best Practices?“, der nach der allgemeinen Liste zu finden ist, bietet detailliertere Informationen zu einigen der Best Practices und warum sie als Prozess, Tool usw. angesehen werden. Sie sollten die Implementierung mit Ihrer Workfront-Instanz in Betracht ziehen.

</br>
</br>

## Best Practices für Projekt-, Aufgaben- und Problemvoreinstellungen

* Setzen Sie den standardmäßigen Aufgabendauertyp auf „Einfach“.

* Legen Sie die Voreinstellung für den Status eines neuen Projekts auf „In Planung“ oder „Idee“ fest, nicht auf „Aktuell“.

* Aktivieren Sie in den globalen Projektvoreinstellungen die Option „Baselines automatisch erstellen“.

* Überprüfen Sie alle Optionen im Abschnitt „Business-Cases“ der Systemprojektvoreinstellungen.

* Aktivieren Sie in den Voreinstellungen für Probleme die Option für automatisches Aktualisieren des Status „Lösbares Problem“, wenn sich der Status des Lösungsobjekts ändert.

</br>
</br>


## Warum sind das Best Practices?

**Best Practice**

Setzen Sie den standardmäßigen Aufgabendauertyp auf „Einfach“.

**Das sind die Gründe**

Die Dauertypen definieren die Beziehung zwischen der Aufgabendauer, den geplanten Stunden und der Anzahl der der Aufgabe zugewiesenen Personen.

Wenn als globaler Systemstandard „Einfach“ eingestellt ist, haben alle manuell erstellten Aufgaben diesen Dauertyp. Die geplanten Stunden werden gleichmäßig über die gesamte Dauer auf die der Aufgabe zugewiesenen Personen verteilt. Der Dauertyp „Einfach“ kann die Projektplanung vereinfachen, da er es Ihnen ermöglicht, Änderungen an den der Aufgabe zugewiesenen Personen und geplanten Stunden vorzunehmen, ohne die Dauer der Aufgabe, das geplante Startdatum oder das geplante Abschlussdatum zu beeinträchtigen.

</br>
</br>

**Best Practice**

Legen Sie die Voreinstellung für den Status eines neuen Projekts auf „In Planung“ oder „Idee“ fest, nicht auf „Aktuell“.

**Das sind die Gründe**

Ist der Status „Aktuell“, bedeutet das, dass ein Projekt gerade läuft und aktiv bearbeitet wird. Es ist selten, dass ein Projekt bereits bei seiner Erstellung diesen Status haben sollte. Selbst wenn Sie eine Projektvorlage verwenden, ist eine gewisse „Planung“ erforderlich, um Aufgabenzuweisungen vorzunehmen, das geplante Abschlussdatum des Projekts anzupassen usw. Der Planungsstatus unterdrückt auch Benachrichtigungen an Aufgabenzugewiesene und Projektteammitglieder. Der Empfang von Benachrichtigungen vor der Live-Schaltung des Projekts kann für die Beteiligten verwirrend sein.

</br>
</br>

**Best Practice**

Aktivieren Sie in den globalen Projektvoreinstellungen die Option „Baselines automatisch erstellen“.

**Das sind die Gründe**

Jedes Mal, wenn Sie einen Projektstatus auf „Aktuell“ ändern, zeichnet Workfront automatisch eine Projekt-Baseline auf. Diese „Momentaufnahme“ des Projekts liefert historische Informationen darüber, wie sich der Projektplan im Laufe der Zeit verändert hat. Sie können beispielsweise den ursprünglichen Projektplan mit dem aktuellen Plan vergleichen, wenn Sie der Geschäftsführung zeigen möchten, wie sich die Verschiebung von Prioritäten oder die Ausweitung des Projektumfangs auf die Projekttermine ausgewirkt hat.

</br>
</br>

**Best Practice**

Überprüfen Sie alle Optionen im Abschnitt „Business-Cases“ der Systemprojektvoreinstellungen.

**Das sind die Gründe**

Aktivieren Sie alle fünf Optionen, damit Projekt-Managerinnen und -Manager, Planende und andere Personen jeden dieser Abschnitte in den Business-Case eines Projekts aufnehmen können. Wenn die Optionen nicht aktiviert sind, erscheinen sie nicht im Business-Case-Fenster. Die Benutzenden können ein Feld leer lassen, wenn es für das jeweilige Projekt nicht benötigt wird, aber sie können kein Feld auf Projektebene aktivieren. Diese Optionen können nur global im Setup aktiviert werden.

</br>
</br>

**Best Practice**

Aktivieren Sie in den Voreinstellungen für Probleme die Option für automatisches Aktualisieren des Status „Lösbares Problem“, wenn sich der Status des Lösungsobjekts ändert.

**Das sind die Gründe**

Wenn ein Problem in ein Projekt umgewandelt wird, „verknüpft“ diese Voreinstellung die Status der beiden Elemente. Durch die Aktualisierung des Projektstatus (des Lösungsobjekts) wird der Problemstatus automatisch aktualisiert. Das bedeutet, dass die anfragende Person den Fortschritt bei ihrer Anfrage sehen kann, selbst wenn sie nicht über die Berechtigung zum Anzeigen des gesamten Projekts in Workfront verfügt.

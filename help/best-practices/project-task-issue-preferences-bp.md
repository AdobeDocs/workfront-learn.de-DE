---
title: Best Practice – Voreinstellungen für Projekte, Aufgaben und Probleme
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Voreinstellungen für Projekte, Aufgaben und Probleme empfehlen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '702'
ht-degree: 100%

---

# Best Practice – Voreinstellungen für Projekte, Aufgaben und Probleme

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Im Bereich „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

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

Ist der Status „Aktuell“, bedeutet das, dass ein Projekt gerade läuft und aktiv bearbeitet wird. Es ist selten, dass ein Projekt bereits bei seiner Erstellung diesen Status haben sollte. Selbst wenn Sie eine Projektvorlage verwenden, ist eine gewisse „Planung“ erforderlich, um die Aufgabenzuweisungen vorzunehmen, das geplante Abschlussdatum des Projekts anzupassen usw. Der Status „In Planung“ unterdrückt auch Benachrichtigungen an der Aufgabe zugewiesene Personen und Mitglieder des Projekt-Teams. Der Empfang von Benachrichtigungen vor der Live-Schaltung des Projekts kann für die Beteiligten verwirrend sein.

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

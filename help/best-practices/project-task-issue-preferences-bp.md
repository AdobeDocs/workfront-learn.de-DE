---
title: Best Practice - Voreinstellungen für Projekte, Aufgaben und Probleme
description: Erfahren Sie mehr über Best Practices-Empfehlungen von Adobe Workfront-Experten zur Einrichtung, Verwaltung und Verwendung von Workfront-Projekt-, Aufgaben- und Problemeinstellungen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Best Practice - Voreinstellungen für Projekte, Aufgaben und Probleme

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für Projekt-, Aufgaben- und Problemeinstellungen

* Setzen Sie den standardmäßigen Aufgabendauer-Typ auf &quot;Einfach&quot;.

* Legen Sie die Voreinstellung für den Status eines neuen Projekts auf &quot;Planung&quot;oder &quot;Idee&quot;fest, nicht auf &quot;Aktuell&quot;.

* Aktivieren Sie in den globalen Projekteigenschaften die Option Grundlinien automatisch erstellen .

* Überprüfen Sie alle Optionen im Abschnitt Geschäftsfälle der Systemprojektvoreinstellungen.

* Aktivieren Sie in den Voreinstellungen für Probleme die Option Status &quot;Gelöstes Problem automatisch aktualisieren&quot;, wenn sich der Status des aufgelösten Objekts ändert.

</br>
</br>


## Warum sind diese Best Practices?

**Best Practice**

Setzen Sie den standardmäßigen Aufgabendauer-Typ auf &quot;Einfach&quot;.

**Deshalb**

Die Dauer der Aufgabe, die geplanten Stunden und die Anzahl der der Aufgabe zugewiesenen Personen werden durch die Typen der Dauer der Aufgabe bestimmt.

Mit Einfach als globaler Systemstandard haben alle manuell erstellten Aufgaben diesen Dauertyp. Geplante Stunden werden gleichmäßig auf die zugewiesenen Aufgaben über die Dauer verteilt. Der Typ Einfache Dauer kann die Projektplanung vereinfachen, da er es Ihnen ermöglicht, Änderungen an den Aufgabenverantwortlichen und geplanten Stunden vorzunehmen, ohne die Dauer der Aufgabe, das geplante Startdatum oder das geplante Abschlussdatum zu beeinträchtigen.

</br>
</br>

**Best Practice**

Legen Sie die Voreinstellung für den Status eines neuen Projekts auf &quot;Planung&quot;oder &quot;Idee&quot;fest, nicht auf &quot;Aktuell&quot;.

**Deshalb**

Der Status &quot;Aktuell&quot;zeigt an, dass ein Projekt live ist und aktiv daran gearbeitet wird. Es kommt selten vor, dass ein Projekt bei seiner Erstellung diesen Status aufweisen muss. Selbst wenn Sie eine Projektvorlage verwenden, ist eine gewisse &quot;Planung&quot;erforderlich, um Aufgabenzuweisungen zu erhalten, das geplante Abschlussdatum des Projekts anzupassen usw. Der Planungsstatus unterdrückt auch Benachrichtigungen an Aufgabenverantwortliche und Projektteams. Der Empfang von Benachrichtigungen vor der Live-Schaltung des Projekts kann für die Beteiligten verwirrend sein.

</br>
</br>

**Best Practice**

Aktivieren Sie in den globalen Projekteigenschaften die Option Grundlinien automatisch erstellen .

**Deshalb**

Jedes Mal, wenn Sie einen Projektstatus in Aktuell ändern, zeichnet Workfront automatisch eine Projektgrundlinie auf. Diese &quot;Momentaufnahme&quot;des Projekts liefert historische Informationen darüber, wie sich der Plan des Projekts im Laufe der Zeit verändert hat. Sie können beispielsweise den ursprünglichen Projektplan mit dem aktuellen Plan vergleichen, wenn Sie zeigen, wie sich verändernde Prioritäten oder der Umfang auf die Projekttermine auswirkten.

</br>
</br>

**Best Practice**

Überprüfen Sie alle Optionen im Abschnitt Geschäftsfälle der Systemprojektvoreinstellungen.

**Deshalb**

Aktivieren Sie alle fünf Optionen, damit Projektmanager, Planer und andere diese Abschnitte in den Geschäftsfall eines Projekts einbeziehen können. Wenn die Optionen nicht aktiviert sind, werden sie nicht im Geschäftsfallfenster angezeigt. Benutzer können jedes Feld leer lassen, wenn es für dieses Projekt nicht benötigt wird, sie können jedoch kein Feld auf Projektebene aktivieren. Diese Optionen können nur global im Setup aktiviert werden.

</br>
</br>

**Best Practice**

Aktivieren Sie in den Voreinstellungen für Probleme die Option Status &quot;Gelöstes Problem automatisch aktualisieren&quot;, wenn sich der Status des aufgelösten Objekts ändert.

**Deshalb**

Wenn ein Problem in ein Projekt konvertiert wird, verknüpft diese Voreinstellung die Status der beiden Elemente. Durch die Aktualisierung des Projektstatus (das auflösende Objekt) wird der Problemstatus automatisch aktualisiert. Das bedeutet, dass der Anfragende den Fortschritt bei seiner Anfrage sehen kann, selbst wenn er nicht über die Berechtigung zum Anzeigen des gesamten Projekts in Workfront verfügt.

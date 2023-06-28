---
title: Best Practice - Status
description: Erfahren Sie mehr über Best Practices von Adobe Workfront-Experten zur Einrichtung, Verwaltung und Verwendung von Workfront-Status.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Best Practice - Status

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für Status

* Behalten Sie beim Umbenennen der Standardstatus von Workfront den ursprünglichen Zweck des Status bei.

* Wenn Sie einen benutzerdefinierten Projektstatus für Abgebrochen erstellen, müssen Sie den Status mit &quot;Dead&quot;gleichsetzen.

* Halten Sie globale benutzerdefinierte Status auf ein Minimum beschränkt.

* Verwenden Sie keinen Projektstatus anstelle von Aufgaben, um den Fortschritt eines Projekts anzuzeigen.


</br>
</br>



## Warum sind diese Best Practices?

**Best Practice**

Behalten Sie beim Umbenennen der Standardstatus von Workfront den ursprünglichen Zweck des Status bei.



**Deshalb**

Einige Aktionen in Workfront werden durch den Standardstatus des Systems ausgelöst. Eine Änderung des Statusabsichten kann sich auf das Verhalten von Workfront in bestimmten Situationen, auf die Berichterstellung usw. auswirken.



Beispielsweise teilt Workfront mit dem standardmäßigen Aufgabenstatus Complete mit, dass der prozentuale Abschluss einer Aufgabe auf 100 % geändert werden soll. Der Status Fertig stellen informiert Workfront auch darüber, dass die Arbeit an abhängigen Aufgaben beginnen kann. Wenn Sie den Namen des Status in Warten geändert haben, um anzugeben, dass die Bearbeitung einer Aufgabe ausgesetzt ist, wird Workfront glauben, dass die Aufgabe abgeschlossen ist, und die nächsten Schritte im Projekt starten.

</br>
</br>



**Best Practice**

Wenn Sie einen benutzerdefinierten Projektstatus für Abgebrochen erstellen, müssen Sie den Status mit &quot;Dead&quot;gleichsetzen.



**Deshalb**

Wenn Sie Abgebrochen mit Abgeschlossen gleicht, können Sie den Status nicht zum Abbrechen eines Projekts verwenden, es sei denn, alle Aufgaben sind als abgeschlossen markiert und alle Probleme werden geschlossen. Wenn Sie Abgebrochen mit Tod gleichsetzen, können Sie das Projekt abbrechen, ohne etwas im historischen Datensatz zu ändern.


</br>
</br>

**Best Practice**

Halten Sie globale benutzerdefinierte Status auf ein Minimum beschränkt.



**Deshalb**

Weniger ist mehr. Neben unnötiger Wartung schaffen zu viele benutzerdefinierte Status Verwirrung, insbesondere bei der Arbeit an funktionsübergreifenden Projekten. Nehmen Sie stattdessen benutzerspezifische Status gruppenspezifisch vor. Dadurch wird Ihre Workfront-Umgebung sauberer und für die zukünftige Erweiterung auf andere Gruppen besser positioniert. Arbeiten Sie mit Ihrem Governance-/Aufsichtsausschuss und den Interessengruppen zusammen, um die Status zu ermitteln, die die Gruppen Ihres Unternehmens benötigen.


</br>
</br>

**Best Practice**

Verwenden Sie keinen Projektstatus anstelle von Aufgaben, um den Fortschritt eines Projekts anzuzeigen.



**Deshalb**

Halten Sie den Projektstatus einfach, um allgemeine Phasen des Fortschritts wie Planung, Aktuell, Abgeschlossen usw. anzugeben. Lassen Sie die Aufgaben, den Aufgabenstatus und den Aufgabenprozentsatz abschließen und erfahren, wie die Arbeit insgesamt im Projekt vorankommt. Diese Indikatoren auf Aufgabenebene werden in den Prozentsatz des Projektabschlusses, die Projektbedingung und den Projektfortschrittsstatus einfließen, die alle bessere und genauere Indikatoren für den Projektfortschritt als ein Projektstatus sind. Darüber hinaus bieten diese Informationen auf Aufgabenebene eine bessere Berichterstellung für Projekte.

---
title: Best Practice - Planung und Verwaltung von Zeitplänen
description: Erfahren Sie mehr über Best Practices-Empfehlungen von Adobe Workfront-Experten zur Einrichtung, Verwaltung und Verwendung von Projektzeitplänen in Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
kt: 10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Best Practice - Planung und Verwaltung von Zeitplänen

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für die Planung und Verwaltung von Zeitplänen

* Alle abgeschlossenen Projekte sollten einen Status aufweisen, der angibt, dass sie abgeschlossen sind.

* Legen Sie beim Kopieren eines Projekts den Status des neuen Projekts auf &quot;Planung&quot;fest.

* Lassen Sie Benutzer die tatsächliche Besuchszeit für Aufgaben aufzeichnen, damit Sie die tatsächlichen Stunden mit den geplanten Stunden vergleichen können.

* Verwenden Sie nach Möglichkeit Aufgabendauer und -versionen, um eine Projekt-Timeline zu erstellen und zu aktualisieren, anstatt spezifische Start- und Abschlussdaten auszuwählen.

* Bitten Sie die Benutzer, ihren Aufgabenstatus, den Prozentsatz der Abschlüsse und die tatsächlichen Stunden jeden Tag (oder wöchentlich einen festgelegten Zeitplan) zu aktualisieren.

* Stellen Sie den Projektstatus bei der Aktualisierung des Projektplans auf Planung ein, um zu verhindern, dass Benachrichtigungen automatisch gesendet werden, wenn Änderungen vorgenommen werden.

* Entfernen Sie Benutzer aus dem Projektteam, denen keine Arbeit im Projekt zugewiesen wurde.

* Platzieren Sie Projektmetriken oben im linken Bedienfeldmenü für Benutzer, die hauptsächlich Workfront verwenden, um Daten anzuzeigen.


</br>
</br>


## Warum sind diese Best Practices?

**Best Practice**

Alle abgeschlossenen Projekte sollten einen Status aufweisen, der angibt, dass sie abgeschlossen sind.


**Deshalb**

Wenn Sie sicherstellen, dass alle abgeschlossenen Projekte den Status Abgeschlossen (oder gleichwertig) haben, bleibt Ihre Workfront-Instanz sauber und aktuell. Indem Sie den Projektstatus auf dem neuesten Stand halten und abschließen, können Benutzer leicht feststellen, welche Arbeit bereits durchgeführt wurde, sodass sie sich auf aktive Prioritäten konzentrieren können. Außerdem wird sichergestellt, dass Berichtsdaten zu Projekten, Aufgaben, Ressourcen usw. korrekt sind.


</br>
</br>

**Best Practice**

Legen Sie beim Kopieren eines Projekts den Status des neuen Projekts auf &quot;Planung&quot;fest.

**Deshalb**

Der Planungsstatus (oder ein entsprechender Status) verhindert, dass Workfront-Benachrichtigungen zu Zuweisungen, Timeline-Änderungen usw. gesendet werden, bevor das Projekt fertig ist. Beim Kopieren eines Projekts wird ein Dialogfeld mit Projektoptionen angezeigt. Ändern Sie hier den Status und passen Sie andere Optionen an, damit keine Daten aus dem Originalprojekt in die kopierte Version kopiert werden.

</br>
</br>

**Best Practice**

Lassen Sie Benutzer die tatsächliche Besuchszeit für Aufgaben aufzeichnen, damit Sie die tatsächlichen Stunden mit den geplanten Stunden vergleichen können.


**Deshalb**

Wenn Sie wissen, wie lange die Arbeit dauert, können Sie Projektvorlagen aktualisieren, um zukünftige Projekte genauer zu planen. Das bedeutet auch, dass Ressourcenschätzungen mithilfe der Ressourcen-Management-Tools von Workfront genauer sind.

</br>
</br>

**Best Practice**

Verwenden Sie nach Möglichkeit Aufgabendauer und -versionen, um eine Projekt-Timeline zu erstellen und zu aktualisieren, anstatt spezifische Start- und Abschlussdaten auszuwählen.

**Deshalb**

Die Verwendung von Dauern und Vorgängern in Verbindung mit flexiblen Aufgabenbeschränkungen (so bald wie möglich und so spät wie möglich) ermöglicht automatische Zeitleistenänderungen, die durch den Projektplan &quot;kaskadiert&quot;werden. Wenn beispielsweise die Dauer einer Aufgabe um einen Tag erhöht wird, ändert dies das geplante Abschlussdatum der Aufgabe, das wiederum die Abschlussdaten der folgenden Aufgaben ändert.

Wenn Sie bestimmte Start- und Enddaten für Aufgaben auswählen, wird die Aufgabenbegrenzung zu einem Datum geändert, das das Datum &quot;sperrt&quot;(Must Start On, Must Finish On, Fixed Dates), d. h., Sie müssen manuell Aktualisierungen des Zeitleistensatzes vornehmen.

</br>
</br>


**Best Practice**

Bitten Sie die Benutzer, ihren Aufgabenstatus, den Prozentsatz der Abschlüsse und die tatsächlichen Stunden jeden Tag (oder wöchentlich einen festgelegten Zeitplan) zu aktualisieren.

**Deshalb**

Berichte in Workfront sind nur so genau wie die in Workfront eingegebenen Daten. Wenn Informationen, die auf den Fortschritt der Arbeit hinweisen (z. B. Status und prozentualer Abschluss), nicht regelmäßig aktualisiert werden, sind Berichte, die den Fortschritt der Arbeit anzeigen, nicht korrekt. Die tägliche Aktualisierung sorgt für die größte Genauigkeit der Echtzeitberichtsdaten.


Der Aufgabenstatus wird auch verwendet, um den Benutzern mitzuteilen, wann die frühere Arbeit abgeschlossen ist und ihre neuen Aufgaben beginnen können. Wenn der Aufgabenstatus nicht geändert wird, um den tatsächlichen Fortschritt am Arbeitselement widerzuspiegeln, kann Workfront die entsprechenden Benachrichtigungen nicht versenden.

</br>
</br>

**Best Practice**

Stellen Sie den Projektstatus bei der Aktualisierung des Projektplans auf Planung ein, um zu verhindern, dass Benachrichtigungen automatisch gesendet werden, wenn Änderungen vorgenommen werden.

**Deshalb**

Projektplanänderungen können mehrere Benachrichtigungen generieren, wenn Aufgabenzuweisungen, geplante Start- und Abschlussdaten und andere Einstellungen geändert werden. Dies kann für Benutzer störend sein und zu Verwirrung bei ordnungsgemäßen Zuweisungen, Terminen usw. führen.

Der Planungsstatus gibt an, dass Workfront keine Benachrichtigungen über das Projekt an Mitglieder des Projektteams (Benutzer, denen Aufgaben/Probleme zugewiesen wurden, oder andere mit Zugriff auf das Projekt) senden soll, da der Projektplan noch entwickelt wird oder das Projekt noch nicht verfügbar ist. Sobald die Änderungen abgeschlossen sind, ändern Sie den Projektstatus zurück in Aktuell und Benachrichtigungen werden gesendet. Auf diese Weise können Sie die Anzahl der Benachrichtigungen, die Benutzer erhalten, minimieren.

</br>
</br>

**Best Practice**

Entfernen Sie Benutzer aus dem Projektteam, denen keine Arbeit im Projekt zugewiesen wurde.


**Deshalb**

Wenn Sie einer Person eine Aufgabe oder ein Problem in einem Projekt zuweisen, wird der Benutzer in den Abschnitten Planung und Personen des Projekts zur Projektteams-Liste hinzugefügt. Sie bleiben jedoch auch dann auf der Liste der Projektteams, wenn Sie sie aus der Zuweisung entfernt haben. Dies kann für den Benutzer zu Verwirrung führen, da er als Teil des Projektteams Benachrichtigungen über die Aktivität im Projekt erhält und das Projekt in der Liste &quot;Projekte, bei denen ich auf der Liste bin&quot;anzeigt.


Darüber hinaus erhalten die Mitglieder des Projektteams Berechtigungen für das Projekt und seine Aufgaben, Probleme und Dokumente. Dies kann dazu führen, dass Benutzer Zugriff auf Artikel in Workfront haben, die sie nicht benötigen oder nicht haben sollten.

</br>
</br>

**Best Practice**

Platzieren Sie Projektmetriken oben im linken Bedienfeldmenü für Benutzer, die hauptsächlich Workfront verwenden, um Daten anzuzeigen.

**Deshalb**

Die meisten Führungskräfte, Führungskräfte und andere Benutzer, die keine Projekte verwalten oder Aufgabenzuweisungen erfüllen, würden es begrüßen, wenn sie diese Ebene von Projektmetriken beim ersten Öffnen eines Projekts sehen würden. Verwenden Sie eine Layoutvorlage, um Projektmetriken im linken Fenstermenü auf einer Projektseite nach oben zu verschieben, damit sie für Benutzer leichter sichtbar und leichter zugänglich sind.

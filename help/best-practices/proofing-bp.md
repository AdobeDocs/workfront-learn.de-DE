---
title: Best Practice - Testversand
description: Erfahren Sie mehr über Best Practices von Adobe Workfront-Experten für die Einrichtung, Verwaltung und Verwendung von Testsendungen in Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Best Practice - Testversand

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Leitlinien, die einen wirksamen und effizienten Handlungsweg darstellen. leicht von Ihnen und den Benutzern in Ihrem Unternehmen übernommen werden; und können in Ihrem gesamten Unternehmen erfolgreich repliziert werden.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für die Überprüfung in Workfront

* Erstellen Sie Workflow-Vorlagen für Testsendungen.

* Deaktivieren Sie in den Workfront-Setups die Einstellung &quot;E-Mails von Workfront senden, wenn ein Kommentar zu einem Testversand abgegeben wird&quot;.

* Verwenden Sie die Einstellung &quot;Benutzerrollen für Nicht-Empfänger, die einen Dokumentversand öffnen&quot;in Workfront nur &quot;Schreibgeschützt&quot;oder &quot;Überprüfer&quot;.

* Passen Sie die Back-End-Einstellungen für den Testversand an, damit Benutzer Termine im 12-Stunden-Uhrzeitformat sehen.

* Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Testversand-Deadline fest.

* Blenden Sie die Option Nicht relevante Testversandentscheidung aus.

* Ordnen Sie die Testversand-Entscheidungsoptionen in den Testversandeinstellungen nicht neu an.

* Legen Sie Benutzerstandardeinstellungen für Testadressen und E-Mail-Warnungen fest.

* Setzen Sie die Testversand-Rolle des Testversands auf &quot;Überprüfer&quot;.

* Vermeiden Sie die Verwendung der Rolle &quot;Testversand genehmigen&quot;.

* Vermeiden Sie die Option E-Mail-Warnhinweis mit Aktivitätsnachweis .

</br>
</br>

## Warum sind diese Best Practices?

**Best Practice**

Erstellen Sie Workflow-Vorlagen für Testsendungen.

**Deshalb**

Vorlagen beschleunigen und optimieren nicht nur die Erstellung und Zuweisung von Testsendungen, sondern bieten auch Konsistenz über Testversand-Workflows hinweg für ähnliche Asset-Typen. Sie stellen außerdem sicher, dass jedem Testversand-Empfänger die richtige Testversandrolle und die richtige E-Mail-Warnung zugewiesen wird und dass ein Termin festgelegt wurde.

</br>
</br>

**Best Practice**

Deaktivieren Sie in den Workfront-Setups die Einstellung &quot;E-Mails von Workfront senden, wenn ein Kommentar zu einem Testversand abgegeben wird&quot;.



**Deshalb**

Wenn diese Einstellung aktiviert ist (standardmäßig), können Benutzer mehrere E-Mail-Benachrichtigungen für jeden Kommentar auf einem Testversand erhalten - eine von der Testfunktion und eine von Workfront selbst. Diese doppelten Benachrichtigungen führen zu einer Unterbrechung und Verwirrung der E-Mail-Benachrichtigung sowie zu einem vollständigen E-Mail-Posteingang, was letztendlich dazu führen kann, dass Benutzer die von ihnen empfangenen Testversandbenachrichtigungen ignorieren. Dies wiederum könnte verpasste Fristen bedeuten.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü > Einrichtung > E-Mail > Überprüfen und Genehmigen .

</br>
</br>

**Best Practice**

Verwenden Sie die Einstellung &quot;Benutzerrollen für Nicht-Empfänger, die einen Dokumentversand öffnen&quot;in Workfront nur &quot;Schreibgeschützt&quot;oder &quot;Überprüfer&quot;.



**Deshalb**

Für die anderen Optionen dieser Einstellung muss eine Testversandentscheidung getroffen werden, durch die Ihr Testversand-Workflow entgleitet werden kann. Im Allgemeinen müssen Personen, die nicht zum Testversand-Workflow hinzugefügt werden, lediglich den Testversand ansehen oder Kommentare abgeben, den Testversand nicht validieren. Daher sind die Optionen Schreibgeschützt oder Prüfer Ihre beste Wahl.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü > Einrichtung > Überprüfen und Genehmigen .

</br>
</br>

**Best Practice**

Passen Sie die Back-End-Einstellungen für den Testversand an, damit Benutzer Termine im 12-Stunden-Uhrzeitformat sehen.



**Deshalb**

Wählen Sie die Option F j, Y, gi:a in den Testversandeinstellungen für Benutzer aus, die die Testversandfristen/-zeiten im AM/PM-Format sehen möchten. Für Bereiche, die eine 12-Stunden-Uhr verwenden, hilft dies bei der Klarheit der Termine.



**Hinweis**: Diese Einstellung können Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Benutzer > vornehmen und für jeden Benutzer das Feld Datumsformat bearbeiten.

</br>
</br>

**Best Practice**

Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Testversand-Deadline fest.



**Deshalb**

Wenn der Ersteller eines Testversands vergisst, einen Termin hinzuzufügen, wendet Workfront diesen Termin automatisch auf jeden hochgeladenen Testversand an.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Einstellungen > Testversand-Standard > Versandgültigkeit (+ Geschäftstage) .

</br>
</br>


**Best Practice**

Blenden Sie die Option Nicht relevante Testversandentscheidung aus.



**Deshalb**

Diese Entscheidungsoption führt bei Genehmigern häufig zu Verwirrung, da Organisationen häufig nicht definieren, wann die Option Nicht relevant verwendet werden soll. Die Option Nicht relevant weist im Allgemeinen darauf hin, dass der Testversand für den Testversand-Empfänger nicht relevant ist und dass er keine genehmigte oder abgelehnte Entscheidung treffen muss. Durch die Auswahl von Nicht relevant kann der Testversand-Workflow fortgesetzt werden.


Die Option Nicht relevant ist in den meisten Testversand-Workflows nicht erforderlich.

**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Entscheidungen.

</br>
</br>

**Best Practice**

Ordnen Sie die Testversand-Entscheidungsoptionen in den Testversandeinstellungen nicht neu an.



**Deshalb**

Jede Einstellung der Testversandentscheidung enthält einen bestimmten Wert/eine bestimmte Gewichtung, die bei einer Neuanordnung Verwirrung in Ihren Testversandkonfigurationen verursachen kann. Die Entscheidungsreihenfolge und der Wert/die Gewichtung werden als Trigger für die Aktivierung der Testphase und in Berichten verwendet.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Entscheidungen.

</br>
</br>

**Best Practice**

Legen Sie Benutzerstandardeinstellungen für Testadressen und E-Mail-Warnungen fest.



**Deshalb**

Diese Einstellungen werden automatisch ausgefüllt, wenn Sie einen Testversand-Workflow zuweisen, den Prozess beschleunigen und zur Konsistenz der Testversand-Workflows beitragen.



**Hinweis**: Die Standardeinstellungen der Benutzer werden im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Benutzer > angezeigt. Wählen Sie dann den Benutzer aus, für den die Standardeinstellungen festgelegt werden sollen.

</br>
</br>

**Best Practice**

Setzen Sie die Testversand-Rolle des Testversands auf &quot;Überprüfer&quot;.



**Deshalb**

Mit der Rolle Testversand überprüfen wird sichergestellt, dass der Ersteller des Testversands Kommentare abgeben und auf Kommentare zugreifen kann, die von anderen Benutzern hinterlassen wurden. Meistens muss der Ersteller des Testversands keine Entscheidung über einen hochgeladenen Testversand treffen. Die Rollen Genehmiger, Prüfer und Genehmiger, Autor oder Moderator-Testversand erfordern eine Entscheidung. Wenn dem Ersteller des Testversands eine dieser Rollen zugewiesen wird, er jedoch nie eine Entscheidung trifft, kann dies die Testversandfristen beeinträchtigen.

</br>
</br>

**Best Practice**

Vermeiden Sie die Verwendung der Rolle &quot;Testversand genehmigen&quot;.



**Deshalb**

Die Rolle &quot;Testversand genehmigen&quot;ermöglicht dem Benutzer keine Kommentare zu diesem Testversand. Dies könnte dazu führen, dass ein Benutzer den Testversand ohne jegliche Erklärung ablehnt, da er keine Kommentare abgeben konnte. Verwenden Sie stattdessen die Rolle &quot;Testversand für Prüfer und Genehmiger&quot;, damit der Benutzer Feedback geben kann.

</br>
</br>

**Best Practice**

Vermeiden Sie die Option E-Mail-Warnhinweis mit Aktivitätsnachweis .

**Deshalb**

Diese Option sendet eine E-Mail-Benachrichtigung zu jedem Fall, in dem ein Testversand durchgeführt wird - ein Kommentar, eine Antwort, eine Entscheidung usw. Der Empfänger sieht im Wesentlichen die Aktivität Testversand , sobald dies geschieht.

Für Testversand-Eigentümer und -Ersteller funktioniert der Benachrichtigungs-E-Mail-Warnhinweis &quot;Entscheidungen&quot;am besten für mehrstufige Testsendungen und die endgültige Entscheidung funktioniert am besten für einstufige Workflows. Im Allgemeinen können alle anderen auf Deaktiviert gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare oder Entscheidungen treffen (in diesem Fall kann eine der Zusammenfassungs-E-Mail-Optionen am besten funktionieren).

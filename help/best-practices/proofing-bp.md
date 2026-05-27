---
title: Best Practice – Proofing
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden der Proofing-Funktion in Workfront empfehlen.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
last-substantial-update: 2024-11-06T00:00:00.000Z
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
TQID: https://experienceleague.adobe.com/GB0kExlH19phGvui4KUhtsrOk-U2mPGnSrXf-5PerpQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 1198
ht-degree: 96%

---

# Best Practice – Proofing

## Was ist eine „Best Practice“ für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des „Warum“ vertraut zu machen.

Die Frage „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

</br>
</br>

## Best Practices für das Proofing in Workfront

* Nehmen Sie sich die Zeit, um Vorlagen für Proofing-Workflows zu erstellen.

* Deaktivieren Sie im Workfront-Setup die Einstellung „E-Mails von Workfront senden, wenn ein Proof kommentiert wird“.

* Legen Sie in Workfront die Einstellung „Benutzerrollen für Nicht-Empfänger, die einen Dokument-Korrekturabzug öffnen“ auf „Schreibgeschützt“ oder „Prüfer“ fest.

* Passen Sie die Backend-Einstellungen für den Korrekturabzug an, damit Benutzende Fristen im 12-Stunden-Zeitformat sehen können.

* Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Frist für den Korrekturabzug fest.

* Blenden Sie die Korrekturabzugsentscheidungs-Option „Nicht relevant“ aus.

* Ordnen Sie die Optionen für die Korrekturabzugsentscheidung in den Korrekturabzugseinstellungen nicht neu an.

* Legen Sie Benutzerstandardeinstellungen für Korrekturabzugsrollen und E-Mail-Warnhinweise fest.

* Setzen Sie die Korrekturabzugsrolle der Person, die den Korrekturabzug erstellt hat, auf „Prüfer“.

* Vermeiden Sie es, die Korrekturabzugsrolle „Genehmigende Person“ zu verwenden.

* Vermeiden Sie die Korrekturabzugs-E-Mail-Warnoption „Alle Aktivitäten“.

</br>
</br>

## Warum sind das Best Practices?

**Best Practice**

Nehmen Sie sich die Zeit, um Vorlagen für Proofing-Workflows zu erstellen.

**Das sind die Gründe**

Vorlagen beschleunigen und optimieren nicht nur die Erstellung und Zuweisung von Korrekturabzügen, sondern bieten für ähnliche Asset-Typen auch eine Konsistenz über Korrekturabzug-Workflows hinweg. Sie stellen außerdem sicher, dass allen Empfängerinnen und Empfängern von Korrekturabzügen die richtige Korrekturabzugsrolle und der richtige E-Mail-Warnhinweis zugewiesen werden und dass eine Frist festgelegt wurde.

</br>
</br>

**Best Practice**

Deaktivieren Sie im Workfront-Setup die Einstellung „E-Mails von Workfront senden, wenn ein Proof kommentiert wird“.



**Das sind die Gründe**

Wenn diese Einstellung aktiviert ist (dies ist standardmäßig der Fall), können Benutzende mehrere E-Mail-Benachrichtigungen für jeden Kommentar zu einem Korrekturabzug erhalten – eine von der Proofing-Funktion und eine von Workfront selbst. Diese doppelten Benachrichtigungen führen zu Störungen und Verwirrung in Bezug auf die E-Mail-Benachrichtigungen sowie zu einem vollen E-Mail-Posteingang. Dies kann letztendlich die Folge haben, dass Benutzende die von ihnen empfangenen Benachrichtigungen über Korrekturabzüge ignorieren. Dadurch können wiederum Fristen verpasst werden.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Setup“ > „E-Mail“ > „Überprüfung und Genehmigung“.

</br>
</br>

**Best Practice**

Legen Sie in Workfront die Einstellung „Benutzerrollen für Nicht-Empfänger, die einen Dokument-Korrekturabzug öffnen“ auf „Schreibgeschützt“ oder „Prüfer“ fest.



**Das sind die Gründe**

Für die anderen Optionen dieser Einstellung muss eine Korrekturabzugsentscheidung getroffen werden, durch die Ihr Proofing-Workflow scheitern kann. Im Allgemeinen müssen Personen, die nicht zum Korrekturabzug-Workflow hinzugefügt werden, lediglich den Korrekturabzug ansehen oder Kommentare abgeben, den Korrekturabzug aber nicht tatsächlich genehmigen. Daher wählen Sie am besten die Optionen „Schreibgeschützt“ oder „Prüfer“ aus.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Setup“ > „Überprüfung und Genehmigung“.

</br>
</br>

**Best Practice**

Passen Sie die Backend-Einstellungen für den Korrekturabzug an, damit Benutzende Fristen im 12-Stunden-Zeitformat sehen können.



**Das sind die Gründe**

Standardmäßig ist ein 24-Stunden-Zeitformat eingerichtet. Dies kann für Personen verwirrend sein, die nicht damit vertraut sind. Ändern Sie das Format, indem Sie im Workfront-Hauptmenü die Option „Proofing“ > „Kontoeinstellungen“ > „Benutzende“ auswählen. Doppelklicken Sie auf einen Benutzernamen, um ihn auszuwählen, und bearbeiten Sie im Abschnitt „Persönliche Einstellungen“ das Feld „Datumsformat“. Sie müssen jeden Benutzernamen einzeln auswählen, um Änderungen vorzunehmen.

</br>
</br>

**Best Practice**

Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Frist für den Korrekturabzug fest.



**Das sind die Gründe**

Wenn eine standardmäßige Korrekturabzugsfrist – Hochladedatum + x Anzahl von Werktagen – festgelegt ist und die Person, die den Korrekturabzug erstellt hat, vergisst, eine Frist hinzuzufügen, wendet Workfront diese Frist automatisch auf jeden hochgeladenen Korrekturabzug an.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Einstellungen“ > „Korrrekturabzugs-Standardeinstellungen“ im Feld „Frist (+ Werktage)“.

</br>
</br>


**Best Practice**

Blenden Sie die Korrekturabzugsentscheidungs-Option „Nicht relevant“ aus.



**Das sind die Gründe**

Diese Entscheidungsoption führt bei genehmigenden Personen häufig zu Verwirrung, da Organisationen oft nicht definieren, wann die Option „Nicht relevant“ verwendet werden soll. Die Option „Nicht relevant“ weist im Allgemeinen darauf hin, dass der Korrekturabzug für die Empfängerin oder den Empfänger des Korrekturabzugs nicht relevant ist und dass diese Person keine Genehmigungs- oder Ablehnungsentscheidung treffen muss. Durch die Auswahl von „Nicht relevant“ kann der Korrekturabzug-Workflow fortgesetzt werden.


Die Option „Nicht relevant“ ist in den meisten Korrekturabzug-Workflows nicht erforderlich.

**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“.

</br>
</br>

**Best Practice**

Ordnen Sie die Optionen für die Korrekturabzugsentscheidung in den Korrekturabzugseinstellungen nicht neu an.



**Das sind die Gründe**

Jede Einstellung für die Korrekturabzugsentscheidung umfasst einen bestimmten Wert bzw. eine bestimmte Gewichtung, was bei einer Neuanordnung in Bezug auf Ihre Korrekturabzugskonfigurationen zu Verwirrung führen kann. Die Entscheidungsreihenfolge und der Wert/die Gewichtung werden als Trigger für die Aktivierung der Korrekturphase und beim Reporting verwendet.



**Hinweis**: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“.

</br>
</br>

**Best Practice**

Legen Sie Benutzerstandardeinstellungen für Korrekturabzugsrollen und E-Mail-Warnhinweise fest.



**Das sind die Gründe**

Diese Einstellungen werden automatisch angegeben, wenn Sie einen Korrekturabzug-Workflow zuweisen. Auf diese Weise wird der Vorgang beschleunigt und trägt zur Konsistenz der Korrekturabzug-Workflows bei.



**Hinweis**: Die Standardeinstellungen für Benutzende finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Benutzer“. Wählen Sie dann die Person aus, für die die Standardeinstellungen festgelegt werden sollen.

</br>
</br>

**Best Practice**

Setzen Sie die Korrekturabzugsrolle der Person, die den Korrekturabzug erstellt hat, auf „Prüfer“.



**Das sind die Gründe**

Mit der Korrekturabzugsrolle „Prüfer“ wird sichergestellt, dass die Person, die den Korrekturabzug erstellt hat, Kommentare abgeben und auf Kommentare von anderen zugreifen kann. Meistens muss diese Person keine Entscheidung über einen hochgeladenen Korrekturabzug treffen. Von den Korrekturabzugsrollen „Genehmigende Person“, „Prüfer und genehmigende Person“, „Verfassende Person“ oder „Moderator“ wird jedoch eine Entscheidung verlangt. Wenn der Person, die den Korrekturabzug erstellt hat, eine dieser Korrekturabzugsrollen zugewiesen wird, aber sie nie eine Entscheidung trifft, kann dies die Korrekturabzugsfristen negativ beeinflussen.

</br>
</br>

**Best Practice**

Vermeiden Sie es, die Korrekturabzugsrolle „Genehmigende Person“ zu verwenden.



**Das sind die Gründe**

Mit der Korrekturabzugsrolle „Genehmigende Person“ können Benutzende keine Kommentare zu diesem Korrekturabzug abgeben. Dies könnte dazu führen, dass jemand den Korrekturabzug ohne jegliche Erklärung ablehnt, da es nicht möglich war, Kommentare abzugeben. Verwenden Sie stattdessen die Korrekturabzugsrolle „Prüfer und genehmigende Person“, damit die Person Feedback geben kann.

</br>
</br>

**Best Practice**

Vermeiden Sie die Korrekturabzugs-E-Mail-Warnoption „Alle Aktivitäten“.

**Das sind die Gründe**

Diese Option sendet jedes Mal eine E-Mail-Benachrichtigung zu einem Korrekturabzug, wenn etwas mit einem Korrekturabzug passiert - ein Kommentar wird abgegeben, eine Antwort wird veröffentlicht, eine Entscheidung getroffen wird usw. Der Empfänger sieht die Aktivität „Testversand“ praktisch sofort.

Für Inhaberinnen und Inhaber sowie Erstellerinnen und Ersteller eines Korrekturabzugs funktioniert der E-Mail-Warnhinweis „Entscheidungen“ am besten bei mehrstufigen Korrekturabzug-Workflows. „Finale Entscheidung“ ist wiederum am besten für einstufige Workflows geeignet. Im Allgemeinen können alle anderen auf „Deaktiviert“ gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare abgeben oder Entscheidungen treffen (in diesem Fall ist ggf. eine der Zusammenfassungs-E-Mail-Optionen am besten geeignet).

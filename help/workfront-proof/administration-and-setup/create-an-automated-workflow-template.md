---
title: Erstellen einer automatisierten Workflow-Vorlage
description: Erfahren Sie, wie Sie eine automatisierte Workflow-Vorlage erstellen, indem Sie Empfängerinnen bzw. Empfänger und Fristen für Korrekturabzüge festlegen. Geben Sie dann die Vorlage für andere Benutzende frei.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 56%

---

# Erstellen einer automatisierten Workflow-Vorlage

In diesem Video lernen Sie Folgendes:

* Erstellen einer automatischen Workflow-Vorlage für das Proofing in [!DNL  Workfront]
* Zuweisen von Empfängerinnen und Empfängern für Korrekturabzüge
* Festlegen einer Frist für den Prüf- und Genehmigungsvorgang
* Freigeben der automatisierten Workflow-Vorlage für andere

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Zusätzliche Optionen für die Stufenaktivierung

Es werden nur selten zwei Optionen verwendet, um zu bestimmen, wann ein Testversand-Workflow-Schritt gestartet werden soll: die [!UICONTROL Datum und Uhrzeit] und &quot;[!UICONTROL Wann der Termin für die vorherige Phase vergeht]&quot;.

Die zweite Option funktioniert nur in Szenarien, in denen eine große Gruppe von Personen eine Überprüfung durchführt und nicht auf alle warten möchte. Es ist eine Art &quot;Ich gebe Ihnen eine gewisse Zeit, um Ihre Überprüfung abzuschließen und dann verlieren Sie Ihre Chance&quot; Option. Aber selbst dies kann einen Überprüfungsprozess verlangsamen.

Wenn Sie &quot;[!UICONTROL wann der Termin der vorherigen Phase vergeht],&quot; ist es wichtig, sich daran zu erinnern, dass Sie eine Phase jederzeit manuell aktivieren können, wenn Sie nicht warten möchten, bis ein Termin erreicht ist.

## Best Practices

| Best Practice | Deshalb |
|---|---|
| Setzen Sie die Testversand-Rolle des Testversands auf &quot;Überprüfer&quot;. | Mit der Korrekturabzugsrolle „Prüfer“ wird sichergestellt, dass die Person, die den Korrekturabzug erstellt hat, Kommentare abgeben und auf Kommentare von anderen zugreifen kann. Meistens muss der Ersteller des Testversands keine Entscheidung über einen hochgeladenen Testversand treffen. Von den Korrekturabzugsrollen „Genehmigende Person“, „Prüfer und genehmigende Person“, „Verfassende Person“ oder „Moderator“ wird jedoch eine Entscheidung verlangt. Wenn der Person, die den Korrekturabzug erstellt hat, eine dieser Korrekturabzugsrollen zugewiesen wird, aber sie nie eine Entscheidung trifft, kann dies die Korrekturabzugsfristen negativ beeinflussen. |
| Vermeiden Sie es, die Korrekturabzugsrolle „Genehmigende Person“ zu verwenden. | Mit der Korrekturabzugsrolle „Genehmigende Person“ können Benutzende keine Kommentare zu diesem Korrekturabzug abgeben. Dies könnte dazu führen, dass ein Benutzer den Testversand ohne jegliche Erklärung ablehnt, da er keine Kommentare abgeben konnte. Verwenden Sie stattdessen die Korrekturabzugsrolle „Prüfer und genehmigende Person“, damit die Person Feedback geben kann. |
| Vermeiden Sie die Korrekturabzugs-E-Mail-Warnoption „Alle Aktivitäten“. | Mit dieser Option wird bei jedem Vorgang im Zusammenhang mit dem Korrekturabzug eine E-Mail-Benachrichtigung gesendet – also bei jedem Kommentar, jeder veröffentlichten Antwort, jeder Entscheidung usw. Die Empfängerin bzw. der Empfänger sieht im Grunde die Proofing-Aktivität in Echtzeit.<br><br>Für Testversand-Eigentümer und -Ersteller funktioniert der Benachrichtigungs-E-Mail-Warnhinweis &quot;Entscheidungen&quot;am besten für mehrstufige Testsendungen und die endgültige Entscheidung funktioniert am besten für einstufige Workflows. Im Allgemeinen können alle anderen auf „Deaktiviert“ gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare abgeben oder Entscheidungen treffen (in diesem Fall ist ggf. eine der Zusammenfassungs-E-Mail-Optionen am besten geeignet). |

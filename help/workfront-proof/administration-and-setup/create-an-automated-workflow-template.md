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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 100%

---

# Erstellen einer automatisierten Workflow-Vorlage

In diesem Video lernen Sie Folgendes:

* Erstellen einer automatischen Workflow-Vorlage für das Proofing in [!DNL  Workfront]
* Zuweisen von Empfängerinnen und Empfängern für Korrekturabzüge
* Festlegen einer Frist für den Prüf- und Genehmigungsvorgang
* Freigeben der automatisierten Workflow-Vorlage für andere

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops)

## Zusätzliche Optionen für die Stufenaktivierung

Zwei Optionen zur Bestimmung des Zeitpunkts, zu dem eine Stufe des Proofing-Workflows beginnen soll, werden selten verwendet, wenn überhaupt: die Option [!UICONTROL Datum und Uhrzeit] und die Option [!UICONTROL Nach Ablauf der Frist der vorherigen Stufe].

Die zweite Option eignet sich nur für Situationen, in denen eine große Gruppe von Personen eine Überprüfung durchführt und Sie nicht auf alle warten wollen. Diese Option besagt in etwa „Ich gebe dir eine bestimmte Zeit, um deine Bewertung zu vervollständigen, ansonsten verlierst du deine Chance“. Aber selbst dies kann einen Überprüfungsprozess verlangsamen.

Wenn Sie die Option [!UICONTROL Nach Ablauf der Frist der vorherigen Stufe] verwenden, sollten Sie daran denken, dass Sie eine Stufe jederzeit manuell aktivieren können, wenn Sie nicht auf den Ablauf einer Frist warten wollen.

## Best Practices

| Best Practice | Das sind die Gründe |
|---|---|
| Setzen Sie die Korrekturabzugsrolle der Person, die den Korrekturabzug erstellt hat, auf „Prüfer“. | Mit der Korrekturabzugsrolle „Prüfer“ wird sichergestellt, dass die Person, die den Korrekturabzug erstellt hat, Kommentare abgeben und auf Kommentare von anderen zugreifen kann. Meistens muss diese Person keine Entscheidung über einen hochgeladenen Korrekturabzug treffen. Von den Korrekturabzugsrollen „Genehmigende Person“, „Prüfer und genehmigende Person“, „Verfassende Person“ oder „Moderator“ wird jedoch eine Entscheidung verlangt. Wenn der Person, die den Korrekturabzug erstellt hat, eine dieser Korrekturabzugsrollen zugewiesen wird, aber sie nie eine Entscheidung trifft, kann dies die Korrekturabzugsfristen negativ beeinflussen. |
| Vermeiden Sie es, die Korrekturabzugsrolle „Genehmigende Person“ zu verwenden. | Mit der Korrekturabzugsrolle „Genehmigende Person“ können Benutzende keine Kommentare zu diesem Korrekturabzug abgeben. Dies könnte dazu führen, dass jemand den Korrekturabzug ohne jegliche Erklärung ablehnt, da es nicht möglich war, Kommentare abzugeben. Verwenden Sie stattdessen die Korrekturabzugsrolle „Prüfer und genehmigende Person“, damit die Person Feedback geben kann. |
| Vermeiden Sie die Korrekturabzugs-E-Mail-Warnoption „Alle Aktivitäten“. | Mit dieser Option wird bei jedem Vorgang im Zusammenhang mit dem Korrekturabzug eine E-Mail-Benachrichtigung gesendet – also bei jedem Kommentar, jeder veröffentlichten Antwort, jeder Entscheidung usw. Die Empfängerin bzw. der Empfänger sieht im Grunde die Proofing-Aktivität in Echtzeit.<br><br>Für Inhaberinnen und Inhaber sowie Erstellerinnen und Ersteller eines Korrekturabzugs funktioniert der E-Mail-Warnhinweis „Entscheidungen“ am besten bei mehrstufigen Korrekturabzug-Workflows. „Finale Entscheidung“ ist wiederum am besten für einstufige Workflows geeignet. Im Allgemeinen können alle anderen auf „Deaktiviert“ gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare abgeben oder Entscheidungen treffen (in diesem Fall ist ggf. eine der Zusammenfassungs-E-Mail-Optionen am besten geeignet). |

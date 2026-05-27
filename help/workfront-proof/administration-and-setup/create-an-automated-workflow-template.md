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
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:09:06.617Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 435
ht-degree: 91%

---

# Erstellen einer automatisierten Workflow-Vorlage

In diesem Video lernen Sie Folgendes:

* Erstellen einer automatischen Workflow-Vorlage für das Proofing in [!DNL &#x200B; Workfront]
* Zuweisen von Empfängerinnen und Empfängern für Korrekturabzüge
* Festlegen einer Frist für den Prüf- und Genehmigungsvorgang
* Freigeben der automatisierten Workflow-Vorlage für andere

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops=1)

## Zusätzliche Optionen für die Stufenaktivierung

Zwei Optionen zur Bestimmung des Zeitpunkts, zu dem eine Stufe des Proofing-Workflows beginnen soll, werden selten verwendet, wenn überhaupt: die Option [!UICONTROL Datum und Uhrzeit] und die Option [!UICONTROL Nach Ablauf der Frist der vorherigen Stufe].

Die zweite Option eignet sich nur für Situationen, in denen eine große Gruppe von Personen eine Überprüfung durchführt und Sie nicht auf alle warten wollen. Diese Option besagt in etwa „Ich gebe dir eine bestimmte Zeit, um deine Bewertung zu vervollständigen, ansonsten verlierst du deine Chance“. Aber selbst dies kann einen Überprüfungsprozess verlangsamen.

Wenn Sie die Option [!UICONTROL Nach Ablauf der Frist der vorherigen Stufe] verwenden, sollten Sie daran denken, dass Sie eine Stufe jederzeit manuell aktivieren können, wenn Sie nicht auf den Ablauf einer Frist warten wollen.

## Best Practices

| Best Practice | Das sind die Gründe |
|---|---|
| Setzen Sie die Korrekturabzugsrolle der Person, die den Korrekturabzug erstellt hat, auf „Prüfer“. | Mit der Korrekturabzugsrolle „Prüfer“ wird sichergestellt, dass die Person, die den Korrekturabzug erstellt hat, Kommentare abgeben und auf Kommentare von anderen zugreifen kann. Meistens muss diese Person keine Entscheidung über einen hochgeladenen Korrekturabzug treffen. Von den Korrekturabzugsrollen „Genehmigende Person“, „Prüfer und genehmigende Person“, „Verfassende Person“ oder „Moderator“ wird jedoch eine Entscheidung verlangt. Wenn der Person, die den Korrekturabzug erstellt hat, eine dieser Korrekturabzugsrollen zugewiesen wird, aber sie nie eine Entscheidung trifft, kann dies die Korrekturabzugsfristen negativ beeinflussen. |
| Vermeiden Sie es, die Korrekturabzugsrolle „Genehmigende Person“ zu verwenden. | Mit der Korrekturabzugsrolle „Genehmigende Person“ können Benutzende keine Kommentare zu diesem Korrekturabzug abgeben. Dies könnte dazu führen, dass jemand den Korrekturabzug ohne jegliche Erklärung ablehnt, da es nicht möglich war, Kommentare abzugeben. Verwenden Sie stattdessen die Korrekturabzugsrolle „Prüfer und genehmigende Person“, damit die Person Feedback geben kann. |
| Vermeiden Sie die Korrekturabzugs-E-Mail-Warnoption „Alle Aktivitäten“. | Diese Option sendet jedes Mal eine E-Mail-Benachrichtigung zu einem Korrekturabzug, wenn etwas mit einem Korrekturabzug passiert - ein Kommentar wird abgegeben, eine Antwort wird veröffentlicht, eine Entscheidung getroffen wird usw. Der Empfänger sieht die Aktivität „Testversand“ praktisch sofort.<br><br>Für Inhaberinnen und Inhaber sowie Erstellerinnen und Ersteller eines Korrekturabzugs funktioniert der E-Mail-Warnhinweis „Entscheidungen“ am besten bei mehrstufigen Korrekturabzug-Workflows. „Finale Entscheidung“ ist wiederum am besten für einstufige Workflows geeignet. Im Allgemeinen können alle anderen auf „Deaktiviert“ gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare abgeben oder Entscheidungen treffen (in diesem Fall ist ggf. eine der Zusammenfassungs-E-Mail-Optionen am besten geeignet). |

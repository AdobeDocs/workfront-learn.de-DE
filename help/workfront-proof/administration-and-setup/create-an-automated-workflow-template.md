---
title: Automatisierte Workflow-Vorlage erstellen
description: Erfahren Sie, wie Sie eine automatisierte Workflow-Vorlage erstellen, indem Sie Testversand-Empfänger zuweisen und Testversandfristen festlegen. Geben Sie dann die Vorlage für andere Benutzer frei.
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
ht-degree: 0%

---

# Automatisierte Workflow-Vorlage erstellen

In diesem Video lernen Sie Folgendes:

* Erstellen Sie eine automatisierte Workflow-Vorlage für [!DNL  Workfront] Testversand
* Testversand-Empfänger zuweisen
* Legen Sie einen Termin für den Überprüfungs- und Genehmigungsprozess fest.
* Freigeben der automatisierten Workflow-Vorlage für andere

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Zusätzliche Statusaktivierungsoptionen

Es werden nur selten zwei Optionen verwendet, um zu bestimmen, wann ein Testversand-Workflow-Schritt gestartet werden soll: die [!UICONTROL Datum und Uhrzeit] und &quot;[!UICONTROL Wann der Termin für die vorherige Phase vergeht]&quot;.

Die zweite Option funktioniert nur in Szenarien, in denen eine große Gruppe von Personen eine Überprüfung durchführt und nicht auf alle warten möchte. Es ist eine Art &quot;Ich gebe Ihnen eine gewisse Zeit, um Ihre Überprüfung abzuschließen und dann verlieren Sie Ihre Chance&quot; Option. Aber selbst dies kann einen Überprüfungsprozess verlangsamen.

Wenn Sie &quot;[!UICONTROL wann der Termin der vorherigen Phase vergeht],&quot; ist es wichtig, sich daran zu erinnern, dass Sie eine Phase jederzeit manuell aktivieren können, wenn Sie nicht warten möchten, bis ein Termin erreicht ist.

## Best Practices

| Best Practice | Deshalb |
|---|---|
| Setzen Sie die Testversand-Rolle des Testversands auf &quot;Überprüfer&quot;. | Mit der Rolle Testversand überprüfen wird sichergestellt, dass der Ersteller des Testversands Kommentare abgeben und auf Kommentare zugreifen kann, die von anderen Benutzern hinterlassen wurden. Meistens muss der Ersteller des Testversands keine Entscheidung über einen hochgeladenen Testversand treffen. Die Rollen Genehmiger, Prüfer und Genehmiger, Autor oder Moderator-Testversand erfordern eine Entscheidung. Wenn dem Ersteller des Testversands eine dieser Rollen zugewiesen wird, er jedoch nie eine Entscheidung trifft, kann dies die Testversandfristen beeinträchtigen. |
| Vermeiden Sie die Verwendung der Rolle &quot;Testversand genehmigen&quot;. | Die Rolle &quot;Testversand genehmigen&quot;ermöglicht dem Benutzer keine Kommentare zu diesem Testversand. Dies könnte dazu führen, dass ein Benutzer den Testversand ohne jegliche Erklärung ablehnt, da er keine Kommentare abgeben konnte. Verwenden Sie stattdessen die Rolle &quot;Testversand für Prüfer und Genehmiger&quot;, damit der Benutzer Feedback geben kann. |
| Vermeiden Sie die Option E-Mail-Warnhinweis mit Aktivitätsnachweis . | Diese Option sendet eine E-Mail-Benachrichtigung zu jedem Fall, in dem ein Testversand durchgeführt wird - ein Kommentar, eine Antwort, eine Entscheidung etc. Der Empfänger sieht im Wesentlichen die Aktivität Testversand , sobald dies geschieht.<br><br>Für Testversand-Eigentümer und -Ersteller funktioniert der Benachrichtigungs-E-Mail-Warnhinweis &quot;Entscheidungen&quot;am besten für mehrstufige Testsendungen und die endgültige Entscheidung funktioniert am besten für einstufige Workflows. Im Allgemeinen können alle anderen auf Deaktiviert gesetzt werden, es sei denn, sie möchten über andere Personen informiert werden, die Kommentare oder Entscheidungen treffen (in diesem Fall kann eine der Zusammenfassungs-E-Mail-Optionen am besten funktionieren). |

---
title: Anfragegenehmigungsprozess in einer Anfragewarteschlange anwenden
description: Implementieren Sie einen standardmäßigen Genehmigungsprozess, um die Anfrage-Workflows zu optimieren und sicherzustellen, dass genehmigte Anfragen ihren Status entsprechend in „Neu“ ändern. Beheben Sie die Verwirrung bei abgelehnten Anfragen durch Auswahl einer Statusänderung in „Wird nicht aufgelöst“.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---

# Anfragegenehmigungsprozess in einer Anfragewarteschlange anwenden

>[!PREREQUISITES]
>
>* [Erstellen eines Anfrageflusses](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Erstellen eines globalen und eines einmaligen Genehmigungsprozesses](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


In diesem Video wird erläutert, wie Sie beim Erstellen einer Anfrage-Warteschlange einen Standardgenehmigungsprozess anwenden. &#x200B; Wenn eine Anfrage erstellt wird, beginnt sie mit dem Status „Neu - Ausstehende Genehmigung“ und eine Genehmigungsbenachrichtigung wird an die benannte genehmigende Person gesendet. &#x200B; Bei Genehmigung ändert sich der Status in „Neu“, sodass zugewiesene Personen mit der Arbeit beginnen können. &#x200B; Wenn er abgelehnt wird, wird der Status möglicherweise aufgrund eines häufigen Fehlers bei der Einrichtung des Genehmigungsprozesses fälschlicherweise auf „Neu“ zurückgesetzt. &#x200B;
In diesem Video wird hervorgehoben, dass der Genehmigungsprozess ausgelöst wird, wenn der Status auf „Neu“ festgelegt wird, was der Standard für neue Anfragen ist. &#x200B; Wird dieser abgelehnt, ändert das System standardmäßig den Status zurück in den vorherigen, was für neue Anfragen nicht ideal ist. &#x200B; Stattdessen sollte ein anderer Status wie „Wird nicht aufgelöst“ ausgewählt werden. &#x200B; In dem Video wird auch darauf hingewiesen, dass es keinen standardmäßig bereitgestellten Status „Abgelehnt“ gibt, sondern ein Systemadministrator bei Bedarf einen erstellen kann. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

## Wichtige Erkenntnisse

* **Standardgenehmigungsprozess:** Beim Erstellen einer Anfrage-Warteschlange können Sie einen standardmäßigen Genehmigungsprozess anwenden, der jeder Anfrage automatisch einen Genehmigungs-Workflow zuweist.
* **Statusänderungen bei Genehmigung:** genehmigten Anfragen ändern ihren Status von „Neu - Genehmigung ausstehend“ in „Neu“, sodass zugewiesene Personen beginnen können, daran zu arbeiten.
* **Häufiger Fehler bei der Verarbeitung von Ablehnungen:** Wenn eine Anfrage abgelehnt wird, wird der Status aufgrund einer Standardsystemeinstellung im Genehmigungsprozess auf „Neu“ zurückgesetzt.
* **Empfohlener Status für abgelehnte Anfragen:** Statt zum vorherigen Status („Neu„) zurückzukehren, ist es besser, einen anderen Status auszuwählen, z. B. „Wird nicht aufgelöst“, um Verwirrung zu vermeiden.
* **Benutzerdefinierte Statusoptionen:** Standardmäßig wird kein Status „Abgelehnt“ bereitgestellt, aber ein Systemadministrator kann bei Bedarf einen erstellen, um den Genehmigungsprozess klarer zu gestalten.


## Empfohlene Tutorials zu diesem Thema

* [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses](/help/manage-work/request-queues/create-a-request-flow.md)
* [Erstellen eines globalen und eines einmaligen Genehmigungsprozesses](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

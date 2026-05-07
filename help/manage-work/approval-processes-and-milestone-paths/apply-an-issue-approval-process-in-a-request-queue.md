---
title: Anwenden eines Problemgenehmigungsprozesses in einer Anfrage-Warteschlange
description: Implementieren Sie einen Standardgenehmigungsprozess, um Anfrage-Workflows zu optimieren und sicherzustellen, dass der Status genehmigter Anfragen entsprechend in „Neu“ geändert wird. Vermeiden Sie Verwirrung bei abgelehnten Anfragen, indem Sie „Lässt sich nicht lösen“ als Statusänderung wählen.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T15:58:59.618Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 426
ht-degree: 65%

---

# Anwenden eines Problemgenehmigungsprozesses in einer Anfrage-Warteschlange

>[!PREREQUISITES]
>
>* [Erstellen eines Anfrageflusses](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Erstellen eines globalen und eines einmaligen Genehmigungsprozesses](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


In diesem Video wird erläutert, wie Sie beim Erstellen einer Anfrage-Warteschlange einen Standardgenehmigungsprozess anwenden. &#x200B; Wenn eine Anfrage erstellt wird, beginnt sie mit dem Status „Neu - Ausstehende Genehmigung“ und eine Genehmigungsbenachrichtigung wird an die benannte genehmigende Person gesendet. &#x200B; der Genehmigung ändert sich der Status in „Neu“, sodass zugewiesene Personen mit der Arbeit beginnen können. &#x200B; der Ablehnung kann der Status aufgrund eines häufigen Fehlers bei der Einrichtung des Genehmigungsprozesses fälschlicherweise zu „Neu“ zurückgesetzt werden. &#x200B;
In diesem Video wird hervorgehoben, dass der Genehmigungsprozess ausgelöst wird, wenn der Status auf „Neu“ festgelegt wird, was der Standard für neue Anfragen ist. &#x200B; der Zurückweisung ändert das System standardmäßig den Status zurück in den vorherigen, was für neue Anfragen nicht ideal ist. &#x200B; Stattdessen sollte ein anderer Status wie „Wird nicht aufgelöst“ ausgewählt werden. &#x200B; Im Video wird auch darauf hingewiesen, dass standardmäßig kein Status „Abgelehnt“ bereitgestellt wird, ein Systemadministrator jedoch bei Bedarf einen erstellen kann. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## Wichtige Schlussfolgerungen

* **Standardgenehmigungsprozess:** Beim Erstellen einer Anfrage-Warteschlange können Sie einen Standardgenehmigungsprozess anwenden, der jeder Anfrage automatisch einen Genehmigungs-Workflow zuweist.
* **Statusänderungen bei Genehmigung:** Bei genehmigten Anfragen ändert sich der Status von „Neu – Ausstehende Genehmigung“ in „Neu“, sodass zugewiesene Personen beginnen können, daran zu arbeiten.
* **Häufiger Fehler beim Umgang mit Ablehnungen:** Wenn eine Anfrage abgelehnt wird, wird der Status aufgrund einer Standardsystemeinstellung im Genehmigungsprozess auf „Neu“ zurückgesetzt.
* **Empfohlener Status für abgelehnte Anfragen:** Statt zum vorherigen Status („Neu“) zurückzukehren, ist es besser, einen anderen Status auszuwählen, z. B. „Lässt sich nicht lösen“, um Verwirrung zu vermeiden.
* **Benutzerdefinierte Statusoptionen:** Standardmäßig wird kein Status „Abgelehnt“ bereitgestellt, aber die Systemadmins können bei Bedarf einen erstellen, um den Genehmigungsprozess klarer zu gestalten.


## Empfohlene Tutorials zu diesem Thema

* [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses](/help/manage-work/request-queues/create-a-request-flow.md)
* [Erstellen eines globalen und eines Genehmigungsprozesses für einmaligen Gebrauch](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

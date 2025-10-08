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
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: ht
source-wordcount: '376'
ht-degree: 100%

---

# Anwenden eines Problemgenehmigungsprozesses in einer Anfrage-Warteschlange

>[!PREREQUISITES]
>
>* [Erstellen eines Anfrageflusses](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Erstellen eines globalen und eines einmaligen Genehmigungsprozesses](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


In diesem Video wird beschrieben, wie Sie beim Erstellen einer Anfrage-Warteschlange einen Standardgenehmigungsprozess anwenden. Wenn eine Anfrage erstellt wird, weist sie zunächst den Status „Neu – Ausstehende Genehmigung“ auf. Außerdem wird eine Genehmigungsbenachrichtigung an die benannte genehmigende Person gesendet. Bei Genehmigung ändert sich der Status in „Neu“, sodass die zugewiesenen Personen mit der Arbeit beginnen können. Im Falle einer Ablehnung wird der Status unter Umständen aufgrund eines häufig auftretenden Fehlers im Genehmigungsprozess fälschlicherweise auf „Neu“ zurückgesetzt. 
Dieses Video hebt hervor, dass der Genehmigungsprozess ausgelöst wird, wenn der Status auf „Neu“ festgelegt wird (Standard bei neuen Anfragen). Bei einer Ablehnung setzt das System standardmäßig den Status auf den vorherigen zurück. Für neue Anfragen ist das nicht ideal. Stattdessen sollte ein anderer Status wie „Lässt sich nicht lösen“ ausgewählt werden. In dem Video wird auch darauf hingewiesen, dass es keinen standardmäßig bereitgestellten Status „Abgelehnt“ gibt. Bei Bedarf kann dieser aber von Systemadmins erstellt werden. 

>[!VIDEO](https://video.tv.adobe.com/v/3455033/?quality=12&learn=on&enablevpops=1&captions=ger)

## Die wichtigsten Punkte

* **Standardgenehmigungsprozess:** Beim Erstellen einer Anfrage-Warteschlange können Sie einen Standardgenehmigungsprozess anwenden, der jeder Anfrage automatisch einen Genehmigungs-Workflow zuweist.
* **Statusänderungen bei Genehmigung:** Bei genehmigten Anfragen ändert sich der Status von „Neu – Ausstehende Genehmigung“ in „Neu“, sodass zugewiesene Personen beginnen können, daran zu arbeiten.
* **Häufiger Fehler beim Umgang mit Ablehnungen:** Wenn eine Anfrage abgelehnt wird, wird der Status aufgrund einer Standardsystemeinstellung im Genehmigungsprozess auf „Neu“ zurückgesetzt.
* **Empfohlener Status für abgelehnte Anfragen:** Statt zum vorherigen Status („Neu“) zurückzukehren, ist es besser, einen anderen Status auszuwählen, z. B. „Lässt sich nicht lösen“, um Verwirrung zu vermeiden.
* **Benutzerdefinierte Statusoptionen:** Standardmäßig wird kein Status „Abgelehnt“ bereitgestellt, aber die Systemadmins können bei Bedarf einen erstellen, um den Genehmigungsprozess klarer zu gestalten.


## Empfohlene Tutorials zu diesem Thema

* [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses](/help/manage-work/request-queues/create-a-request-flow.md)
* [Erstellen eines globalen und eines einmaligen Genehmigungsprozesses](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

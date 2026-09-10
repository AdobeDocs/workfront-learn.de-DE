---
source-git-commit: b150105844a42e06f5e96f787ad62a1b62185f91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 51%

---
# Anfragegenehmigungsprozess in einer Anfragewarteschlange anwenden - FREIGEGEBEN

>[!PREREQUISITES]
>
>* [Erstellen eines Anfrageflusses in Workfront](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Genehmigungsprozesse erstellen und verwalten](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


In diesem Video wird erläutert, wie Sie beim Erstellen einer Anfrage-Warteschlange einen Standardgenehmigungsprozess anwenden. &#x200B; Wenn eine Anfrage erstellt wird, beginnt sie mit dem Status „Neu - Ausstehende Genehmigung“ und eine Genehmigungsbenachrichtigung wird an die benannte genehmigende Person gesendet. &#x200B; der Genehmigung ändert sich der Status in „Neu“, sodass zugewiesene Personen mit der Arbeit beginnen können. &#x200B; der Ablehnung kann der Status aufgrund eines häufigen Fehlers bei der Einrichtung des Genehmigungsprozesses fälschlicherweise zu „Neu“ zurückgesetzt werden. &#x200B;
In diesem Video wird hervorgehoben, dass der Genehmigungsprozess ausgelöst wird, wenn der Status auf „Neu“ festgelegt wird, was der Standard für neue Anfragen ist. &#x200B; der Zurückweisung ändert das System standardmäßig den Status zurück in den vorherigen, was für neue Anfragen nicht ideal ist. &#x200B; Stattdessen sollte ein anderer Status wie „Wird nicht aufgelöst“ ausgewählt werden. &#x200B; Im Video wird auch darauf hingewiesen, dass standardmäßig kein Status „Abgelehnt“ bereitgestellt wird, ein Systemadministrator jedoch bei Bedarf einen erstellen kann. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455033/?captions=ger&quality=12&learn=on&enablevpops=1)

## Wichtige Schlussfolgerungen

* **Standardgenehmigungsprozess:** Beim Erstellen einer Anfrage-Warteschlange können Sie einen Standardgenehmigungsprozess anwenden, der jeder Anfrage automatisch einen Genehmigungs-Workflow zuweist.
* **Statusänderungen bei Genehmigung:** Bei genehmigten Anfragen ändert sich der Status von „Neu – Ausstehende Genehmigung“ in „Neu“, sodass zugewiesene Personen beginnen können, daran zu arbeiten.
* **Häufiger Fehler beim Umgang mit Ablehnungen:** Wenn eine Anfrage abgelehnt wird, wird der Status aufgrund einer Standardsystemeinstellung im Genehmigungsprozess auf „Neu“ zurückgesetzt.
* **Empfohlener Status für abgelehnte Anfragen:** Statt zum vorherigen Status („Neu“) zurückzukehren, ist es besser, einen anderen Status auszuwählen, z. B. „Lässt sich nicht lösen“, um Verwirrung zu vermeiden.
* **Benutzerdefinierte Statusoptionen:** Standardmäßig wird kein Status „Abgelehnt“ bereitgestellt, aber die Systemadmins können bei Bedarf einen erstellen, um den Genehmigungsprozess klarer zu gestalten.


## Empfohlene Tutorials zu diesem Thema

* [Aufgaben, Probleme und Genehmigungen effektiv delegieren](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses in Workfront](/help/manage-work/request-queues/create-a-request-flow.md)
* [Genehmigungsprozesse erstellen und verwalten](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


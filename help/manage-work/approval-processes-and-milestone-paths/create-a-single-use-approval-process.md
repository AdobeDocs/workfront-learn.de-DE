---
title: Erstellen eines globalen und eines einmaligen Genehmigungsprozesses
description: Erfahren Sie, wie Sie ein einmaliges Genehmigungsverfahren für ein Projekt, eine Aufgabe oder ein Problem in Workfront erstellen können.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
last-substantial-update: 2024-09-24T00:00:00Z
recommendations: noDisplay,noCatalog
exl-id: 85d28b54-72a6-4dd1-bac8-8e7ffb3e2b76
doc-type: video
source-git-commit: b0114985964736fb7bb234c581cb56930714915c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 42%

---

# Erstellen eines globalen und eines einmaligen Genehmigungsprozesses

Genehmigungsverfahren für Projekte, Aufgaben und Probleme ermöglichen es der Projekt-Managerin oder dem Projekt-Manager, sich von Fachleuten bestätigen zu lassen, dass die Arbeit richtig gemacht wurde, bevor es weitergeht. Der Projektmanager kann für jede Situation einen Validierungsprozess erstellen (dies wird als Validierungsprozess für einzelne Verwendungszwecke bezeichnet) oder aus einer Liste von möglicherweise vielen Validierungsprozessen auswählen, die zuvor erstellt wurden, um gemeinsamen Anforderungen zu entsprechen (diese werden als globale oder vorhandene Validierungsprozesse bezeichnet).

In beiden Instanzen wird die genehmigende Person, wenn sich der Objektstatus in einen im Genehmigungsverfahren festgelegten Status ändert, auf verschiedene Weise benachrichtigt, um die Arbeit zu überprüfen und sie zu genehmigen oder abzulehnen. Da es sein kann, dass das gesamte Projekt bis zur Genehmigung pausiert wird, sollten sich die Genehmigenden schon im Voraus darüber im Klaren sein, dass sie möglicherweise um eine Genehmigung ersucht werden. Sind genehmigende Personen aus irgendeinem Grund abwesend, können sie dann ihre Genehmigungen an qualifizierte Vertretende delegieren. Siehe [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md) für Details.

In diesem Video erfahren Sie, wie Sie einen globalen Genehmigungsprozess und einen einmaligen Genehmigungsprozess für ein Projekt, eine Aufgabe oder ein Problem erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on)

>[!TIP]
>
>Sie können ein einmaliges Genehmigungsverfahren für ein Projekt oder eine Aufgabe zu einer Projektvorlage hinzufügen.

>[!NOTE]
>
>Sie können eine einmalige Genehmigung für Projekte und Probleme auf die gleiche Weise einrichten, wie es im Video für Aufgaben beschrieben wird.

## Anwenden automatischer Problemvalidierungen in einer Anforderungswarteschlange

Wenn Sie automatische Problemgenehmigungen in einer Anforderungswarteschlange einrichten möchten, können diese nur mithilfe eines globalen Genehmigungsprozesses für Probleme durchgeführt werden und werden in einem [!UICONTROL Warteschlangenthema] angewendet.

Wählen Sie beim Erstellen oder Bearbeiten eines [!UICONTROL Queue-Themas] den globalen Genehmigungsprozess im Feld **[!UICONTROL Standardgenehmigung]** aus.

![Bild, das zeigt, wie ein standardmäßiger Genehmigungsprozess in einem Warteschlangenthema ausgewählt wird](assets/automatic-issue-approval-1.png)

Möglicherweise müssen Sie den Prozess zur Genehmigung von Problemen bearbeiten, um sicherzustellen, dass der **[!UICONTROL Vorheriger Status]** nicht dem entspricht, auf den das Problem gesetzt ist, wenn die Genehmigung abgelehnt wird. Der Grund dafür ist, dass der vorherige Status **[!UICONTROL Neu]** lautet und dies auch der Status ist, der den Genehmigungsprozess Trigger. Daher ist es der Status, auf den er bei Genehmigung festgelegt wird. Um Verwirrung zu vermeiden, wenn die Genehmigung eines Problems abgelehnt wird, sollten Sie den Status auf einen Wert wie **[!UICONTROL Wird nicht aufgelöst]** oder einen benutzerdefinierten Status festlegen, der zu diesem Zweck erstellt wurde.

![Bild, das die Änderung des Status anzeigt, der verwendet werden soll, wenn das Problem abgelehnt wird](assets/automatic-issue-approval-2.png)


## Empfohlene Tutorials zu diesem Thema

* [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Anhängen und Bearbeiten vorhandener Genehmigungsprozesse](/help/manage-work/approval-processes-and-milestone-paths/attach-and-edit-existing-approval-processes.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses](/help/manage-work/request-queues/create-a-request-flow.md)


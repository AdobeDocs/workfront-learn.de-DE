---
title: Erstellen eines globalen und eines einmaligen Genehmigungsprozesses
description: Erfahren Sie, wie Sie einen globalen und einen einmaligen Genehmigungsprozess für ein Projekt, eine Aufgabe oder ein Problem erstellen.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:20:03.459Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 448
ht-degree: 100%

---

# Erstellen eines globalen und eines einmaligen Genehmigungsprozesses

Genehmigungsverfahren für Projekte, Aufgaben und Probleme ermöglichen es der Projekt-Managerin oder dem Projekt-Manager, sich von Fachleuten bestätigen zu lassen, dass die Arbeit richtig gemacht wurde, bevor es weitergeht. Die Projekt-Managerin bzw. der Projekt-Manager kann einen Genehmigungsprozess für jede Situation erstellen (dies wird als einmaliger Genehmigungsprozess bezeichnet) oder aus einer Liste von möglicherweise zuvor erstellten Genehmigungsprozessen wählen, um gängige Bedürfnisse zu erfüllen (diese werden als globale oder vorhandene Genehmigungsprozesse bezeichnet).

In beiden Instanzen wird die genehmigende Person, wenn sich der Objektstatus in einen im Genehmigungsverfahren festgelegten Status ändert, auf verschiedene Weise benachrichtigt, um die Arbeit zu überprüfen und sie zu genehmigen oder abzulehnen. Da es sein kann, dass das gesamte Projekt bis zur Genehmigung pausiert wird, sollten sich die Genehmigenden schon im Voraus darüber im Klaren sein, dass sie möglicherweise um eine Genehmigung ersucht werden. Sind genehmigende Personen aus irgendeinem Grund abwesend, können sie dann ihre Genehmigungen an qualifizierte Vertretende delegieren. Siehe [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md) für Details.

In diesem Video erfahren Sie, wie Sie einen globalen und einen einmaligen Genehmigungsprozess für ein Projekt, eine Aufgabe oder ein Problem erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on&enablevpops=1)

>[!TIP]
>
>Sie können ein einmaliges Genehmigungsverfahren für ein Projekt oder eine Aufgabe zu einer Projektvorlage hinzufügen.

>[!NOTE]
>
>Sie können eine einmalige Genehmigung für Projekte und Probleme auf die gleiche Weise einrichten, wie es im Video für Aufgaben beschrieben wird.

## Anwenden automatischer Problemgenehmigungen in einer Anfrage-Warteschlange

Wenn Sie automatische Problemgenehmigungen in einer Anfrage-Warteschlange einrichten möchten, kann dies nur mithilfe eines globalen Genehmigungsprozesses für Probleme durchgeführt und auf ein [!UICONTROL Warteschlangen-Thema] angewendet werden.

Wählen Sie beim Erstellen oder Bearbeiten eines [!UICONTROL Warteschlangen-Themas] im Feld **[!UICONTROL Standardgenehmigung]** den globalen Genehmigungsprozess aus.

![Bild, das zeigt, wie ein standardmäßiger Genehmigungsprozess für ein Warteschlangen-Thema ausgewählt wird](assets/automatic-issue-approval-1.png)

Möglicherweise müssen Sie den Problem-Genehmigungsprozess bearbeiten, um sicherzustellen, dass der Problemstatus nicht auf **[!UICONTROL Vorheriger Status]** gesetzt ist, wenn die Genehmigung abgelehnt wird. Der Grund dafür ist, dass der vorherige Status **[!UICONTROL Neu]** lautet. Dies ist auch der Status, der den Genehmigungsprozess auslöst und deshalb bei der Genehmigung angezeigt wird. Um Verwirrung zu vermeiden, wenn die Genehmigung eines Problems abgelehnt wird, sollten Sie den Status auf einen Wert wie **[!UICONTROL Lässt sich nicht lösen]** oder einen benutzerdefinierten, zu diesem Zweck erstellten Status stellen.

![Bild, das die Änderung des Status anzeigt, der verwendet werden soll, wenn das Problem abgelehnt wird](assets/automatic-issue-approval-2.png)


## Empfohlene Tutorials zu diesem Thema

* [Delegieren von Aufgaben, Problemen und Genehmigungen](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Informationen zu gruppenspezifischen Genehmigungsprozessen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Erstellen eines Anfrageflusses](/help/manage-work/request-queues/create-a-request-flow.md)


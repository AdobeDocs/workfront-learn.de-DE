---
title: Sichtbarkeit in Ressourcen-Management-Tools
description: Erfahren Sie, was eine primär zugewiesene Person ist und wie sie sich auf die Verwaltung Ihrer Ressourcen auswirkt.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10184
exl-id: 3818c7fb-b820-4002-bf49-9c79c9f0afb2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '175'
ht-degree: 100%

---

# Sichtbarkeit in Ressourcen-Management-Tools

Zu wissen, wer wann verfügbar ist, ist für die Ressourcenplanung und -verwaltung von entscheidender Bedeutung. Wenn Benutzende ihre persönliche Freizeit im Workfront-Kalender markieren, können diese Informationen auch in den Ressurcen-Tools von Workfront angezeigt werden.

## Ressourcenplaner

Die Ausfallzeit einer Person wird in der Spalte „Verfügbar (AVL)“ des Ressourcenplaners angezeigt. Workfront zieht die in ihrem Kalender markierte Ausfallzeit von der verfügbaren Zeit ab, die Workfront auf Grundlage des zugewiesenen Zeitplans, des Aufgabengebietsanteils usw. berechnet.

![Ausfallzeit in der Spalte „Verfügbar“](assets/vis_01.png)

## Workload-Balancer

Im Workload Balancer erscheinen die Ausfallzeiten als graue Balken im Kalender. Diese Sichtbarkeit hilft Ressourcen-Managerinnen und -Managern und anderen, fundiertere Entscheidungen bei der Arbeitszuweisung zu treffen.

Die Ausfallzeitmarkierung verhindert jedoch nicht, dass der Person über den Workload Balancer Arbeit zugewiesen wird. Wenn Arbeit zugewiesen wird, zeigt der Workload Balancer an, dass die Person während der Ausfallphase überlastet ist.

![Grauer Balken für Ausfallzeit](assets/vis_02.png)

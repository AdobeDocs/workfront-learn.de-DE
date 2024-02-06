---
title: Verfolgen des Fortschritts über die Projektzeitleiste
description: Erfahren Sie, wie Sie den Arbeitsfortschritt auf der Projektzeitleiste in [!DNL  Workfront] anhand von prozentualer Abschlussrate, Status, Zuweisungen oder Einschränkungen verfolgen können.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Beginner
jira: KT-10150
exl-id: c8793f49-24b8-48cc-af84-5239234ead0e
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 100%

---

# Verfolgen des Fortschritts über die Projektzeitleiste

Vergewissern Sie sich, dass die Aufgaben so vorankommen, wie sie sollten, um die Projektfristen einzuhalten. Beim Durchsuchen der [!UICONTROL Aufgabenliste] gibt es in [!DNL  Workfront] mehrere Funktionen, die Ihnen helfen, den Fortschritt und den Status der Arbeit zu überwachen.

## Prozent abgeschlossen

Die prozentuale Abschlussrate der einzelnen Arbeitsaufgaben wird manchmal verwendet, um den Arbeitsfortschritt zu messen. Es ist wichtig zu beachten, dass dieses Feld manuell angepasst werden muss, da es der Einschätzung der Benutzenden obliegt, wie weit sie sind.

>[!TIP]
>
>Auch wenn die prozentuale Abschlussrate der Arbeitsaufgaben manuell aktualisiert werden muss, wird die prozentuale Abschlussrate einer Hauptaufgabe von Workfront basierend auf der prozentualen Abschlussrate und entweder der Dauer oder den geplanten Stunden jeder Unteraufgabe berechnet. Das bedeutet, dass Sie eine bessere Genauigkeit zur prozentualen Abschlussrate erhalten, wenn Sie große Aufgaben in kleinere Unteraufgaben unterteilen.


![Projektaufgabenliste mit der Spalte [!UICONTROL Prozent abgeschlossen]](assets/planner-fund-task-percent-complete.png)

Es gibt drei Zeitpunkte, zu denen sich die prozentuale Abschlussrate automatisch ändert:

* Wenn der [!UICONTROL Aufgabenstatus] auf „Abgeschlossen“ gesetzt wird, ändert sich die prozentuale Abschlussrate auf 100.
* Wenn der [!UICONTROL Aufgabenstatus] auf „Neu“ zurückgesetzt wird, wird die prozentuale Abschlussrate auf 0 zurückgesetzt.
* In einer übergeordneten Aufgabe, wenn sich die prozentuale Abschlussrate einer untergeordneten Aufgabe ändert.

## Status

Fügen Sie die [!UICONTROL Statusspalte] in eine [!UICONTROL Ansicht] ein, um schnell zu sehen, welche Aufgaben gestartet wurden, welche in Bearbeitung sind und welche abgeschlossen sind. Sie können sogar eine bedingte Formatierung in einer [!UICONTROL Ansicht] einrichten, um jeden Status farblich zu kodieren und so die Informationen leichter zu entziffern.

## Aufgabenzuweisungen

Überprüfen Sie bei der Durchsicht des Projekts auch die Aufgabenzuweisungen. Vielleicht ist die Arbeit in Verzug geraten, weil niemandem die Aufgabe zugeordnet war. Oder die zugeordnete Person hatte nicht die richtigen Fähigkeiten, um die Arbeit zu erledigen. Fügen Sie dann einer Aufgabe weitere Personen hinzu oder weisen Sie Aufgaben neu zu, um sicherzustellen, dass die Arbeit erledigt wird.

## Aufgabenbeschränkung

Manchmal werden Aufgabenbeschränkungen geändert, ohne dass Sie es merken. Einschränkungen können das Verhalten Ihrer Zeitleiste beeinflussen, daher sollten Sie sicherstellen, dass sie so eingestellt sind, wie Sie es wünschen.

![Aufgabenliste des Projekts mit Spalte für Aufgabenbeschränkungen](assets/planner-fund-task-constraint.png)

Erstellen Sie eine benutzerdefinierte Ansicht, die die Spalte [!UICONTROL Aufgabenbeschränkung] enthält, um diese Informationen in Ihrer Aufgabenliste anzuzeigen. Wenn Sie das Projekt von einem Starttermin aus geplant haben, sollten Ihre Aufgaben die Beschränkung [!UICONTROL So bald wie möglich] ([!UICONTROL ASAP]) haben.

Weitere Details zu Aufgabenbeschränkungen finden Sie unter [Verstehen und Verwalten von Dauertypen und Aufgabenbeschränkungen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=de).

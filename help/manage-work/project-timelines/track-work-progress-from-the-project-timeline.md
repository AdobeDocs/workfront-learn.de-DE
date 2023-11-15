---
title: Verfolgen des Fortschritts über die Projekt-Timeline
description: Erfahren Sie, wie Sie den Fortschritt der Arbeit über die Projekt-Timeline in [!DNL  Workfront] Verwendung von "Prozent abgeschlossen", "Status", "Zuweisungen"oder "Begrenzungen".
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
source-wordcount: '417'
ht-degree: 0%

---

# Verfolgen des Fortschritts über die Projekt-Timeline

Stellen Sie sicher, dass die Aufgaben so vorankommen, wie sie die Projektzeiträume erreichen sollten. Während Sie durch die [!UICONTROL Aufgabe] auflisten, gibt es mehrere Funktionen in [!DNL  Workfront] die Ihnen dabei helfen, den Fortschritt und den Status der Arbeit zu überwachen.

## Prozent abgeschlossen

Der Prozentsatz, der für jede Arbeitsaufgabe abgeschlossen ist, wird manchmal verwendet, um den Fortschritt der Arbeit zu messen. Beachten Sie, dass dieses Feld manuell angepasst werden muss, da der Bevollmächtigte schätzt, wie weit sie sind.

>[!TIP]
>
>Auch wenn der prozentuale Anteil, der mit Arbeitsaufgaben fertig gestellt ist, manuell aktualisiert werden muss, wird der prozentuale Abschluss einer Hauptaufgabe von Workfront basierend auf dem Prozentsatz der Fertigstellung und entweder auf der Dauer oder den geplanten Stunden jeder Unteraufgabe berechnet. Das bedeutet, dass Sie eine bessere Prozentgenauigkeit erhalten, wenn Sie große Aufgaben in kleinere Unteraufgaben unterteilen.


![Liste der Projektaufgaben anzeigen [!UICONTROL Prozent abgeschlossen] column](assets/planner-fund-task-percent-complete.png)

Es gibt dreimal, wenn sich der prozentuale Abschluss automatisch ändert:

* Wenn die Aufgabe [!UICONTROL Status] auf &quot;Fertig stellen&quot;eingestellt ist, wird der Prozentsatz für die Fertigstellung auf 100 gesetzt.
* Wenn die Aufgabe [!UICONTROL Status] wird zurück auf Neu gesetzt, wird der prozentuale Abschluss auf 0 zurückgesetzt.
* In einer übergeordneten Aufgabe, wenn sich der Prozentsatz des Abschlusses einer untergeordneten Aufgabe ändert.

## Status

Fügen Sie die [!UICONTROL Status] in einer Spalte [!UICONTROL Ansicht] um schnell zu sehen, welche Aufgaben gestartet wurden, welche ausgeführt werden und welche abgeschlossen sind. Sie können sogar die bedingte Formatierung in einer [!UICONTROL Ansicht] um jeden Status farblich zu kennzeichnen, wodurch die Informationen leichter zu entschlüsseln sind.

## Aufgabenzuweisungen

Überprüfen Sie beim Überprüfen des Projekts die Aufgabenzuweisungen. Vielleicht fiel die Arbeit zurück, weil niemand der Aufgabe zugewiesen war. Oder vielleicht hatte die zugewiesene Person nicht die richtigen Fähigkeiten, um die Arbeit abzuschließen. Fügen Sie einer Aufgabe weitere Personen hinzu oder weisen Sie Aufgaben neu zu, um sicherzustellen, dass die Arbeit erledigt wird.

## Aufgabenbeschränkung

Manchmal werden Aufgabenbegrenzungen geändert und Sie erkennen sie nicht. Einschränkungen können sich auf das Verhalten Ihrer Timeline auswirken. Stellen Sie also sicher, dass sie so eingerichtet sind, wie Sie sie möchten.

![Aufgabenliste des Projekts mit Spalte für Aufgabeneinschränkungen](assets/planner-fund-task-constraint.png)

Erstellen Sie eine benutzerdefinierte Ansicht, die die [!UICONTROL Aufgabenbegrenzung] -Spalte, um diese Informationen in Ihrer Aufgabenliste anzuzeigen. Wenn Sie das Projekt von einem Startdatum an geplant haben, sollen Ihre Aufgaben die [!UICONTROL So bald wie möglich] ([!UICONTROL ASAP]).

Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter [Typen und Aufgabenbegrenzungen von Dauer verstehen und verwalten](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).

---
title: Anzeigen der Zeitabstände wirkt sich auf die Projektzeitpläne aus
description: Erfahren Sie, was mit einer Projekt-Timeline passiert, wenn die Einstellung ein- und ausgeschaltet ist.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
kt: 10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# Auswirkungen der Zeitüberschreitung auf die Projektzeitpläne

Ob die Zeitpunkte eines zugewiesenen Benutzers in der Projekt-Timeline von einer Projekteinstellung mit dem Namen [!UICONTROL Zeitlimit für Benutzer]. Mit dieser Einstellung wird festgelegt, ob die Zeitspanne, die der primäre Verantwortliche der Aufgabe für diese Aufgabe benötigt, die für das Projekt geplanten Daten anpasst.

Sehen wir uns an, was mit einer Projekt-Timeline passiert, wenn jede der Einstellungen ausgewählt ist - C[!UICONTROL Benutzerzeitlimit in Aufgabendauer berücksichtigen] oder [!UICONTROL Ignorieren der Benutzerzeit in der Aufgabendauer].

![Einstellung der Benutzerzeit](assets/toapt_01.png)

## Benutzer-Ausfallzeit in Aufgabenlaufzeiten berücksichtigen

Diese Option ist die Standardeinstellung von Workfront.

In diesem Beispiel hat der primäre Verantwortliche für die Aufgabe im Kalender seiner Person Tage mit Markierungen.

![persönlicher Kalender](assets/toapt_02.png)

Der Projektmanager möchte diese Person einer Aufgabe zuweisen, deren geplante Daten sich über die Zeitspanne des Benutzers hinausgehen.

![Projektaufgabe mit Datumsangaben](assets/toapt_03.png)

Wenn dieser Benutzer der Aufgabe zugewiesen wird, werden die geplanten Datumsangaben automatisch angepasst. Jetzt wurde das geplante Abschlussdatum der Aufgabe um mehrere Tage verlängert, um die Zeitspanne des Benutzers aufzunehmen. Es ist wichtig zu beachten, dass diese Änderung die geplanten Termine für andere Aufgaben im Projekt und möglicherweise das geplante Abschlussdatum des Projekts beeinflussen kann.

![Projektaufgabe mit Fälligkeitsdatum](assets/toapt_04.png)

## [!UICONTROL Benutzer-Ausfallzeit in Aufgabenlaufzeiten ignorieren]

Mit dieser Option bleiben die geplanten Termine der Aufgabe wie ursprünglich geplant, auch wenn der Hauptverantwortliche während der Dauer dieser Aufgabe über eine Zeitspanne verfügt.

Der Teammitglied hat Tage frei markiert auf seinem Kalender.

![Kalender mit markierten Datumsangaben](assets/toapt_05.png)

Der Projektmanager weist ihnen eine Aufgabe zu, die sich mit der Zeitdauer überschneidet. Sobald der Benutzer zugewiesen wurde, bleiben die geplanten Aufgabendaten wie ursprünglich geplant.

![Anpassen der Projektaufgabedaten](assets/toapt_06.png)

Um sicherzustellen, dass die Arbeit rechtzeitig erledigt wird, kann es hilfreich sein, eine andere Person zuzuweisen, die an der Aufgabe arbeiten kann, während der ursprüngliche Bevollmächtigte nicht im Büro ist.

## Passen Sie die Einstellung auf Projektebene an.

So ändern Sie die Einstellung für die Benutzerzeit in einem Projekt:

* Öffnen Sie das Projekt, indem Sie in Workfront auf seinen Namen klicken.

* Auswählen [!UICONTROL Bearbeiten] über das Menü mit 3 Punkten in der Kopfzeile der Seite rechts neben dem Projektnamen.

* Scrollen Sie zum [!UICONTROL Projekteinstellungen] und suchen Sie nach [!UICONTROL Zeitlimit für Benutzer] -Feld.

* Wählen Sie die Option aus, die Sie auf dieses Projekt anwenden möchten — [!UICONTROL Benutzerzeitlimit in Aufgabendauern berücksichtigen] I[!UICONTROL Nutzerzeitlimit in Aufgabendauer ignorieren].

* Klicken Sie auf [!UICONTROL Speichern] in der oberen rechten Ecke des Fensters.

![Benutzer-Ausfallzeit in Aufgabenlaufzeiten berücksichtigen](assets/toapt_07.png)


**Hinweis**: Diese Einstellung ist nicht verfügbar, wenn Sie [!UICONTROL Projektdetails] im linken Bedienfeldmenü der Projektseite.

Eine globale Einstellung dafür ist in den Projektvoreinstellungen im Abschnitt [!UICONTROL Einrichtung] Menü. Diese Einstellung wird von Ihrem Systemadministrator verwaltet. Gruppenadministratoren können diese Einstellung möglicherweise für die von ihnen verwalteten Gruppen anpassen.

Workfront empfiehlt, die Einstellung so festzulegen, wie Sie möchten, dass die meisten Ihrer Projekte eine Zeitüberschreitung in Ihrem Unternehmen verarbeiten.

Die Einstellung kann auch in Projektvorlagen über die Vorlagendetails integriert werden.

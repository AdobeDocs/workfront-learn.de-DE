---
title: Grundlegende bedingte Formatierung hinzufügen
description: In diesem Video erfahren Sie, was die bedingte Formatierung in einer Ansicht ist und wie bedingte Formatierungen in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
source-git-commit: b09d634a8b4ec32eda2663f1df04cc8bc04596a9
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Ansicht grundlegende bedingte Formatierungen hinzufügen

In diesem Video erfahren Sie:

* Welche bedingten Formatierungen gibt es in der Ansicht?
* Erstellen und Ändern der bedingten Formatierung

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12)

## Aktivität: Bedingte Formatierung zu einer Ansicht hinzufügen

Erstellen Sie eine Aufgabenansicht mit dem Namen &quot;Standard + Fortschritt&quot;, indem Sie die vorhandene Standardansicht verwenden und diese bedingte Formatierung zum [!UICONTROL Name] Spalte.

1. Fügen Sie eine Spaltenregel hinzu, die den Feldhintergrund rot macht, wenn der Fortschritt der Aufgabe überfällig ist.
1. Fügen Sie eine Spaltenregel hinzu, die den Feldhintergrund gelb macht, wenn der Fortschrittsstatus &quot;Hinter&quot;oder &quot;At Risk&quot;lautet.

Auf diese Weise können Sie problematische Aufgaben erkennen, ohne die Spalte für den Fortschrittsstatus als Teil Ihrer Ansicht aufzunehmen.

## Antwort

![Ein Bild des Bildschirms zum Erstellen einer neuen Spaltenregel](assets/conditional-formatting-exercise.png)

1. Gehen Sie in einem Aufgabenlistenbericht zum **[!UICONTROL Ansicht]** Dropdown-Menü und **[!UICONTROL Neue Ansicht]**.
1. Benennen Sie Ihre Ansicht mit &quot;Standard + Fortschritt&quot;.
1. Verwenden Sie die Standardspalten.
1. Wählen Sie die [!UICONTROL Aufgabenname] Spalte. Dies ist die Spalte, auf die Sie die bedingte Formatierung anwenden möchten. Sie wird rot oder gelb angezeigt, wenn der Fortschritt der Aufgabe nicht &quot;Einschaltzeit&quot;lautet.
1. Klicken **[!UICONTROL Erweiterte Optionen]** oben rechts im ReportBuilder-Fenster.
1. Klicken **[!UICONTROL Eine Regel für diese Spalte hinzufügen]**.
1. Starten Sie die Spaltenregel, indem Sie [!UICONTROL Aufgabe] > [!UICONTROL Name] oben im Fenster zu [!UICONTROL Aufgabe] > [!UICONTROL Statusfortschritt]. Klicken Sie einfach auf **[!UICONTROL X]** Symbol neben [!UICONTROL Aufgabe] > [!UICONTROL Name] , um es aus dem Feld zu löschen.
1. Geben Sie &quot;progress&quot;in das Feld ein und wählen Sie dann [!UICONTROL Statusfortschritt] unter [!UICONTROL Aufgabe] -Feldquelle.
1. Auswählen **[!UICONTROL Verspätet]** im Feld rechts neben dem Feld [!UICONTROL Gleich] qualifier.
1. Wählen Sie einen roten Hintergrund im [!UICONTROL Textfarbe] Zeile.
1. Klicken **[!UICONTROL Regel hinzufügen]** , um die Spaltenregel zu speichern.
1. Jetzt klicken **[!UICONTROL Spaltenregel hinzufügen]** erneut, um eine weitere Regel hinzuzufügen.
1. Löschen Sie wie zuvor [!UICONTROL Aufgabe] > [!UICONTROL Name] aus dem Kriterienfeld aus. Ersetzen Sie es durch [!UICONTROL Statusfortschritt] unter [!UICONTROL Aufgabe] -Feldquelle.
1. Wählen Sie beides aus [!UICONTROL Risiko] und [!UICONTROL Hinter] im Feld rechts neben dem Gleichen Qualifizierer.
1. Wählen Sie einen gelben Hintergrund im [!UICONTROL Textfarbe] Zeile.
1. Klicken **[!UICONTROL Regel hinzufügen]** , um die Spaltenregel zu speichern.
1. Klicken **[!UICONTROL Ansicht speichern]** , um die Ansicht zu speichern.

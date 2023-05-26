---
title: Grundlegende bedingte Formatierung hinzufügen
description: Erfahren Sie, wie Sie mithilfe von Spaltenregeln die Textfarbe, Formatierung und Hintergrundfarben in einem Bericht oder einer Ansicht basierend auf von Ihnen festgelegten Kriterien ändern können.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 0ee80dceb8208bd0360fd8c9ab68fb8a73677a9d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Ansicht grundlegende bedingte Formatierungen hinzufügen

Die bedingte Formatierung erfolgt durch Erstellen von Spaltenregeln. Mithilfe von Spaltenregeln können Sie eine Spalte basierend auf von Ihnen festgelegten Kriterien in einer bestimmten Weise formatieren.

In diesem Video erfahren Sie:

* Welche bedingten Formatierungen gibt es in der Ansicht?
* Erstellen und Ändern der bedingten Formatierung

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## Zusammenfassung

So erstellen Sie eine bedingte Formatierung:

1. Wählen Sie die Spalte aus, in der die Formatierung angezeigt werden soll
1. Entscheiden Sie, welche Bedingungen die Formatierung ändern soll.
1. Entscheiden, welche Formatierungsänderungen am besten funktionieren

   * Hintergrundfarbe
   * Textfarbe
   * Ersatztext
   * Symbol anzeigen

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

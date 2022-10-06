---
title: Switch-Funktion
description: Erfahren Sie, wie Sie die Switch-Funktion mit der Switch-Funktion verwenden.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Switch-Funktion

Erfahren Sie, wie Sie die Switch-Funktion mit der Switch-Funktion verwenden.

## Übungsübersicht

Verwenden Sie für einfache Datenänderungen die Switch-Funktion, um innerhalb eines Modulfelds einen Wert in einen anderen umzuwandeln. Ändern Sie in dieser Übung den zweistelligen Schlüssel in den tatsächlichen Namen, damit der Projektfortschrittsstatus in eine E-Mail gesendet werden kann.

![Switch-Funktion Bild 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Klonen Sie das Szenario mit dem Namen &quot;Freigeben von Variablen zwischen Routing-Pfaden&quot;.
1. Nennen Sie das neue Szenario &quot;Freigeben von Variablen zwischen Routing-Pfaden - Wechsel&quot;.
1. Klicken Sie auf das Trigger-Modul und fügen Sie dem Bereich &quot;Outputs&quot;den Fortschrittsstatus hinzu.
1. Fügen Sie im Modul E-Mail senden dem Feld Inhalt den Fortschrittsstatus hinzu.

   + Wenn Sie einfach den Wert aus dem Suchmodul zuordnen, gibt es einen aus zwei Buchstaben bestehenden Code für den Fortschrittsstatus.
   + Um den Code für den vollständigen Namen jedes möglichen Fortschrittsstatus zu &quot;wechseln&quot;, verwenden Sie die Funktion &quot;switch&quot; im Tab Allgemeine Funktionen .

1. Die Switch-Funktion verwendet den Fortschrittsstatus-Wert oder -Ausdruck als Schlüssel und gibt dann den Ausgabewert basierend auf diesem Schlüssel zurück.

   + Ein Schlüsselwert wird an der ersten Position nach dem Fortschrittsstatus (&quot;LT&quot;) definiert, wobei die entsprechende Ausgabe an der zweiten Position (&quot;Late&quot;) definiert wird.
   + Der nächste Schlüsselwert wird an der dritten Position definiert, wobei die entsprechende Ausgabe an der vierten Position etc. für beliebig viele Schlüssel definiert ist.

      ![Switch-Funktion Bild 2](../12-exercises/assets/switch-function-walkthrough-2.png)
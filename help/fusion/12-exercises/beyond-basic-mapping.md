---
title: Über die grundlegende Zuordnung hinaus
description: Erfahren Sie, wie Sie mit den Formeln des Zuordnungsbedienfelds Felder bearbeiten oder konvertieren können, die an ein Modul gesendet werden.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Über die grundlegende Zuordnung hinaus

Erfahren Sie, wie Sie mit den Formeln des Zuordnungsbedienfelds Felder bearbeiten oder konvertieren können, die an ein Modul gesendet werden.

## Übungsübersicht

Ändern Sie den Projektnamen, das geplante Startdatum und die Priorität in den exemplarischen Vorgehensweisen für &quot;Über die grundlegende Zuordnung&quot;unter Verwendung der Formeln des Zuordnungsbedienfelds.

![Jenseits des Basisbilds Bild 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

**Erstellen Sie einen Klon Ihres Designszenarios mit dem anfänglichen Szenario.**

1. Wählen Sie die Option Klonen rechts neben dem anfänglichen Szenario-Entwurf im Szenario-Abschnitt aus, wie unten dargestellt. Nennen Sie ihn &quot;Jenseits der grundlegenden Zuordnung&quot;.

   ![Jenseits des Grundlinienbilds 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Jetzt werden wir das Zuordnungsbedienfeld im Modul Workfront-Projekte erstellen verwenden, um den Projektnamen, das geplante Startdatum und die Prioritätsfelder zu konfigurieren.**

1. Klicken Sie auf das Modul Workfront-Projekte erstellen , um die Einstellungen zu bearbeiten. Ändern Sie im Zuordnungsfenster das Feld Name in &quot;[Mein Projektname] von [Sponsor].&quot;

   + Die [Mein Projektname] ist Spalte 1 des Analytics-CSV-Moduls und [Sponsor] ist Spalte 6. Das Wort &quot;by&quot; wird nur zwischen den beiden eingegeben.

1. Navigieren Sie als Nächstes zum geplanten Startdatum und verwenden Sie die Formel addDays , um dem Feld 15 Tage hinzuzufügen, wie im Video Beyond basic mapping Walkthrough beschrieben.
1. Suchen Sie das Feld Priorität und schalten Sie die Schaltfläche Zuordnung oben rechts im Feld ein. Das Menü der Auswahlliste ändert sich in eine Zahl. Erstellen Sie eine if -Anweisung, um ein Projekt mit der Priorität Hoch(4) zu kennzeichnen, wenn die CSV-Datei-Konfidenzbewertung kleiner als 100 ist. Andernfalls kann es sich um Normal(2) handeln.

   + Die Konfidenzbewertung ist in Spalte 4 enthalten.

   **An dieser Stelle sollte Ihr Zuordnungsbedienfeld wie folgt aussehen:**

   ![Jenseits des grundlegenden Zuordnungsbilds 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Klicken Sie auf OK und dann auf Ausführen einmal.
1. Suchen Sie das Projekt in Ihrer Workfront-Instanz, um sicherzustellen, dass alles korrekt zugeordnet wurde.
1. Speichern Sie Ihr Szenario.

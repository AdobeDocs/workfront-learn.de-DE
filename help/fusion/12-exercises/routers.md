---
title: Router
description: Machen Sie sich mit der Wichtigkeit von Routern vertraut und erfahren Sie, wie sie zur bedingten Verarbeitung verschiedener Module verwendet werden können.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11043
thumbnail: KT11043.png
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Router

Machen Sie sich mit der Wichtigkeit von Routern vertraut und erfahren Sie, wie sie zur bedingten Verarbeitung verschiedener Module verwendet werden können.

## Übungsübersicht

Verwenden Sie einen Router, um Pokemon oder Superhelden den richtigen Pfad zu übergeben und dann eine Aufgabe für jedes Zeichen zu erstellen.

![Router Image 1](../12-exercises/assets/routers-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Klonen Sie das Szenario Verwendung universeller Connectoren aus der vorherigen Übung. Nennen Sie es &quot;Erstellen verschiedener Pfade mithilfe von Routern&quot;.

   **Erstellen Sie einen neuen Pfad für Superhelden, indem Sie Module klonen und einen Router hinzufügen.**

   ![Router Image 2](../12-exercises/assets/routers-walkthrough-2.png)

1. Klicken Sie mit der rechten Maustaste auf das Infomodul Pokemon abrufen und wählen Sie Klon. Nachdem Sie geklont haben, ziehen Sie es und verbinden Sie es mit der Linie zwischen dem neuen HTTP-Modul und dem Parse CSV-Modul.

   >[!NOTE]
   >
   > Beachten Sie, wie automatisch ein Router mit zwei Pfaden hinzugefügt wird.

1. Nennen Sie dieses Modul &quot;Get superhero appearance&quot;.
1. Klonen Sie dieses Modul, bewegen Sie den Klon nach rechts und nennen Sie es &quot;Get superhero abilities&quot;.
1. Klonen Sie das Tool-Modul und verschieben Sie es an das Ende des zweiten Pfads.
1. Klicken Sie in der Symbolleiste auf das Zauberstab-Symbol - die Schaltfläche Automatisch ausrichten .

   **Ihr Szenario sollte wie folgt aussehen:**

   ![Router Image 3](../12-exercises/assets/routers-walkthrough-3.png)

   **Als Nächstes ändern Sie die zugeordneten Werte in den neuen geklonten Modulen.**

1. Navigieren Sie zu <https://www.superheroapi.com/> und verwenden Sie Ihr Facebook-Konto, um ein Zugriffstoken zu erhalten.

   >[!NOTE]
   >
   >Wenn Sie Probleme beim Zugriff auf Ihr eigenes Superhero-Token haben, können Sie dieses gemeinsam genutzte Token verwenden: 10110256647253588. Beachten Sie bitte, wie oft Sie die Superhero-API aufrufen, damit dieses gemeinsam genutzte Token für alle weiterhin funktioniert.

1. Öffnen Sie die Einstellungen für das Erscheinungsbild &quot;Get Superhero&quot;und ändern Sie die URL in `https://www.superheroapi.com/api/[access- token]/332/appearance`. Stellen Sie sicher, dass Sie Ihr Zugriffstoken in die URL aufnehmen. Klicken Sie auf OK.
1. Öffnen Sie die Einstellungen für &quot;Get Superhero&quot;-Fähigkeiten und ändern Sie die URL in `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Stellen Sie sicher, dass Sie Ihr Zugriffstoken in die URL aufnehmen. Klicken Sie auf OK.
1. Klicken Sie mit der rechten Maustaste auf jedes Superhero-Modul und wählen Sie Nur dieses Modul ausführen. Dadurch wird die Datenstruktur generiert, die Sie für die Zuordnung sehen müssen.
1. Nachdem Sie beide Seiten ausgeführt haben, ändern Sie die Zahl &quot;332&quot;in jedem URL-Feld in Spalte 4, die vom CSV-Modul Parsen zugeordnet ist.

   ![Routers Bild 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Jetzt können Sie in das Modul Mehrere Variablen festlegen im Superhero-Pfad klicken und den Namen, die Höhe, die Gewichtung und die Fähigkeiten aktualisieren.**

1. Aktualisieren Sie die Felder Name und Funktion im Modul Superheldenfähigkeiten abrufen - Modul 8.

   ![Bild 5 für Router](../12-exercises/assets/routers-walkthrough-5.png)

1. Aktualisieren Sie die Felder Höhe und Gewichtung im Modul Superhero-Erscheinungsbild abrufen - Modul 6.

   ![Router Image 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Wenn Sie fertig sind, sollten Ihre Variablen wie folgt aussehen. Beachten Sie, dass die Modulnummern in den Feldwerten angezeigt werden.**

   ![Router Image 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Klicken Sie auf OK und speichern Sie das Szenario.

   **Erstellen Sie einen weiteren Pfad, um eine Aufgabe pro Zeichen zu erstellen.**

1. Erstellen Sie in Workfront ein leeres Projekt. Nennen Sie es &quot;Versandmanifest-Projekt&quot;und kopieren Sie die Projekt-ID aus der URL.
1. Kehren Sie zu Workfront Fusion zurück und klicken Sie in der Mitte des Routers auf , um einen weiteren Pfad zu erstellen.

   ![Router Image 8](../12-exercises/assets/routers-walkthrough-8.png)

1. Klicken Sie in der Mitte des leeren Moduls, das angezeigt wird, und fügen Sie ein Datensatzmodul erstellen aus der Workfront-App hinzu.
1. Setzen Sie den Record Type auf Task und wählen Sie Projekt-ID aus dem Abschnitt Felder zur Zuordnung aus.
1. Fügen Sie die Projekt-ID, die Sie aus Workfront kopiert haben, in das Feld Projekt-ID ein.
1. Wählen Sie nun das Feld Name aus dem Abschnitt Zu zuordnende Felder aus.
1. Benennen Sie die Aufgabe &quot;[Zeichen] von [Franchise],&quot;wobei der Zeichenname und der Franchise-Name aus der CSV-Datei. Spalte 3 ist der Zeichenname und Spalte 2 der Name der Franchise.

   ![Router Image 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Klicken Sie auf OK und benennen Sie dieses Modul in &quot;Aufgabe für jedes Zeichen erstellen&quot;um.

   **Fügen Sie Filter hinzu, damit das Szenario fehlerfrei ausgeführt werden kann. Sie möchten, dass nur Pokemon-Zeichen in den oberen Pfad hinuntergehen, nur Superheldenzeichen in den mittleren Pfad und alle Zeichen in den unteren Pfad.**

1. Klicken Sie auf die gepunktete Zeile links neben dem Informationsmodul &quot;Get Pokemon&quot;, um den ersten Filter zu erstellen. Nennen Sie es &quot;Pokemon-Zeichen&quot;.
1. Für die Bedingung nur Datensätze zulassen, bei denen die Franchise (Spalte 2) gleich &quot;Pokemon&quot;ist. Wählen Sie den Operator &quot;Gleich&quot;aus.
1. Klicken Sie auf die gepunktete Linie links neben dem Erscheinungsbild-Modul &quot;Superhero abrufen&quot;, um den nächsten Filter zu erstellen. Nennen Sie es &quot;Superhero-Zeichen&quot;.
1. Da Superhelden aus verschiedenen Franchisen stammen können, verwenden Sie das Feld Superhero-ID (Spalte 4), um zu bestimmen, ob ein Zeichen ein Superheld ist oder nicht.

   **Die Filter sollten wie folgt aussehen:**

   ![Bild für Router 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Bild für Router 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Speichern Sie das Szenario und klicken Sie einmal auf Ausführen . Überprüfen Sie mithilfe der Ausführungsinspektoren, ob alle Vorgänge erfolgreich waren, und überprüfen Sie die Aufgaben, die in Ihrem Workfront-Projekt erstellt wurden.

   ![Bild für Router 12](../12-exercises/assets/routers-walkthrough-12.png)

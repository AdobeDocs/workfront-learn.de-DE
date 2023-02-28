---
title: Aufgabenbericht erstellen
description: In diesem Video erfahren Sie, wie Sie einen Aufgabenbericht mit einem komplexen Filter in Workfront erstellen und die von Ihnen erstellten Berichte finden. Aktivität – einen Notizbericht mit Eingabeaufforderungen erstellen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 11%

---

# Aufgabenbericht erstellen

In diesem Video erfahren Sie:

* Erstellen eines Aufgabenberichts mit einem komplexen Filter
* So finden Sie die erstellten Berichte

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12)

## Aktivität: Erstellen eines Berichts mit Eingabeaufforderungen

Erstellen Sie einen Hinweis -Bericht, mit dem Sie nach Benutzerhinweisen (d. h. Kommentaren oder Aktualisierungen) oder Systemnotizen suchen können, die auf dem Inhalt der Notiz, dem Autor, dem Eintragsdatum, dem Projektnamen oder dem Audittyp basieren. Nennen Sie den Bericht &quot;Notizsuche&quot;.

Bei Verwendung der Eingabeaufforderung Text notieren durchsucht dieser Bericht in Aktualisierungs-Threads, um schnell alle zu extrahieren, die die in den Eingabeaufforderungen angegebenen Kriterien erfüllen. Wenn Sie den Bericht ausführen, müssen Sie nicht jede Eingabeaufforderung ausfüllen, sondern nur die, die Ihnen wichtig sind. Die leeren werden automatisch ignoriert.

Die Ansicht sollte Spalten für Folgendes enthalten:

* Notizentext
* Text prüfen
* Eingabedatum
* Inhaber: Name
* Prüfungstyp
* Aufgabenname
* Name des Problems

Lassen Sie die Registerkarte Filter leer.

Gruppe für den Projektnamen.

Fügen Sie Aufforderungen für Folgendes ein:

* Text prüfen
* Notizentext
* Name des Inhabers
* Eingabedatum
* Projektname
* Prüfungstyp

## Antwort

1. Auswählen **[!UICONTROL Berichte]** von **[!UICONTROL Hauptmenü]**.
1. Klicken Sie auf **[!UICONTROL Neuer Bericht]** Menü und wählen Sie **[!UICONTROL Hinweis]**.
1. In **[!UICONTROL Spalten (Ansicht)]** Richten Sie Ihre Spalten so ein, dass Folgendes enthalten ist:

   ![Ein Bild des Bildschirms zur Erstellung von Berichtsspalten für Anmerkungen](assets/note-report-columns.png)

   * [!UICONTROL Hinweis] > [!UICONTROL Hinweis Text]
   * [!UICONTROL Hinweis] > [!UICONTROL Audit-Text]
   * [!UICONTROL Hinweis] > [!UICONTROL Entrydatum]
   * [!UICONTROL Inhaber] > [!UICONTROL Name]
   * [!UICONTROL Hinweis] > [!UICONTROL Audittyp]
   * [!UICONTROL Aufgabe] > [!UICONTROL Name]
   * [!UICONTROL Problem] > [!UICONTROL Name]

1. Wählen Sie die **[!UICONTROL Entrydatum]** und ändern Sie die **[!UICONTROL Nach Absteigend sortieren]**.
1. Im **[!UICONTROL Gruppierungen]** Registerkarte, den Bericht auf [!UICONTROL Projekt] > [!UICONTROL Name].

   ![Ein Bild des Bildschirms zur Erstellung von Berichtsgruppen für Anmerkungen](assets/note-report-groupings.png)

1. Urlaub [!UICONTROL Filter] leer.
1. Öffnen **[!UICONTROL Berichtseinstellungen]** und benennen Sie den Bericht &quot;Notizsuche&quot;.
1. Im [!UICONTROL Beschreibung] -Feld ein, z. B. &quot;Suchen Sie basierend auf dem ausgewählten Audittyp und anderen Eingabeaufforderungen nach System- oder Benutzernotizen. Systemnotizen werden in der Spalte &quot;Audit Text&quot;und Benutzerhinweise in der Spalte Hinweis Text angezeigt.&quot;

   ![Ein Bild des Bildschirms zur Erstellung der Berichtseinstellungen für Anmerkungen](assets/note-report-report-options.png)

1. Auswählen **[!UICONTROL Registerkarte &quot;Details&quot;]** sodass sie beim Laden des Berichts angezeigt wird.
1. Stellen Sie den Bericht so ein, dass 200 Elemente angezeigt werden, wenn der Bericht in ein Dashboard aufgenommen wird.
1. Klicken **[!UICONTROL Berichtsaufforderungen]** und fügen Sie Folgendes hinzu:

   ![Ein Bild des Bildschirms zur Erstellung von Meldeberichten](assets/note-report-report-prompts.png)

   * [!UICONTROL Hinweis] > [!UICONTROL Audit-Text]
   * [!UICONTROL Hinweis] > [!UICONTROL Hinweis Text]
   * [!UICONTROL Inhaber] > [!UICONTROL Name]
   * [!UICONTROL Hinweis] > [!UICONTROL Entrydatum]
   * [!UICONTROL Projekt] > [!UICONTROL Name]
   * [!UICONTROL Hinweis] > [!UICONTROL Audittyp]

1. Aktivieren Sie das Kontrollkästchen für **[!UICONTROL Anzeigen von Eingabeaufforderungen in Dashboards]**.
1. Speichern und schließen Sie den Bericht.

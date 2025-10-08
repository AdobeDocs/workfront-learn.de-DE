---
title: Erstellen von Berichten mit Diagrammen
description: Diagramme optimieren die Datenvisualisierung, indem sie Datenerkenntnisse durch anpassbare Filter, Gruppierungen und gestapelte Säulenformate organisieren, was eine übersichtlichere und besser umsetzbare Analyse ermöglicht.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
last-substantial-update: 2025-05-06T00:00:00Z
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: ht
source-wordcount: '595'
ht-degree: 100%

---

# Erstellen von Berichten mit Diagrammen

In diesem Video wird erläutert, wie Sie mithilfe von Diagrammen Daten auf effektive Weise visualisieren können, insbesondere zum Tracking von Projektaufgaben. Es zeigt die Erstellung von zwei Berichtstypen in Workfront:

**Bericht zu in Verzug geratenen Aufgaben nach Projekt:**

* Beginnen Sie mit einem Listenbericht und wenden Sie Filter an, um in aktuellen Projekten nur unvollständige, in Verzug geratene Aufgaben anzuzeigen. 
* Gruppieren Sie Aufgaben nach den Projektnamen und erstellen Sie ein Tortendiagramm, um die Verteilung in Verzug geratener Aufgaben auf die Projekte anzuzeigen. 
* Legen Sie das Diagramm als Standardregisterkarte fest, um einfachen Zugriff zu ermöglichen. 

**Bericht zu Aufgaben nach Projekt und Fortschrittsstatus:**

* Kopieren Sie den ersten Bericht und fügen Sie eine weitere Gruppierung für den Fortschrittsstatus der Aufgaben hinzu.
* Entfernen Sie Filter, um alle Aufgaben einzuschließen und ihren Fortschritt während der Projektausführung anzuzeigen.
* Verwenden Sie ein gestapeltes Säulendiagramm, um die Gesamtzahl der Aufgaben pro Projekt anzuzeigen, wobei die einzelnen Säulen für die verschiedenen Fortschrittsstatus stehen.
* Passen Sie bei Bedarf Farben an und speichern Sie den Bericht.

In diesem Video wird gezeigt, wie Diagramme, z. B. Torten- und gestapelte Säulendiagramme, Erkenntnisse zur Aufgabenverteilung und Projektleistung liefern und so Benutzende Projekte vergleichen und den Aufgabenfortschritt visuell nachvollziehen können. 

>[!VIDEO](https://video.tv.adobe.com/v/3450023/?quality=12&learn=on&captions=ger)

## Die wichtigsten Punkte

* **Mehr Datenklarheit durch Diagramme**: Durch die Visualisierung von Daten mit Diagrammen, z. B. Torten- oder Säulendiagrammen, können sowohl die Aufgabenverteilung als auch der Projektfortschritt im Vergleich zu Listenberichten einfacher nachvollzogen werden. 
* **Filterung nach bestimmten Erkenntnissen**: Die Anwendung von Filtern (z. B. für in aktuellen Projekten unvollständige, in Verzug geratene Aufgaben) ermöglicht es, sich für eine zielgerichtete Analyse auf relevante Daten zu konzentrieren. 
* **Gruppierung für eine bessere Organisation**: Durch Gruppierung von Aufgaben nach dem Projektnamen oder Fortschrittsstatus werden Daten effektiv organisiert, was aussagekräftige Vergleiche zwischen den Projekten ermöglicht. 
* **Optionen zur Diagrammanpassung**: Benutzende können Diagrammtypen (z. B. Torten-, Säulen- und Balkendiagramme) auswählen und Farben anpassen, um sie an Voreinstellungen oder das Branding anzupassen. 
* **Gestapelte Säulendiagramme für detaillierte Erkenntnisse**: Gestapelte Säulendiagramme bieten eine umfassende Ansicht des Aufgabenfortschritts innerhalb von Projekten, wobei sowohl die Gesamtzahl der Aufgaben als auch deren Status in einer einzigen Visualisierung angezeigt werden.


## Aktivitäten zum Erstellen von Berichten mit Diagrammen

### Aktivität 1: Hinzufügen eines Diagramms zu einem Bericht

Das Quartalsende naht, und Sie möchten sehen, inwieweit die kürzlich abgeschlossenen Projekte ihr Budget eingehalten haben. Erstellen Sie einen Bericht, der die geplanten Kosten im Vergleich zu den tatsächlichen Kosten für Projekte zeigt. Sie möchten nur die Projekte sehen, die im letzten Quartal abgeschlossen wurden. Fügen Sie ein Diagramm mit einer Kombination von Spalten hinzu, das benutzerdefinierte Farben verwendet.

### Antwort 1

1. Wählen Sie **[!UICONTROL Berichte]** aus dem **[!UICONTROL Hauptmenü]** aus.
1. Klicken Sie auf das Menü **[!UICONTROL Neuer Bericht]** und wählen Sie **[!UICONTROL Projekt]** aus.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Spalten (Ansicht)]** und dann auf **[!UICONTROL Spalte hinzufügen]**.
1. Wählen Sie [!UICONTROL Projekt] > [!UICONTROL Geplante Kosten] aus und fassen Sie diese Spalte mit **[!UICONTROL Summieren]** zusammen.
1. Klicken Sie erneut auf **[!UICONTROL Spalte hinzufügen]**.
1. Wählen Sie [!UICONTROL Projekt] > [!UICONTROL Tatsächliche Kosten] aus und fassen Sie diese Spalte mit **[!UICONTROL Summieren]** zusammen.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Spalten zu einem Bericht](assets/chart-report-columns.png)

1. Legen Sie auf der Registerkarte **[!UICONTROL Gruppierungen]** fest, dass der Bericht nach [!UICONTROL Projekt] > [!UICONTROL Name] gruppiert werden soll.

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Gruppierungen zu einem Bericht](assets/chart-report-groupings.png)

1. Fügen Sie auf der Registerkarte **[!UICONTROL Filter]** zwei Filterregeln hinzu:

   * [!UICONTROL Projekt] > [!UICONTROL Status entspricht] > [!UICONTROL Abgeschlossen]
   * [!UICONTROL Projekt] > [!UICONTROL Tatsächliches Abschlussdatum] > [!UICONTROL Letztes Quartal]

   ![Ein Screenshot des Bildschirms zum Hinzufügen von Filtern zu einem Bericht](assets/chart-report-filters.png)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Diagramm]** die Option **[!UICONTROL Spalte]** für den Diagrammtyp aus.
1. Wählen Sie unter [!UICONTROL Linke Achse (Y)] die Option [!UICONTROL Geplante Kosten] aus.
1. Wählen Sie unter [!UICONTROL Untere Achse (X)] die Option [!UICONTROL Name] aus.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Kombinationsdiagramm]** und wählen Sie im Feld **[!UICONTROL Wert]** die Option [!UICONTROL Ist-Kosten] aus.
1. Wählen Sie im Feld **[!UICONTROL Diagrammtyp]** die Option für das Liniendiagramm aus.
1. Klicken Sie auf das Farbfeld, um die Farbe für die [!UICONTROL Ist-Kosten] zu ändern. Wählen Sie eine Farbe aus.
1. Klicken Sie auf **[!UICONTROL Speichern + schließen]**. Wenn Sie zur Eingabe eines Berichtnamens aufgefordert werden, nennen Sie ihn „Geplante vs. tatsächliche Kosten nach abgeschlossenem Projekt im letzten Quartal“.

   ![Ein Screenshot des Bildschirms zum Hinzufügen eines Diagramms zu einem Bericht](assets/chart-report-chart.png)

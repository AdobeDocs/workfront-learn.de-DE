---
title: Verstehen mehrerer Abrechnungsraten
description: Innerhalb von Workfront kann ein Projektmanager die Abrechnungsraten des Systems innerhalb eines bestimmten Projekts außer Kraft setzen.
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Verstehen mehrerer Abrechnungsraten

Within [!DNL Workfront], kann ein Projektmanager die Abrechnungsraten des Systems innerhalb eines bestimmten Projekts außer Kraft setzen. Früher hatte die Anwendung der neuen Abrechnungsrate auf das Projekt nicht nur Auswirkungen auf zukünftige Stunden, sondern auch auf bereits im Projekt angemeldete Stunden.

Mit [!DNL Workfront]Dank der neuen Funktion für mehrere Abrechnungsraten kann der Projektmanager entscheiden, welchen Zeitraum ein Abrechnungskurs angewendet werden soll. Auf diese Weise kann der Projektmanager festlegen, wann dieser Satz wirksam werden soll, wenn ein Kurs ausgehandelt oder geändert wurde.

## Ändern der Abrechnungsrate

1. Rufen Sie die Landingpage des Projekts auf. Auswählen **[!UICONTROL Abrechnungssätze]** aus dem linken Bereich.

   ![Bild der Auswahl [!UICONTROL Abrechnungssätze] in [!DNL Workfront]](assets/project-finances-1.png)

1. Aus dem **[!UICONTROL Abrechnungssätze]** klicken Sie auf die **[!UICONTROL Abrechnungsrate hinzufügen]** Schaltfläche. Auswählen **[!UICONTROL Neuer Abrechnungskurs]** aus dem Dropdown-Menü aus.

   ![Bild der Auswahl [!UICONTROL Neuer Abrechnungskurs] in [!DNL Workfront]](assets/project-finances-2.png)

1. Die [!UICONTROL Neuer Abrechnungskurs] angezeigt. Aus dem **[!UICONTROL Auftragsrolle]** Dropdown-Liste die Auftragrolle auswählen, auf die der neue Abrechnungskurs angewendet werden soll.

   ![Ein Bild von der Auswahl von Vorgangsrollen in einer neuen Abrechnungsrate in [!DNL Workfront]](assets/project-finances-3.png)

1. Nach Auswahl der Auftragsrolle wird die [!UICONTROL Standardabrechnungsrate] und [!UICONTROL Abrechnungskurs 1] angezeigt. Geben Sie den neuen Abrechnungskurs in das Feld [!UICONTROL Abrechnungskurs 1] -Feld. Wenn dieser Abrechnungskurs für das gesamte Projekt gilt (vergangene, aktuelle und zukünftige Stunden protokolliert), klicken Sie auf die **[!UICONTROL Speichern]** Schaltfläche.

   ![Ein Bild vom Speichern einer neuen Abrechnungsrate, die für das gesamte Projekt in gilt [!DNL Workfront]](assets/project-finances-5.png)

1. Wenn der neue Abrechnungskurs nur für einen bestimmten Zeitraum gilt, klicken Sie auf die **[!UICONTROL Rate hinzufügen]** Schaltfläche. Die [!UICONTROL Abrechnungsrate 1 Enddatum] und [!UICONTROL Abrechnungskurs 2] werden angezeigt. Enddatum eingeben für [!UICONTROL Abrechnungskurs 1]. Sie können kein Startdatum eingeben für [!UICONTROL Abrechnungskurs 1] weil das System davon ausgeht, dass es zu Beginn des Projekts gestartet wurde.

   ![Ein Bild vom Erstellen einer neuen Abrechnungsrate, die für einen bestimmten Zeitraum gilt, beginnend mit dem Beginn des Projekts in [!DNL Workfront]](assets/project-finances-6.png)

1. Wenn dies nicht der Fall ist:

   * Standardabrechnungsrate eingeben für [!UICONTROL Abrechnungskurs 1].
   * Enddatum auswählen für [!UICONTROL Abrechnungskurs 1] ([!UICONTROL Standardabrechnungsrate]).
   * Das Startdatum für [!UICONTROL Abrechnungskurs 2] wird automatisch auf den folgenden Tag eingestellt [!UICONTROL Abrechnungskurs 1] endet.
   * Geben Sie die gewünschte Abrechnungsrate in das Feld [!UICONTROL Abrechnungskurs 2] Abschnitt.
   * Fügen Sie nach Bedarf weitere Abrechnungssätze hinzu, indem Sie auf die Schaltfläche **[!UICONTROL Rate hinzufügen]** Schaltfläche.
   * Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.
   * Alle Abrechnungssätze werden im [!UICONTROL Abrechnungssätze] im Projekt.
   ![Ein Bild von der Erstellung neuer Abrechnungssätze, die für die verschiedenen Zeiträume in [!DNL Workfront]](assets/project-finances-7.png)

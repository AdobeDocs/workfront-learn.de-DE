---
title: Grundlegendes zu mehrfachen Abrechnungstarifen
description: Erfahren Sie, wie Sie die Abrechnungsrtarife des Systems innerhalb eines Projekts überschreiben.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
exl-id: 5b1ae2c4-43bd-4382-900f-078ef84408a5
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:00:23.025Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 93%

---

# Grundlegendes zu mehrfachen Abrechnungstarifen

Innerhalb von [!DNL Workfront] haben Projekt-Managerinnen und -Manager die Möglichkeit, die Abrechnungstarife des Systems innerhalb eines bestimmten Projekts außer Kraft zu setzen. Früher hatte die Anwendung des neuen Abrechnungstarifs auf das Projekt nicht nur Auswirkungen auf zukünftige Stunden, sondern auch auf bereits im Projekt angemeldete Stunden.

Mit der neuen Funktion für mehrere Abrechnungssätze von [!DNL Workfront] kann der Projekt-Manager entscheiden, in welchem Zeitraum ein Abrechnungssatz angewendet werden soll. Auf diese Weise können Projekt-Managerinnen und -Manager festlegen, wann dieser Tarif wirksam werden soll, wenn ein Tarif ausgehandelt oder geändert wurde.

## Ändern des Abrechnungstarifs

1. Navigieren Sie zur Landingpage des Projekts. Wählen Sie **[!UICONTROL Abrechnungstarife]** im linken Bedienfeld.

   ![Ein Bild der Auswahl der [!UICONTROL Abrechnungstarife] in [!DNL Workfront]](assets/project-finances-1.png)

1. Klicken Sie auf der Registerkarte **[!UICONTROL Abrechnungstarife]** auf die Schaltfläche **[!UICONTROL Abrechnungstarif hinzufügen]**. Wählen Sie **[!UICONTROL Neuer Abrechnungstarif]** aus dem Dropdown-Menü aus.

   ![Bild der Auswahl eines [!UICONTROL neuen Abrechnungstarifs] in [!DNL Workfront]](assets/project-finances-2.png)

1. Das Dialogfeld [!UICONTROL Neuer Abrechnungstarif] wird angezeigt. Wählen Sie in der Dropdown-Liste **[!UICONTROL Aufgabengebiet]** das Aufgabengebiet, auf das der neue Abrechnungstarif angewendet werden soll.

   ![Ein Bild der Auswahl von Aufgabengebieten in einem neuen Abrechnungstarif in [!DNL Workfront]](assets/project-finances-3.png)

1. Sobald das Aufgabengebiet ausgewählt ist, erscheinen die Felder [!UICONTROL Standardabrechnungstarif] und [!UICONTROL Abrechnungstarif 1]. Geben Sie den neuen Abrechnungstarif in das Feld [!UICONTROL Abrechnungstarif 1] ein. Wenn dieser Abrechnungstarif für das gesamte Projekt gilt (vergangene, aktuelle und zukünftige protokollierte Stunden), klicken Sie auf die Schaltfläche **[!UICONTROL Speichern]**.

   ![Ein Bild vom Speichern eines neuen Abrechnungstarifs, der für das gesamte Projekt in [!DNL Workfront]](assets/project-finances-5.png) gilt

1. Wenn der neue Abrechnungstarif nur für einen bestimmten Zeitraum gilt, klicken Sie auf die Schaltfläche **[!UICONTROL Abrechnungstarif hinzufügen]**. Die Felder [!UICONTROL Abrechnungstarif 1 Enddatum] und [!UICONTROL Abrechnungstarif 2] erscheinen. Geben Sie das Enddatum für [!UICONTROL Abrechnungstarif 1] ein. Sie können kein Startdatum für [!UICONTROL Abrechnungstarif 1] eingeben, weil das System davon ausgeht, dass er zu Beginn des Projekts begonnen hat.

   ![Ein Bild zur Erstellung eines neuen Abrechnungstarifs, der für einen bestimmten Zeitraum gilt, beginnend mit dem Beginn des Projekts in [!DNL Workfront]](assets/project-finances-6.png)

1. Wenn dies nicht der Fall ist:

   * Geben Sie den Standardabrechnungstarif für [!UICONTROL Abrechnungstarif 1] ein.
   * Wählen Sie das Enddatum für [!UICONTROL Abrechnungstarif 1] aus ([!UICONTROL Standardabrechnungstarif]).
   * Das Startdatum für [!UICONTROL Abrechnungstarif 2] wird automatisch auf den folgenden Tag eingestellt, nachdem [!UICONTROL Abrechnungstarif 1] endet.
   * Geben Sie den gewünschten Abrechnungstarif in den Abschnitt [!UICONTROL Abrechnungstarif 2] ein.
   * Fügen Sie nach Bedarf weitere Abrechnungstarife hinzu, indem Sie auf die Schaltfläche **[!UICONTROL Tarif hinzufügen]** klicken.
   * Klicken Sie abschließend auf **[!UICONTROL Speichern]**.
   * Alle Abrechnungstarife werden in der Registerkarte [!UICONTROL Abrechnungstarife] im Projekt angezeigt.

   ![Ein Bild der Erstellung neuer Abrechnungstarife, die für verschiedene Zeiträume in [!DNL Workfront]](assets/project-finances-7.png) gelten

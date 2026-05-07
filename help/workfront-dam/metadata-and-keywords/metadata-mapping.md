---
title: Einrichten der Metadatenzuordnung
description: Erfahren Sie, wie Sie die Metadatenzuordnung für [!UICONTROL Workfront DAM] einrichten.
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 100%

---

# Einrichten der Metadatenzuordnung

[!DNL Workfront]-bezogene Informationen über ein Asset können zusammen mit dem Asset von [!DNL Workfront] in [!UICONTROL Workfront DAM] übertragen werden. Die Option für die Metadatenzuordnung im Bereich [!DNL Workfront] [!UICONTROL Setup] ermöglicht diese Übertragung von Informationen.

Wenden Sie sich an Ihre [!DNL Workfront]-Beraterin bzw. Ihren -Berater, um Empfehlungen zu Best Practices für die Einrichtung der Metadatenzuordnung zu erhalten.

Sie müssen [!DNL Workfront]-Admin und [!UICONTROL Workfront DAM]-Admin sein, um eine Metadatenzuordnung einzurichten. Bevor Sie beginnen können, müssen Sie Ihre [!DNL Workfront]- und [!UICONTROL Workfront DAM]-Konten verbinden.

## Konten verbinden

1. Melden Sie sich bei [!DNL Workfront] an.
1. Öffnen Sie ein Projekt, eine Aufgabe oder ein Problem und klicken Sie auf die Registerkarte **[!UICONTROL Dokumente]**.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Neu hinzufügen]** und wählen Sie im Dropdown-Menü **[!UICONTROL Aus Workfront DAM]**.
1. Geben Sie Ihren Anmeldenamen und Ihr Kennwort in das [!UICONTROL Workfront DAM]-Autorisierungsfeld ein, das erscheint.
1. Klicken Sie anschließend auf **[!UICONTROL Ja]**, um [!DNL Workfront] Zugriff auf das [!UICONTROL DAM]-Konto zu gewähren.
1. Aktualisieren Sie bei Bedarf die Seite, um den Zugriff auf [!UICONTROL Workfront DAM] zu aktualisieren.

Wenn diese Verbindung hergestellt ist, können Sie mit der Metadatenzuordnung zwischen den beiden Systemen beginnen. Stellen Sie sicher, dass Sie die benötigten Metadatenfelder in [!UICONTROL Workfront DAM] bereits erstellt haben, bevor Sie mit der Zuordnung beginnen.

## Einrichten der Zuordnung

1. Melden Sie sich bei [!DNL Workfront] an.
1. Wählen Sie **[!UICONTROL Setup]** im [!UICONTROL Hauptmenü].
1. Erweitern Sie den Abschnitt **[!UICONTROL Dokumente]** im Menü des linken Bedienfelds.
1. Klicken Sie anschließend auf **[!UICONTROL Metadatenzuordnung]**.
1. Geben Sie in das Workfront-Feld die Feldquelle des [!DNL Workfront]-Feldes ein, das Sie zuordnen möchten.
1. Wählen Sie dann das entsprechende oder gewünschte **[!UICONTROL Workfront DAM]**-Metadatenfeld aus.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zuordnung hinzufügen]**.
1. Im Diagramm unten im Fenster sehen Sie das [!UICONTROL Workfront-Feldquelle] und [!UICONTROL Workfront DAM-Zielfeld].
1. Wiederholen Sie diese Schritte für alle gewünschten Metadatenfelder.

![Screenshot des Bildschirms [!UICONTROL Metadatenzuordnung] in [!DNL Workfront]](assets/01-metadata-mapping.png)

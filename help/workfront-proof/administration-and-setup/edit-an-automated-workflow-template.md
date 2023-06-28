---
title: Automatisierte Workflow-Vorlage bearbeiten
description: Erfahren Sie, wie Sie Änderungen an einer vorhandenen automatisierten Testversand-Workflow-Vorlage vornehmen können in [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
jira: KT-8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Automatisierte Workflow-Vorlage bearbeiten

Da die Prüfungs- und Validierungsprozesse für Testsendungen verfeinert oder organisatorische Änderungen vorgenommen werden, sollten die automatisierten Workflow-Vorlagen aktualisiert werden, um die aktuellen Vorgänge für Ihre Teams mit Workfront widerzuspiegeln.

Durch die Aktualisierung von Vorlagen wird die Konsistenz Ihrer Prüfungs- und Validierungsprozesse sichergestellt und die Zeit für die Testversand-Upload-Benutzer wird gespart, da sie einen Workflow nicht ständig anpassen müssen.

1. Auswählen **[!UICONTROL Testversand]** von **[!UICONTROL Hauptmenü]** in [!DNL Workfront].
1. Wählen Sie dort die Option **[!UICONTROL Workflows]** im Menü des linken Bedienfelds.
1. Klicken Sie auf das Menü mit den 3 Punkten rechts neben dem Vorlagennamen und wählen Sie **[!UICONTROL Vorlagendetails anzeigen]**.

Die Optionen zum Freigeben, Kopieren und Löschen der Vorlage befinden sich oben im Fenster mit den Vorlagendetails für jede Vorlage. Das Löschen einer Vorlage wirkt sich nicht auf laufende Testsendungen aus, auf die diese Vorlage angewendet wird. Das bedeutet jedoch, dass die Vorlage nicht mehr verwendet werden kann.

![Fenster &quot;Vorlagendetails&quot;](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Klicken Sie auf den Pfeil, um den [!UICONTROL Details] -Abschnitt, um Elemente wie den Vorlagennamen oder die Zeitzone der Vorlage zu ändern.

## Vornehmen von Änderungen an Bühnen und Empfängern

Möglicherweise sind Änderungen im [!UICONTROL Workflow] Bereich, in dem ein optimierter Prozess eine frühere Frist bedeutet oder wenn jemand dem Team beitritt und Testsendungen überprüft.

Jede Etappe eines automatisierten Workflows verfügt über einen eigenen Abschnitt, in dem Termine, Datenschutz, Testversand-Empfänger und andere Informationen unabhängig voneinander geändert werden können.

In diesem Video werden kurz einige der Änderungen vorgestellt, die Sie im [!UICONTROL Workflow] Bereich. Sehen Sie sich die Liste mit Aufzählungszeichen unter diesem Video an, in der Sie diese Einstellungen überprüfen. In diesem Video gibt es kein Audio.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12&learn=on)

Im Folgenden finden Sie die Änderungen an der Testversandvorlage, die Sie in der [!UICONTROL Workflow] Abschnitt:

* Klicken Sie in die [!UICONTROL Staging-Name] oder [!UICONTROL deadline] -Feld, um diese Informationen zu aktualisieren.
* Wählen Sie den Pfeil neben dem [!UICONTROL deadline] um die Bühne zu sperren, zu bestimmen, wann die Bühne aktiviert ist, oder nur eine Entscheidung erforderlich.
* Klicken Sie in der Empfängerliste auf die Schaltfläche [!UICONTROL Rolle] oder [!UICONTROL E-Mail-Warnungen] -Felder, um eine andere Option auszuwählen.
* Gehen Sie zum Menü mit den drei Punkten rechts neben dem Namen eines Empfängers, um ihn aus der Liste zu löschen, ihn zur wichtigsten Entscheidungsfindung für diese Workflow-Phase zu machen oder die Rolle des Testversands und die E-Mail-Warnhinweisinformationen zu bearbeiten.
* Sie haben zwei Möglichkeiten, Empfänger zur Liste hinzuzufügen. Sobald Sie die [!UICONTROL Hinzufügen von Personen zur Bühne] -Fenster klicken Sie auf die Phase, der sie hinzugefügt werden sollen. Geben Sie dann ihren Namen oder ihre E-Mail-Adresse in die Empfängerliste ein und weisen Sie eine Testversand-Rolle und eine E-Mail-Warnung zu. Klicken Sie auf [!UICONTROL Personen hinzufügen] klicken, wenn Sie fertig sind.
   1. Navigieren Sie oben rechts in jedem Abschnitt zur [!UICONTROL Mehr] Menü und wählen Sie [!UICONTROL Hinzufügen von Personen zur Bühne].
   1. Oben im [!UICONTROL Workflow] Bereich, auswählen [!UICONTROL Hinzufügen von Personen zur Bühne].

## Vorlagenfreigabe

Die [!UICONTROL Freigegeben für] zeigt die Testversand-Benutzer an, die die Vorlage verwenden können. Entfernen Sie Personen, die die Vorlage nicht mehr benötigen, indem Sie auf das Menü mit den 3 Punkten rechts neben ihrem Namen klicken und [!UICONTROL Entfernen].

![[!UICONTROL Freigegeben für] Liste](assets/proof-system-setups-edit-template-shared-with.png)

Sie können in diesem Abschnitt jedoch keine Personen zur Freigabeliste hinzufügen. Gehen Sie dazu oben im Fenster mit den Vorlagendetails zurück und klicken Sie auf die Schaltfläche [!UICONTROL Vorlage freigeben] Schaltfläche.

## Aktivitätsabschnitt

[!DNL Workfront] speichert einen Prüfverlauf darüber, wann Änderungen an der Vorlage vorgenommen wurden. Sie können das Datum, wer die Änderung vorgenommen hat und einige kurze Informationen darüber sehen, welche Änderungen vorgenommen wurden.

In diesem Abschnitt werden keine Informationen darüber aufgezeichnet, wann die Vorlage für Testsendungen verwendet wurde.

![Aktivitätenliste des Testversands](assets/proof-system-setups-edit-template-activity.png)

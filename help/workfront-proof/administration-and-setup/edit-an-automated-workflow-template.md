---
title: Bearbeiten einer automatisierten Workflow-Vorlage
description: Erfahren Sie, wie Sie in [!DNL  Workfront]Änderungen an einer bestehenden Vorlage für einen automatisierten Proofing-Workflow vornehmen können.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
last-substantial-update: 2024-08-08T00:00:00Z
jira: KT-8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: 55edb8b797583f93f405c9c6b69422b818c90cdc
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 61%

---

# Bearbeiten einer automatisierten Workflow-Vorlage

Wenn Prüf- und Genehmigungsprozesse für Korrekturabzüge präzisiert oder organisatorische Änderungen vorgenommen werden, sollten die automatisierten Workflow-Vorlagen aktualisiert werden, um die aktuellen Abläufe in Ihren Teams widerzuspiegeln, die Workfront verwenden.

Durch die Aktualisierung von Vorlagen wird die Konsistenz Ihrer Überprüfungs- und Validierungsprozesse sichergestellt und die Zeit für die Testversand-Upload-Benutzer wird gespart, da sie einen Workflow nicht ständig anpassen müssen.

1. Wählen Sie **[!UICONTROL Proofing]** aus dem **[!UICONTROL Hauptmenü]** in [!DNL Workfront] aus.
1. Wählen Sie dort im Menü des linken Bedienfelds **[!UICONTROL Workflows]** aus.
1. Klicken Sie auf das Drei-Punkte-Menü ganz rechts neben dem Namen der Vorlage und wählen Sie **[!UICONTROL Vorlagendetails anzeigen]** aus.

Die Optionen zum Freigeben, Kopieren und Löschen der Vorlage befinden sich am oberen Rand des Fensters mit den Vorlagendetails für jede Vorlage. Das Löschen einer Vorlage wirkt sich nicht auf laufende Testsendungen aus, auf die diese Vorlage angewendet wird. Das bedeutet jedoch, dass die Vorlage nicht mehr verwendet werden kann.

![Fenster mit Vorlagendetails](assets/proof-system-setup-edit-templates-details-area.png)


Klicken Sie auf den Pfeil links neben dem Wort &quot;[!UICONTROL Details]&quot;, um den Abschnitt zu erweitern oder zu reduzieren.

## Vornehmen von Änderungen an Abschnitten und Empfängerinnen bzw. Empfängern

Änderungen können im Bereich [!UICONTROL Workflow] erforderlich sein, wenn ein gestraffter Prozess einen früheren Abgabetermin bedeutet oder wenn jemand zum Team stößt und die Korrekturabzüge überprüfen wird.

Jeder Schritt eines automatisierten Workflows hat seinen eigenen Bereich, in dem Fristen, Datenschutz, Empfängerinnen und Empfänger von Korrekturabzügen und andere Informationen unabhängig voneinander geändert werden können.

In diesem Video werden einige der Änderungen vorgestellt, die Sie im Bereich [!UICONTROL Workflow] vornehmen können. Sehen Sie sich die Liste mit Aufzählungszeichen unter diesem Video an, in der Sie diese Einstellungen überprüfen.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12&learn=on)

Im Folgenden finden Sie eine Übersicht über die Änderungen, die Sie an der Korrekturabzug-Vorlage im Abschnitt [!UICONTROL Workflow] vornehmen können:

* Klicken Sie in das Feld für den Staging-Namen oder in das Feld für den Termin, um diese Informationen zu aktualisieren.
* Klicken Sie auf den Pfeil links neben dem Termin, um die Phase zu sperren, zu bestimmen, wann die Phase aktiviert wird, oder nur eine Entscheidung erforderlich zu machen.
* Klicken Sie in der Empfängerliste in die Felder [!UICONTROL Rolle] oder [!UICONTROL E-Mail-Warnmeldungen], um eine andere Option auszuwählen.
* Öffnen Sie das Menü mit den drei Punkten ganz rechts neben dem Namen eines Empfängers, um ihn aus der Liste zu löschen, ihn zur wichtigsten Entscheidungsfindung für diese Workflow-Phase zu machen oder bearbeiten Sie die Rolle &quot;Testversand&quot;und die E-Mail-Warnhinweisinformationen.
* Sie haben zwei Möglichkeiten, Empfänger zur Liste hinzuzufügen.
   1. Wechseln Sie oben rechts in jedem Schritt zum Menü [!UICONTROL Mehr] und wählen Sie [!UICONTROL Personen zur Bühne hinzufügen] aus. Nachdem Sie das Fenster [!UICONTROL Personen zur Bühne hinzufügen] geöffnet haben, klicken Sie auf die Bühne, der Sie Personen hinzufügen möchten. Geben Sie dann den Namen oder die E-Mail-Adresse der Person in die Empfängerliste ein und weisen Sie ihr eine Korrekturabzug-Rolle und eine E-Mail-Warnmeldung zu. Klicken Sie auf die Schaltfläche [!UICONTROL Personen hinzufügen] , wenn Sie fertig sind.
   1. Wählen Sie oben im Bereich [!UICONTROL Workflow] die Option [!UICONTROL Personen zum Schritt hinzufügen] aus.

## Freigeben von Vorlagen

Der Bereich [!UICONTROL Freigegeben für] zeigt die Benutzenden eines Korrekturabzugs an, die die Vorlage verwenden können. Entfernen Sie Personen, die die Vorlage nicht mehr benötigen, indem Sie auf das Drei-Punkte-Menü ganz rechts neben ihrem Namen klicken und [!UICONTROL Entfernen] auswählen.

Liste ![[!UICONTROL Freigegeben für]](assets/proof-system-setups-edit-template-shared-with.png)

In diesem Bereich können Sie jedoch keine Personen zur Freigabeliste hinzufügen. Gehen Sie dazu zurück an den oberen Rand des Fensters mit den Vorlagendetails und klicken Sie auf die Schaltfläche [!UICONTROL Vorlage freigeben].

## Weitere Informationen

[!DNL Workfront] führt ein Protokoll darüber, wann Änderungen an der Vorlage vorgenommen wurden. Sie können das Datum sehen, wer die Änderung vorgenommen hat und einige kurze Informationen über die vorgenommenen Änderungen.

In diesem Abschnitt werden keine Informationen darüber gespeichert, wann die Vorlage für Korrekturabzüge verwendet wurde.

![Aktivitätsliste eines Korrekturabzugs](assets/proof-system-setups-edit-template-activity.png)

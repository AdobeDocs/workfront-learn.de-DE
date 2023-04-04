---
title: Hochladen eines Testversands mit einem automatisierten Workflow
description: Erfahren Sie, wann ein Workflow für einen automatisierten Testversand verwendet werden soll, wie ein Workflow mit einer Testversand-Vorlage angewendet werden kann und wie ein automatisierter Workflow von Grund auf eingerichtet wird.
activity: use
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335133.png
kt: 8833
exl-id: 8301ef00-1f47-4779-aa35-c735b66fdcac
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Hochladen eines Testversands mit einem automatisierten Workflow

In diesem Video erfahren Sie:

* Verwendung eines automatisierten Testversand-Workflows
* Anwenden eines Workflows mithilfe einer Testversand-Vorlage
* So richten Sie einen automatisierten Workflow von Grund auf neu ein

>[!VIDEO](https://video.tv.adobe.com/v/335133/?quality=12&learn=on)



## Zusätzliche Workflow-Einstellungen für Testsendungen

Die Einstellungen am unteren Rand des Fensters zum Hochladen von Testsendungen sind optional. Fragen Sie daher Ihre Organisation nach, ob und wie Sie diese verwenden.

![Ein Bild der [!UICONTROL Neuer Testversand ]mit dem [!UICONTROL Staging-Einstellungen] hervorgehoben.](assets/additional-proof-workflow-settings.png)

* **[!UICONTROL Bühne sperren] —** Dadurch wird verhindert, dass Personen in dieser Workflow-Phase Kommentare abgeben oder Entscheidungen ändern, nachdem ihre Workflow-Phase abgeschlossen ist.
* **[!UICONTROL Übertragen der Rechte der primären Entscheidung an] —** Beschleunigen Sie den Testversand, indem Sie einen primären Entscheidungsträger bestimmen. Wenn festgelegt, [!DNL Workfront] erkennt die Beweisentscheidung dieser Person als Entscheidung AN. Sobald diese Person ihre Entscheidung trifft, ist die Bühne vorbei und es sind keine weiteren Entscheidungen erforderlich.
* **[!UICONTROL Nur eine Entscheidung für diese Phase anfordern] —** Eine andere Möglichkeit, den Testversand zu optimieren, besteht darin, nur eine Entscheidung über den Testversand zu verlangen. Wenn diese Option aktiviert ist, ist diese Phase abgeschlossen, unabhängig davon, wie viele Genehmiger Sie in dieser Phase haben, sobald einer von ihnen eine Entscheidung trifft.
* **[!UICONTROL Machen Sie diese Phase privat] —** Kommentare zum Testversand sind standardmäßig für alle Beteiligten in allen Phasen sichtbar. Verhindern Sie Empfängern von Testsendungen, während dieser Phase Kommentare zu sehen, indem Sie auf das entsprechende Kästchen klicken.

Am unteren Rand des Fensters zum Hochladen von Testsendungen befinden sich verschiedene Testversandeinstellungen, die sich auf die Sicherheit Ihres Testversands auswirken, z. B. die Notwendigkeit, sich zum Anzeigen des Testversands anzumelden.

<!--
Learn more about these in the Proof settings section of the Configure a proof article.
-->

![Ein Bild der [!UICONTROL Testversandeinstellungen] Abschnitt des Fensters zum Testversand-Upload.](assets/additional-proof-workflow-settings-2.png)

<!--
### Learn more
* Automated workflow overview
* Automated workflow stages overview
-->

<!--
### Guides
* Plan an advanced workflow worksheet
-->

## Warum befinden Sie sich im Testversand-Workflow?

Sie werden feststellen, dass Sie sich auf der Liste der Testversand-Empfänger befinden, da Sie die Testversand-Zielgruppe hochladen. Dadurch erhalten Sie auch die Berechtigung zum Testversand, sodass Sie u. a. die Workflow-Setups ändern oder eine neue Version hochladen können.

![Ein Bild des Fensters zum Hochladen des Testversands, in dem der Besitzer des Testversands in der Empfängerliste hervorgehoben ist.](assets/proof-owner.png)

Wenn Sie nur den Testversand hochladen, der Workflow jedoch von einer anderen Person verwaltet wird, können Sie den Testversand-Besitzer durch Auswahl von [!UICONTROL Inhaber] und geben Sie ihren Namen ein. Dies wird empfohlen, wenn andere Personen als der ursprüngliche Uploader eine Version hochladen.

## Ihre Wendung

>[!IMPORTANT]
>
>Vergessen Sie nicht, Ihre Mitarbeiter daran zu erinnern, dass Sie ihnen im Rahmen Ihrer Workfront-Schulung einen Testversand schicken.


Hochladen eines Testversands mit einem erweiterten Workflow. Wenn Ihre Organisation bereits Testversandvorlagen eingerichtet hat, wählen Sie die von Ihrem Team verwendete Vorlage aus und nehmen Sie dann einige Anpassungen vor.

* Passen Sie die E-Mail-Warnungen so an, dass niemand benachrichtigt wird, wenn eine Aktivität auf dem Testversand stattfindet.
* In der ersten Phase sollten 2 Prüfer/Genehmiger vorhanden sein.
* In der zweiten Phase sollte nur 1 Prüfer/Genehmiger vorhanden sein.

Wenn für Ihr Unternehmen noch keine Testversandvorlagen erstellt wurden, richten Sie einen Workflow für zwei Phasen ein.

* Weisen Sie sich und Ihren bevorzugten Mitarbeiter der ersten Stufe zu.
* Vergeben Sie einen Termin für den ersten Schritt von 1 Tag ab der Erstellung des Testversands.
* Weisen Sie der zweiten Stufe einen weiteren bevorzugten Mitarbeiter zu.
* Starten Sie die Bühne, wenn die Frist für die erste Phase abgelaufen ist.
* Geben Sie der Person in dieser Phase 2 Tage, um die Überprüfung abzuschließen, aber es muss bis Mittag getan werden.



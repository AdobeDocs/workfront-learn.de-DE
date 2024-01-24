---
title: Informationen zu E-Mail-Warnungen und Testversandbenachrichtigungen
description: den Unterschied zwischen E-Mail-Warnungen und Testversandbenachrichtigungen in [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Informationen zu E-Mail-Warnungen und Testversandbenachrichtigungen

E-Mail-Warnungen unterscheiden sich von Testversand-Benachrichtigungs-E-Mails. Sie erhalten eine Benachrichtigungs-E-Mail über einen Testversand, wenn Ihnen ein neuer Testversand zugewiesen wurde, wenn ein Testversand verspätet ist oder wenn eine neue Testversand-Version vorliegt, die Sie ansehen können.

![Ein Bild einer Benachrichtigungs-E-Mail zum Testversand, das angibt, dass ein neuer Testversand durchgeführt werden muss.](assets/email-alert-1.png)

Wenn Sie die Benachrichtigungsoption beim Hochladen eines Testversands deaktivieren, erhält niemand eine Mitteilung von [!DNL Workfront] , dass es einen neuen zu überprüfenden Nachweis gibt.

E-Mail-Warnhinweise werden pro Validierer/Genehmiger festgelegt, meistens beim Hochladen des Testversands. Sie können Ihren Testversand-Empfängern einen Standard-E-Mail-Warnhinweistyp zuweisen, damit Sie ihn nicht jedes Mal festlegen müssen, wenn Sie einen Testversand hochladen. Wenden Sie sich an Ihren Systemadministrator, wenn Sie wissen möchten, wie diese Standardeinstellungen festgelegt wurden.

![Ein Bild eines E-Mail-Warnhinweises, das angibt, dass eine Entscheidung über den Testversand getroffen wurde und dass ein Kommentar zu überprüfen ist.](assets/email-alert-2.png)

Auch wenn E-Mail-Warnungen auf [!UICONTROL Behinderte], werden die Testversand-Empfänger weiterhin über einen neuen Testversand oder eine neue Version informiert.

## Best Practices

| Best Practice | Deshalb |
|---|---|
| Deaktivieren Sie die Einstellung &quot;E-Mails von Workfront senden, wenn ein Kommentar zu einem Testversand abgegeben wird&quot; in den Workfront-Setups. | Wenn diese Einstellung aktiviert ist (standardmäßig), können Benutzer mehrere E-Mail-Benachrichtigungen für jeden Kommentar auf einem Testversand erhalten - eine von der Testfunktion und eine von Workfront selbst. Diese doppelten Benachrichtigungen führen zu einer Unterbrechung und Verwirrung der E-Mail-Benachrichtigung sowie zu einem vollständigen E-Mail-Posteingang, was letztendlich dazu führen kann, dass Benutzer die von ihnen empfangenen Testversandbenachrichtigungen ignorieren. Dies wiederum könnte verpasste Termine bedeuten. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü > Einrichtung > E-Mail > Überprüfen und Genehmigen . |



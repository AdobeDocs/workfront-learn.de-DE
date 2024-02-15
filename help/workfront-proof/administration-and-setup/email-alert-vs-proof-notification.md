---
title: Grundlegendes zu E-Mail-Warnhinweisen und Benachrichtigungen zu Korrekturabzügen
description: Sie müssen den Unterschied zwischen E-Mail-Warnhinweisen und Benachrichtigungen zu Korrekturabzügen in [!DNL  Workfront]verstehen.
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: ht
source-wordcount: '306'
ht-degree: 100%

---

# Grundlegendes zu E-Mail-Warnhinweisen und Benachrichtigungen zu Korrekturabzügen

E-Mail-Warnhinweise unterscheiden sich von E-Mails mit Korrekturabzugsbenachrichtigungen. Sie erhalten eine Benachrichtigungs-E-Mail über einen Korrekturabzug, wenn Ihnen ein neuer Korrekturabzug zur Überprüfung zugewiesen wurde, wenn ein Korrekturabzug verspätet ist oder wenn eine neue Version des Korrekturabzugs vorliegt, die Sie sich ansehen können.

![Ein Bild einer Benachrichtigungs-E-Mail zum Korrekturabzug, das angibt, dass ein neuer Korrekturabzug überprüft werden muss.](assets/email-alert-1.png)

Wenn Sie die Benachrichtigungsoption beim Hochladen eines Korrekturabzugs deaktivieren, erhält niemand eine Mitteilung von [!DNL Workfront], dass es einen neuen zu überprüfenden Korrekturabzug gibt.

E-Mail-Benachrichtigungen werden für jede prüfende/genehmigende Person festgelegt, meistens, sobald der Korrekturabzug hochgeladen wird. Den Empfängerinnen und Empfängern Ihrer Korrekturabzüge kann ein Standard-E-Mail-Warntyp zugewiesen werden, damit Sie diesen nicht jedes Mal neu festlegen müssen, wenn Sie einen Korrekturabzug hochladen. Wenden Sie sich an Ihre Systemadmins, wenn es darum geht, diese Standardeinstellungen festzulegen.

![Ein Bild eines E-Mail-Warnhinweises, das angibt, dass eine Entscheidung über den Korrekturabzug getroffen wurde und dass ein Kommentar zu überprüfen ist.](assets/email-alert-2.png)

Auch wenn E-Mail-Warnhinweise [!UICONTROL deaktiviert] sind, werden die Empfängerinnen und Empfänger der Korrekturabzüge weiterhin über einen neuen Korrekturabzug oder eine neue Version informiert.

## Best Practices

| Best Practice | Das sind die Gründe |
|---|---|
| Deaktivieren der Einstellung „E-Mails von Workfront senden, wenn ein Korrekturabzug kommentiert wird“ im Workfront-Setup | Wenn diese Einstellung aktiviert ist (dies ist standardmäßig der Fall), können Benutzende mehrere E-Mail-Benachrichtigungen für jeden Kommentar zu einem Korrekturabzug erhalten – eine von der Proofing-Funktion und eine von Workfront selbst. Diese doppelten Benachrichtigungen führen zu Störungen und Verwirrung in Bezug auf die E-Mail-Benachrichtigungen sowie zu einem vollen E-Mail-Posteingang. Dies kann letztendlich die Folge haben, dass Benutzende die von ihnen empfangenen Benachrichtigungen über Korrekturabzüge ignorieren. Dadurch können wiederum Fristen verpasst werden. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Setup“ > „E-Mail“ > „Überprüfung und Genehmigung“. |



---
title: Grundlegendes zu E-Mail-Warnhinweisen und Benachrichtigungen zu Korrekturabzügen
description: Sie müssen den Unterschied zwischen E-Mail-Warnhinweisen und Benachrichtigungen zu Korrekturabzügen in [!DNL  Workfront]verstehen.
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:07:01.396Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 307
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



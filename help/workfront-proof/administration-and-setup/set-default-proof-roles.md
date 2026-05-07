---
title: Festlegen von Standard-Korrekturabzugsrollen
description: Erfahren Sie, wie Sie die standardmäßige Korrekturabzugsrolle festlegen, die zugewiesen wird, wenn neue Benutzende angelegt werden oder Personen einen Korrekturabzug öffnen.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:03:40.797Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 87%

---

# Festlegen von Standard-Korrekturabzugsrollen



Die erste Standardeinstellung, die Sie vornehmen müssen, ist die Festlegung einer standardmäßigen Korrekturabzugsrolle, die zugewiesen wird, wenn neue Benutzende angelegt werden oder Personen einen Korrekturabzug öffnen.

Korrekturabzug-Rollen bestimmen, was ein Benutzer mit einem Korrekturabzug tun kann - einfach ihn anzeigen, Kommentare abgeben, ihn genehmigen usw. [!DNL Workfront] empfiehlt, für alle Benutzer Standardwerte für die Korrekturabzugsrolle festzulegen, um das Hinzufügen von Empfängern zu Korrekturabzügen und das Einrichten von Workflows schneller und einfacher zu gestalten.

![Beim Hochladen eines Korrekturabzugs können Korrekturabzugsrollen ausgewählt werden](assets/proof-system-setups-proof-role-example.png)

Diese standardmäßige Korrekturabzugsrolle kann jedoch geändert werden, wenn einzelne Korrekturabzüge hochgeladen werden, um sicherzustellen, dass alle in der Lage sind, die für sie erforderliche Rolle im Überprüfungs- und Genehmigungsprozess zu erfüllen.


## Festlegen von Standard-Korrekturabzugsrollen

1. Wählen Sie **Einrichtung** im [!UICONTROL Hauptmenü].
1. Wählen Sie **Überprüfung und Genehmigung** im linken Menü.
1. Klicken Sie auf die Schaltfläche neben der gewünschten standardmäßigen Korrekturabzugsrolle sowohl für neue [!DNL Workfront]-Benutzende als auch für Gastbenutzende von Korrekturabzügen als „designierte Empfänger“, d. h. alle Personen, die dem Korrekturabzug-Workflow entweder manuell oder über eine Workflow-Vorlage hinzugefügt werden.
1. Klicken Sie auf die Schaltfläche neben der gewünschten standardmäßigen Korrekturabzugsrolle sowohl für neue [!DNL Workfront]-Benutzende als auch für Gastbenutzende von Korrekturabzügen für „Nicht-Empfänger“-Benutzende. Dies sind in der Regel [!DNL Workfront]-Benutzende, die zwar Zugriff auf einen Korrekturabzug haben, aber nicht zu den Personen gehören, die dem Workflow zugewiesen sind.
1. Speichern Sie die Änderungen.

![Überprüfungs- und Genehmigungseinstellungen in Workfront](assets/proof-system-setups-workfront-defaults.png)

Überlegen Sie, was die meisten Ihrer Benutzenden und Gäste erwarten, wenn sie zu einem Proofing-Workflow hinzugefügt werden. Dies sollte Ihre Standardeinstellung sein.

## Best Practices

| Best Practice | Das sind die Gründe |
|---|---|
| Legen Sie in Workfront die Einstellung „Benutzerrollen für Nicht-Empfänger, die einen Dokument-Korrekturabzug öffnen“ auf „Schreibgeschützt“ oder „Prüfer“ fest. | Für die anderen Optionen dieser Einstellung muss eine Korrekturabzugsentscheidung getroffen werden, wodurch Ihr Proofing-Workflow gestört werden kann. Im Allgemeinen müssen Personen, die nicht zum Korrekturabzug-Workflow hinzugefügt werden, lediglich den Korrekturabzug ansehen oder Kommentare abgeben, den Korrekturabzug aber nicht tatsächlich genehmigen. Daher wählen Sie am besten die Optionen „Schreibgeschützt“ oder „Prüfer“ aus. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Setup“ > „Überprüfung und Genehmigung“. |

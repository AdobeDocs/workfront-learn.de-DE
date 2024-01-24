---
title: Festlegen von standardmäßigen Testrollen
description: Erfahren Sie, wie Sie die standardmäßige Testversandrolle festlegen, die zugewiesen wird, wenn neue Benutzer erstellt werden oder Personen einen Testversand öffnen .
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Festlegen von standardmäßigen Testrollen



Mit der ersten abgeschlossenen Standardeinstellung wird eine standardmäßige Testversandrolle bestimmt, die zugewiesen wird, wenn neue Benutzer erstellt oder Personen einen Testversand öffnen.

Testrollen bestimmen, was ein Benutzer mit einem Testversand machen kann - sehen Sie sich ihn an, erstellen Sie Kommentare, genehmigen Sie ihn usw. [!DNL Workfront] empfiehlt die Festlegung von Standardwerten für die Testversandrolle für alle Benutzer, um das Hinzufügen von Empfängern zu Testsendungen und die schnellere und einfachere Einrichtung von Workflows zu erleichtern.

![Testversandrollen können beim Hochladen eines Testversands ausgewählt werden](assets/proof-system-setups-proof-role-example.png)

Diese standardmäßige Testversand-Rolle kann jedoch geändert werden, wenn einzelne Testsendungen hochgeladen werden, um sicherzustellen, dass jeder in der Lage ist, die von ihm im Prüfungs- und Genehmigungsprozess benötigte Rolle zu erfüllen.


## Festlegen von standardmäßigen Testrollen

1. Auswählen **Einrichtung** aus dem [!UICONTROL Hauptmenü].
1. Auswählen **Prüfung und Genehmigung** über das Menü links.
1. Klicken Sie auf die Schaltfläche neben der gewünschten standardmäßigen Testversandrolle für beide neue [!DNL Workfront] Benutzer und Benutzer von Testsendungen für &quot;bestimmte Empfänger&quot; - alle, die manuell oder über eine Workflow-Vorlage zum Testversand-Workflow hinzugefügt werden.
1. Klicken Sie auf die Schaltfläche neben der gewünschten standardmäßigen Testversandrolle für beide neue [!DNL Workfront] Benutzer und Benutzer von Gästebesuchen für Benutzer, die keine Empfänger sind. Diese [!DNL Workfront] Benutzer, die Zugriff auf einen Testversand haben, aber nicht zu den Personen gehören, die dem Workflow zugewiesen sind.
1. Speichern Sie die Änderungen.

![Überprüfungs- und Genehmigungseinstellungen in Workfront](assets/proof-system-setups-workfront-defaults.png)

Überlegen Sie, was die meisten Ihrer Benutzer und Gäste tun sollen, wenn sie zu einem Testversand-Workflow hinzugefügt werden. Dies sollte Ihre Standardeinstellung sein.

## Best Practices

| Best Practice | Deshalb |
|---|---|
| Verwenden Sie die Einstellung &quot;Benutzerrollen für Nicht-Empfänger, die einen Dokumentversand öffnen&quot;in Workfront nur &quot;Schreibgeschützt&quot;oder &quot;Überprüfer&quot;. | Für die anderen Optionen dieser Einstellung muss eine Testversandentscheidung getroffen werden, die den Testversand-Workflow zum Verfall bringen kann. Im Allgemeinen müssen Personen, die nicht zum Testversand-Workflow hinzugefügt werden, lediglich den Testversand ansehen oder Kommentare abgeben, den Testversand nicht validieren. Daher sind die Optionen Schreibgeschützt oder Prüfer Ihre beste Wahl. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü > Einrichtung > Überprüfen und Genehmigen . |

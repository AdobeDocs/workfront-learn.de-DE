---
title: Korrekturabzugsrollen und E-Mail-Warnhinweise
description: Erfahren Sie, wie Sie ordnungsgemäße Korrekturabzugsrollen und E-Mail-Warnhinweise aktivieren, damit Empfängerinnen und Empfänger von Korrekturabzügen Zugriff auf Korrekturabzüge haben und Einblick in die in [!DNL  Workfront]durchgeführten Arbeiten haben.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '551'
ht-degree: 100%

---

# Korrekturabzugsrollen und E-Mail-Warnhinweise

Korrekturabzugsrollen und E-Mail-Warnhinweise tragen dazu bei, den Korrekturabzug-Workflow zu optimieren und sicherzustellen, dass Empfängerinnen und Empfänger den richtigen Zugriff auf Korrekturabzüge erhalten und Einblick in die durchgeführten Arbeiten haben.

Sehen wir uns die grundlegende Terminologie für Korrekturabzüge an:

* **Korrekturabzugsrolle** – Definiert, was eine Person mit einem Korrekturabzug tun kann (z. B. Kommentar, Markup, Genehmigung usw.).
* **E-Mail-Warnhinweis:** E-Mails, die an Personen im Korrekturabzug-Workflow gesendet werden, wenn zum Korrekturabzug eine Aktivität vorhanden ist.

![Ein Bild des Fensters [!UICONTROL Neuer Korrekturabzug] mit Hervorhebung der Spalten [!UICONTROL Korrekturabzugsrolle] und [!UICONTROL E-Mail-Warnhinweisen].](assets/proof-roles-and-email-alerts.png)

Ihre Korrekturabzug-Systemadmins können standardmäßige Korrekturabzugsrollen und E-Mail-Warnhinweise für die Menschen in Ihrem Unternehmen festlegen; die mit Korrekturabzügen arbeiten. Darüber hinaus können diese Informationen in Korrekturabzug-Workflow-Vorlagen (auch als automatisierte Workflow-Vorlagen bezeichnet) integriert werden.

Es kann jedoch vorkommen, dass Sie diese Informationen beim Hochladen eines Korrekturabzugs manuell festlegen müssen.

[!DNL Workfront] bietet folgende allgemeine Empfehlungen für die Zuweisung von Korrekturabzugsrollen an Empfängerinnen und Empfänger von Korrekturabzügen:

* **Prüfende und genehmigende Person** – Diese Personen können sowohl Kommentare zu Korrekturabzügen abgeben als auch eine Entscheidung (z. B. genehmigt oder abgelehnt) zu einem Korrekturabzug treffen. Verwenden Sie diese Korrekturabzugsrolle für die wichtigsten internen und externen Beteiligten am Überprüfungsprozess.
* **Prüfende Person** – Einige Personen in Ihrem Korrekturabzug-Workflow müssen nur Kommentare abgeben. Für sie ist diese Rolle ideal. Die Rolle der prüfenden Person kann auch an Benutzende von [!DNL Workfront] zugewiesen werden, die in erster Linie Korrekturabzüge hochladen oder als verantwortliche Person für einen Korrekturabzug dienen, ansonsten jedoch nicht am Proofing-Prozess beteiligt sind.
* **Schreibgeschützt** – Ideal für Empfängerinnen und Empfänger, die den Korrekturabzug nur sehen müssen. [!UICONTROL Schreibgeschützt] gibt nur Ansichtszugriff und lässt keine Kommentare zu.

[!DNL Workfront] bietet diese allgemeinen Empfehlungen bei der Zuweisung von E-Mail-Warnhinweise an Empfängerinnen und Empfänger von Korrekturabzügen:

* **Endgültige Entscheidung** – Diese Funktion sendet eine E-Mail, wenn die letzte Person eine Entscheidung über den Korrekturabzug getroffen hat. Weisen Sie diese der Person zu, die den Korrekturabzug-Workflow überwacht. Dies können Manager und Managerinnen, Verantwortliche, Ersteller und Erstellerinnen von Korrekturabzügen sowie Projekt-Manager und Projekt-Managerinnen oder auch andere Benutzende von [!DNL Workfront] sein. [!DNL Workfront] empfiehlt diesen Warnhinweis bei Verwendung eines einfachen Workflows, sodass die Person, die den Korrekturabzug überwacht, weiß, dass alle Entscheidungen getroffen wurden.
* **Entscheidungen** – Diese Funktion sendet Warnhinweise, wenn die am Proofing-Workflow beteiligten Personen jeweils eine Entscheidung über den Korrekturabzug treffen. Diese Option ist am besten geeignet, wenn ein automatisierter Arbeitsablauf mit mehreren Entscheidungen verwendet wird. Weisen Sie dies der Person zu, die den Korrekturabzug-Workflow überwacht. Dies können Manager und Managerinnen, Verantwortliche, Ersteller und Erstellerinnen von Korrekturabzügen sowie Projekt-Manager und Projekt-Managerinnen oder auch andere Benutzende von [!DNL Workfront] sein.
* **Deaktiviert** – Verwenden Sie diese Option für Gastbenutzende von Korrekturabzügen, um die Anzahl der E-Mails zu begrenzen, die sie über den Korrekturabzug erhalten. Empfängerinnen und Empfänger werden weiterhin über neue Korrekturabzüge, neue Versionen und verspätete Korrekturabzüge informiert. Benutzende von [!DNL Workfront] erhalten darüber hinaus Direktnachrichten, die in einem Korrekturabzugskommentar gemacht wurden, über @username, und Gastempfängerinnen und -empfänger erhalten sie über @emailaddress.

## Sie sind dran

1. Melden Sie sich bei Workfront an und legen Sie Benutzerinnen bzw. Benutzer an, die Proofing nutzen sollen, das Sie nicht zuvor erstellt haben. Legen Sie das Profil für Korrekturabzugsberechtigungen in ihren Benutzereinstellungen entsprechend der Rolle fest, die die Person in Korrekturabzug-Workflows spielen wird.
1. Bearbeiten Sie für bereits erstellte Benutzende bei Bedarf ihre Einstellungen, um die Profilauswahl für Korrekturabzugsberechtigungen anzupassen.
1. Rufen Sie den Bereich „Proofing-Einstellungen“ auf und wechseln Sie zur Registerkarte „Benutzer“. Überprüfen Sie die persönlichen Einstellungen für Ihre Benutzenden – Sprache, Zeitzone, Datumsformat, Standard-Korrekturabzugsrolle und Standard-E-Mail-Warnhinweis. Dies ist wichtig, wenn diese Benutzenden erstellt wurden, bevor die globalen Systemstandardwerte festgelegt wurden.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->

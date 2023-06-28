---
title: Testadressen und E-Mail-Warnungen
description: Erfahren Sie, wie Sie ordnungsgemäße Testversandrollen und E-Mail-Warnungen aktivieren, damit Testversand-Empfänger Zugriff auf die durchgeführten Arbeiten haben, und wie Sie die entsprechenden Schritte in [!DNL  Workfront].
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
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Testadressen und E-Mail-Warnungen

Proof-Rollen und E-Mail-Warnhinweise tragen dazu bei, den Testversand-Workflow zu optimieren und sicherzustellen, dass die Empfänger den richtigen Zugriff auf Testsendungen haben und Einblick in die durchgeführten Arbeiten erhalten.

Sehen wir uns die grundlegende Terminologie des Testversands an:

* **Testversandrolle —** Definiert, was ein Benutzer mit einem Testversand tun kann (z. B. Kommentar, Markup, Genehmigung usw.).
* **E-Mail-Warnhinweis —** E-Mails, die an Personen im Testversand-Workflow gesendet werden, wenn eine Aktivität im Testversand vorhanden ist.

![Ein Bild der [!UICONTROL Neuer Testversand] mit dem [!UICONTROL Proof role] und [!UICONTROL E-Mail-Warnungen] hervorgehobene Spalten.](assets/proof-roles-and-email-alerts.png)

Ihr Testversand-Systemadministrator kann standardmäßige Testversandrollen und E-Mail-Warnungen für die Testversand-Benutzer Ihrer Organisation festlegen. Darüber hinaus können diese Informationen in Testversand-Workflow-Vorlagen (auch als automatisierte Workflow-Vorlagen bezeichnet) integriert werden.

Es kann jedoch vorkommen, dass Sie diese Informationen beim Hochladen eines Testversands manuell festlegen müssen.

[!DNL Workfront] bietet folgende allgemeine Empfehlungen für die Zuweisung von Testversandrollen an Testversand-Empfänger:

* **Reviewer und Genehmiger —** Diese Benutzer können sowohl zu Testsendungen Stellung nehmen als auch eine Entscheidung (z. B. genehmigt oder abgelehnt) für einen Testversand treffen. Verwenden Sie diese Testfunktion für die wichtigsten internen und externen Akteure im Überprüfungsprozess.
* **Überprüfer —** Einige Personen in Ihrem Testversand-Workflow müssen nur Kommentare abgeben. Diese Rolle ist ideal für sie. Die Überprüferrolle kann auch [!DNL Workfront] -Benutzer, die in erster Linie Testsendungen hochladen oder als Testversand-Besitzer dienen, aber anderweitig nicht Teil des Testversands sind.
* **Schreibgeschützt —** Ideal für Empfänger, die nur den Testversand sehen müssen. [!UICONTROL Schreibgeschützt] gibt Ansichtszugriff und lässt keine Kommentare zu.

[!DNL Workfront] bietet diese allgemeinen Empfehlungen bei der Zuweisung von E-Mail-Warnungen an Testversand-Empfänger:

* **Endgültige Entscheidung —** Dieser versendet eine E-Mail, wenn die letzte Person eine Entscheidung über den Testversand trifft. Weisen Sie dies der Person zu, die den Testversand-Workflow überwacht. Dabei kann es sich um einen Testversandverantwortlichen, einen Testversandinhaber, einen Ersteller, einen Projektmanager oder einen anderen [!DNL Workfront] Benutzer. [!DNL Workfront] empfiehlt diese Warnung bei Verwendung eines einfachen Workflows, sodass die Person, die den Testversand überwacht, weiß, dass alle Entscheidungen getroffen wurden.
* **Entscheidungen —** Dadurch werden Warnhinweise gesendet, wenn jeder Verantwortliche des Testversand-Workflows eine Entscheidung über den Testversand trifft. Diese Option eignet sich am besten für einen automatisierten Workflow mit mehreren Entscheidungen. Weisen Sie ihn der Person zu, die den Testversand-Workflow überwacht. Dabei kann es sich um einen Testversandverantwortlichen, einen Testversandinhaber, einen Ersteller, einen Projektmanager oder einen anderen [!DNL Workfront] Benutzer.
* **Behinderte —** Verwenden Sie diese Option für Benutzer von Testsendungen, um die Anzahl der E-Mails zu begrenzen, die sie über den Testversand erhalten. Empfänger werden weiterhin über neue Testsendungen, neue Versionen und verspätete Testsendungen benachrichtigt, plus [!DNL Workfront] -Benutzer erhalten über @username und Gastempfänger mit @emailaddress Direktnachrichten, die in einem Testversand-Kommentar gesendet werden.

## Ihre Wendung

1. Melden Sie sich bei Workfront an und erstellen Sie Benutzer, die die zuvor noch nicht erstellte Testversand-Aktivität verwenden. Legen Sie das Profil für Testversandberechtigungen in den Benutzereinstellungen entsprechend der Rolle fest, die die Person in Testversand-Workflows spielen wird.
1. Bearbeiten Sie für bereits erstellte Benutzer bei Bedarf ihre Einstellungen, um die Profilauswahl für Testberechtigungen anzupassen.
1. Öffnen Sie den Bereich Testversandeinstellungen und rufen Sie die Registerkarte Benutzer auf. Überprüfen Sie die persönlichen Einstellungen Ihrer Benutzer - Sprache, Zeitzone, Datumsformat, Standardrolle für Testversand und Standard-E-Mail-Warnung. Dies ist wichtig, wenn diese Benutzer erstellt wurden, bevor die globalen Systemstandardwerte festgelegt wurden.

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

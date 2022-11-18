---
title: Durchführen des Testversands
description: Erfahren Sie, wie Sie [!UICONTROL SOCD] Indikatoren, Fortschritt des Testversands und Berichte zur Verfolgung des Fortschritts eines Testversands in [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Durchführen des Testversands

Als Projektmanager, Testversand-Manager oder anderer Beteiligter am Prüfungs- und Genehmigungsprozess möchten Sie den Fortschritt Ihrer Testsendungen verfolgen. Sie können dies tun mit [!DNL Workfront’s] integriert **Testversandindikatoren** auf [!UICONTROL Dokumente] oder durch Schreiben benutzerdefinierter Berichte.

So zeigen Sie den Fortschritt des Testversands an: [!DNL Workfront], müssen Sie über eine Lizenz für Plan, Arbeit oder Überprüfung verfügen und ein Testnutzer sein. Wenn Sie sich nicht sicher sind, [!DNL Workfront] Profil erfüllt diese Anforderungen, wenden Sie sich an den Administrator des Testversand-Systems in Ihrem Unternehmen.

## Fortschritt beim Testversand verfolgen mit [!UICONTROL SOCD] Indikatoren und Teststatus

Verschaffen Sie sich einen allgemeinen Überblick darüber, wie der Testversand durch den Prüfungs- und Genehmigungsprozess mit dem [!UICONTROL SOCD] -Symbole in [!UICONTROL Dokumente] Liste. Diese Symbole geben an, welche Aktionen beim Testversand durchgeführt wurden.

![Ein Bild der [!UICONTROL Dokumente] in einer Liste [!DNL  Workfront] Projekt mit [!UICONTROL SOCD] hervorgehobene Symbole.](assets/manage-proofs-socd.png)

Die Symbole geben an, welche Arbeit an einem Testversand von dem Zeitpunkt an, an dem Sie den Testversand an die Empfänger senden, bis zu dem Zeitpunkt, an dem sie über den Testversand entscheiden.

* **S —** Der Testversand wurde an die Empfänger gesendet.
* **O —** Der Testversand wurde eröffnet.
* **C —** Zu dem Testversand wurden Anmerkungen gemacht.
* **D —** Über den Testversand wurde entschieden (genehmigt, abgelehnt usw.).

Die Farben zeigen an, ob die Aktion abgeschlossen ist oder nicht.

* **weiß —** Der Schritt ist noch nicht passiert.
* **Grün —** Der Schritt wurde abgeschlossen.
* **Orange —** Die Testversand-Deadline beträgt 24 Stunden und der Schritt ist nicht passiert.
* **Rot —** Die Testversand-Deadline ist abgelaufen und der Schritt ist nicht passiert.

Die [!UICONTROL SOCD] auf [!UICONTROL Dokumente] im Zusammenfassungsfenster oder im [!UICONTROL Dokumentdetails], ist eine allgemeine Zusammenfassung des Testfortschritts. [!DNL Workfront] konfiguriert dies anhand des Empfängers, der im Testversand am &quot;meisten hinterher&quot;ist.

Wenn es beispielsweise drei Validierungsverantwortliche/Genehmigende gibt und nur zwei davon den Testversand angesehen und Kommentare abgegeben haben, wird die [!UICONTROL SOCD] -Symbole zeigen an, dass der Testversand gesendet wurde ([!UICONTROL S]) und geöffnet ([!UICONTROL O]), jedoch nicht, dass Kommentare abgegeben wurden ([!UICONTROL C]).

Wenn Sie wissen möchten, wie jeder einzelne Testversand-Empfänger funktioniert, öffnen Sie den Testversand-Workflow. Der allgemeine Testfortschritt befindet sich oben im Fenster. Jede Etappe verfügt über einen eigenen Fortschrittsanzeige in der grauen Leiste.  Neben jedem Benutzer befindet sich der Fortschritt des Kontakts.

![Ein Bild der [!UICONTROL Testversand-Workflow] -Abschnitt eines Dokuments.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Teststatus

Der Testversandstatus basiert auf dem Status der Testversand-Empfänger der Bühne. Der allgemeine Testversandstatus wird auf der [!UICONTROL Dokumente] Seite rechts neben dem [!UICONTROL SOCD] Indikatoren, damit Sie leicht feststellen können, ob Sie eine Entscheidung über den Testversand haben.

![Ein Bild der [!UICONTROL Dokumente] in einer Liste [!DNL  Workfront] Projekt mit dem allgemeinen Testversandstatus hervorgehoben.](assets/manage-proofs-overall-status.png)

Dieser Testversandstatus gibt den Gesamtstatus des Testversands an. Wenn beispielsweise zwei Empfänger den Testversand validiert haben, zeigt der jeweilige Status an [!UICONTROL Genehmigt]. Der dritte Empfänger hat jedoch noch keine Entscheidung getroffen, sodass der Status dieser Person [!UICONTROL Ausstehend]. Daher wird der Gesamtstatus als [!UICONTROL Ausstehend].

Wenn benutzerdefinierte Status für Ihr Unternehmen konfiguriert wurden, werden diese Status verwendet. Andernfalls werden die Standardstatusoptionen von angezeigt:

* [!UICONTROL Ausstehend]
* [!UICONTROL Genehmigt]
* [!UICONTROL Genehmigt mit Änderungen]
* [!UICONTROL Erforderliche Änderungen]
* [!UICONTROL Nicht relevant]

Öffnen Sie das Workflow-Fenster Testversand , um den Testversandstatus für die Empfänger anzuzeigen, denen die [!UICONTROL Überprüfer und Genehmiger] oder [!UICONTROL Genehmiger ]Testversandrollen.

## Berichte in [!DNL Workfront]

Sie können auch [!DNL Workfront’s] Berichterstellungsfunktionen zur Verfolgung von Testsendungen während des Prüfungs- und Genehmigungsprozesses.

Ein Bericht über die Testversandvalidierung hilft Ihnen, ausstehende Validierungen zu verfolgen, um sicherzustellen, dass Termine eingehalten werden.

![Ein Bild eines Validierungsberichts für einen Testversand in [!DNL  Workfront].](assets/proof-approval-report.png)

Ein Dokumentversionsbericht ermöglicht die Verwaltung und Verfolgung von Testversandversionen.

![Ein Bild eines Dokumentversionsberichts in [!DNL  Workfront].](assets/document-version-report.png)

Es wird empfohlen, mit Ihrem [!DNL Workfront] Berater , um Berichte zu erstellen, die den Anforderungen Ihres Unternehmens entsprechen. Einige Berichte müssen mit [!DNL Workfront’s] Textmodusberichte.

## Ihre Wendung

Wenden Sie sich an Ihr Team oder Ihren Testsystemadministrator, um herauszufinden, welche Art von Reporting Sie in Workfront verwenden werden, um sicherzustellen, dass Testversand-Workflows reibungslos ausgeführt werden.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->

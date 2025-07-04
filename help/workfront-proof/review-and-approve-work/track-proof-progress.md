---
title: Verfolgen des Korrekturabzugfortschritts
description: Erfahren Sie, wie Sie [!UICONTROL SOCD]-Indikatoren, den Korrekturabzugsfortschritt und Berichte verwenden können, um den Fortschritt eines Korrekturabzugs in [!DNL  Workfront]zu verfolgen.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: ht
source-wordcount: '767'
ht-degree: 100%

---

# Verfolgen des Korrekturabzugfortschritts

Als Projekt-Managerin bzw. -Manager, Korrekturabzugs-Managerin bzw. -Manager oder sonstige verantwortliche Person im Überprüfungs- und Genehmigungsprozess sollten Sie den Fortschritt Ihrer Korrekturabzüge verfolgen. Sie können dies mit [!DNL Workfront's]integrierten **Korrekturabzugs-Fortschrittsindikatoren** auf der Seite [!UICONTROL Dokumente] oder durch das Schreiben benutzerdefinierter Berichte vornehmen.

Um den Korrekturabzugsfortschritt in [!DNL Workfront] anzuzeigen, müssen Sie über eine Plan-, Arbeits- oder Überprüfunglizenz verfügen und zu den Benutzenden des Proofings gehören. Wenn Sie sich nicht sicher sind, ob Ihr [!DNL Workfront]-Profil diese Anforderungen erfüllt, wenden Sie sich an die oder den Systemadmin für Korrekturabzüge in Ihrem Unternehmen.

## Verfolgen Sie den Korrekturabzugsfortschritt mit [!UICONTROL SOCD]-Indikatoren und Korrekturabzugs-Status

Über die [!UICONTROL SOCD]-Symbole in der Liste [!UICONTROL Dokumente] erhalten Sie einen Überblick über den Fortschritt des Überprüfung- und Genehmigungsprozesses des Korrekturabzugs. Diese Symbole kennzeichnen bestimmte Aktionen, die mit dem Korrekturabzug durchgeführt werden.

![Ein Bild der Liste [!UICONTROL Dokumente] in einem [!DNL  Workfront]-Projekt, wo die [!UICONTROL SOCD]-Symbolen hervorgehoben sind.](assets/manage-proofs-socd.png)

Die Symbole zeigen die Arbeit an einem Korrekturabzug von dem Zeitpunkt an, an dem Sie den Korrekturabzug an die Empfänger bzw. Empfängerinnen senden, bis zu dem Zeitpunkt, an dem diese eine Entscheidung über den Korrekturabzug treffen.

* **S —** Der Korrekturabzug wurde an die Empfänger bzw. Empfängerinnen gesendet.
* **O —** Der Korrekturabzug wurde geöffnet.
* **C —** Es wurden Kommentare zu dem Korrekturabzug abgegeben.
* **D —** Es wurde eine Entscheidung über den Korrekturabzug getroffen (genehmigt, abgelehnt usw.).

Die Farben zeigen an, ob die Aktion abgeschlossen ist oder nicht.

* **Weiß –** Der Schritt ist noch nicht erfolgt.
* **Grün –** Der Schritt wurde abgeschlossen.
* **Orange –** Die Frist für den Korrekturabzug liegt innerhalb der nächsten 24 Stunden und der Schritt ist noch nicht erfolgt.
* **Rot –** Die Frist für den Korrekturabzug ist verstrichen und der Schritt ist noch nicht erfolgt.

Das Element [!UICONTROL SOCD] in der Liste [!UICONTROL Dokumente], im Zusammenfassungs-Panel oder in den [!UICONTROL Dokumentendetails] bietet eine allgemeine Zusammenfassung über den Fortschritt des Korrekturabzugs. [!DNL Workfront] konfiguriert dies auf der Grundlage der empfangenden Person, die im Korrekturabzug-Prozess am weitesten zurückliegt.

Wenn es beispielsweise drei prüfende/genehmigende Personen gibt und nur zwei von ihnen den Korrekturabzug angesehen und Kommentare abgegeben haben, dann zeigen die [!UICONTROL SOCD]-Symbole an, dass der Korrekturabzug versandt ([!UICONTROL S]) und geöffnet ([!UICONTROL O]) wurde, nicht aber, dass Kommentare abgegeben wurden ([!UICONTROL C]).

**Sobald eine endgültige Entscheidung** (z. B. genehmigt oder abgelehnt) für einen Korrekturabzug getroffen wurde, werden möglicherweise alle SOCD-Indikatoren für Benutzende in diesem Schritt grün angezeigt, auch wenn einzelne Aktionen (z. B. Öffnen des Korrekturabzugs oder Erstellen von Kommentaren) nicht ausgeführt wurden. Dieses systemweite Verhalten ist so konzipiert, dass es den allgemeinen Abschluss der Phase widerspiegelt, nicht die individuelle Interaktion.

**Vor der Registrierung einer Entscheidung** spiegelt jeder SOCD-Indikator die tatsächliche Benutzeraktivität wider (z. B. weiß, wenn keine Aktion durchgeführt wurde; grün, wenn die Aktion abgeschlossen wurde). Nach der Entscheidung geht das System davon aus, dass der Workflow abgeschlossen ist, und aktualisiert alle Indikatoren entsprechend.

Wenn Sie wissen möchten, wie weit die einzelnen Empfängerinnen bzw. Empfänger des Korrekturabzugs sind, öffnen Sie den Proofing-Workflow. Der gesamte Korrekturabzugsfortschritt wird im oberen Teil des Fensters angezeigt. Jeder Schritt hat seine eigene Fortschrittsanzeige in der grauen Leiste.  Und neben jeder bzw. jedem Benutzenden wird der Fortschritt der Einzelperson angezeigt.

![Ein Bild des Abschnitts [!UICONTROL Proofing-Workflow] eines Dokuments.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Korrekturabzugs-Status

Der Status des Korrekturabzugs basiert auf dem Status der Korrekturabzugs-Empfangenden des Schritts. Der gesamte Korrekturabzugs-Status ist auf der Seite [!UICONTROL Dokumente] rechts neben den [!UICONTROL SOCD]-Indikatoren ersichtlich, sodass Sie leicht erkennen können, ob Sie eine Entscheidung über den Korrekturabzug getroffen haben.

![Ein Bild der Liste [!UICONTROL Dokumente] in einem [!DNL  Workfront]-Projekt, in dem der gesamte Korrekturabzugs-Status hervorgehoben ist.](assets/manage-proofs-overall-status.png)

Dieser Korrekturabzugs-Status zeigt den Gesamtstatus des Korrekturabzugs an. Wenn zum Beispiel zwei Empfänger und/oder Empfängerinnen den Korrekturabzug genehmigt haben, werden ihre individuellen Status als [!UICONTROL Genehmigt] angezeigt. Die dritte Person hat jedoch noch keine Entscheidung getroffen, sodass deren Status [!UICONTROL Ausstehend] lautet. Daher wird der Gesamtstatus als [!UICONTROL Ausstehend] angezeigt.

Wenn für Ihr Unternehmen benutzerdefinierte Status konfiguriert wurden, werden diese Status verwendet. Andernfalls sehen Sie folgende Standard-Statusoptionen:

* [!UICONTROL Ausstehend]
* [!UICONTROL Genehmigt]
* [!UICONTROL Genehmigt mit Änderungen]
* [!UICONTROL Erforderliche Änderungen]
* [!UICONTROL Nicht relevant]

Öffnen Sie das Fenster des Proofing-Workflows, um den Korrekturabzugs-Status von Empfängern bzw. Empfängerinnen mit den Korrekturabzugs-Rollen [!UICONTROL Prüfer und genehmigende Person] oder [!UICONTROL Genehmigende Person]anzuzeigen.

## Berichte in [!DNL Workfront]

Sie können die Berichterstellungsfunktionen von [!DNL Workfront's] auch nutzen, um Korrekturabzüge auf ihrem Weg durch den Überprüfungs- und Genehmigungsprozess zu verfolgen.

Ein Bericht über die Genehmigung von Korrekturabzügen hilft Ihnen, ausstehende Genehmigungen nachzuverfolgen, um sicherzustellen, dass die Fristen eingehalten werden.

![Ein Bild eines Korrekturabzugs-Genehmigungsberichts in [!DNL  Workfront].](assets/proof-approval-report.png)

Mit einem Bericht über die Dokumentversion können Sie Korrekturabzugsversionen verwalten und verfolgen.

![Ein Bild eines Dokumentversionsberichts in [!DNL  Workfront].](assets/document-version-report.png)

Wir empfehlen, mit Ihrer [!DNL Workfront]-Beraterin bzw. Ihrem -Berater zusammenzuarbeiten, um Berichte zu erstellen, die den Anforderungen Ihres Unternehmens entsprechen. Für einige der Berichte müssen Sie mit der Berichterstellung im [!DNL Workfront's]-Textmodus vertraut sein.

## Sie sind dran

Sprechen Sie mit Ihrem Team bzw. der oder dem Systemadmin für Korrekturabzüge, um herauszufinden, welche Art von Berichten in Workfront verwendet werden, damit die Korrekturabzug-Workflows reibungslos funktionieren.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->

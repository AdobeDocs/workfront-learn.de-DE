---
title: Grundlegendes zu Korrekturabzugsdetails
description: Dringen Sie tiefer in die Details eines Korrekturabzugs in [!DNL  Workfront] über das Bedienfeld „Zusammenfassung“ und die Seite [!UICONTROL Dokumentdetails] ein.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: cb72c429f0ef4cd9945282876aa49189dab1bd96
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 57%

---

# Grundlegendes zu Korrekturabzugsdetails

## Anzeigen von Korrekturabzugsdetails

Als Managerin bzw. Manager oder Inhaberin bzw. Inhaber eines Korrekturabzugs können Sie über das Bedienfeld „Zusammenfassung“ und die Seite [!UICONTROL Dokumentdetails] weitere Informationen zu einem Korrekturabzug erhalten. Suchen Sie zunächst nach Ihrem Korrekturabzug im Abschnitt [!UICONTROL Dokumente] eines Projekts, einer Aufgabe oder eines Problems.

### Bedienfeld „Zusammenfassung“

Wählen Sie einen Testversand aus der Dokumentliste aus und klicken Sie dann oben rechts im Bildschirm auf das Symbol Zusammenfassung .

![Ein Bild des Bereichs [!UICONTROL Dokumente] eines Projekts mit ausgewähltem Testversand.](assets/document-summary-1.png)

Klicken Sie anschließend auf Übersicht , um den Übersichtsabschnitt zu erweitern.

![Ein Bild des Abschnitts [!UICONTROL Dokumente] eines Projekts mit ausgewähltem Korrekturabzug und erweitertem Bedienfeld „Zusammenfassung“. Sowohl das Bedienfeld „Zusammenfassung“ als auch das Symbol für das Bedienfeld sind hervorgehoben.](assets/document-summary-2.png)

Scrollen Sie dann nach unten zum Abschnitt Testversand . Hier sehen Sie den Testversand-Eigentümer, den Fortschritt, die Anzahl der Kommentare, den Status und das Fälligkeitsdatum.

![Ein Bild des Abschnitts [!UICONTROL Dokumente] eines Projekts mit ausgewähltem Korrekturabzug und erweitertem Bedienfeld „Zusammenfassung“. Sowohl das Bedienfeld „Zusammenfassung“ als auch das Symbol für das Bedienfeld sind hervorgehoben.](assets/document-summary-3.png)

Hinweis: Der Abschnitt &quot;[!UICONTROL Genehmigungen]&quot;im Zusammenfassungsbereich dient für Genehmigungen für das Dokument **Dokument** und **ist nicht** an den Prozess zur Überprüfung und Genehmigung des Testversands gebunden. Die beiden Prozesse sind in [!DNL Workfront] voneinander getrennt.

### [!UICONTROL Dokumentdetails]

Um weitere Informationen zum Testversand zu erhalten, klicken Sie auf [!UICONTROL Dokumentdetails].

![Ein Bild des Bereichs [!UICONTROL Dokumente] eines Projekts mit einem ausgewählten Testversand und [!UICONTROL Dokumentdetails] hervorgehoben.](assets/document-summary-4.png)

Dadurch gelangen Sie zur Seite [!UICONTROL Dokumentdetails] und erhalten im linken Bereich eine Reihe weiterer Optionen.

![Ein Bild der Seite des Korrekturabzugs in [!DNL  Workfront].](assets/document-details.png)

Beachten Sie, dass die Möglichkeit, Informationen zum Testprozess anzuzeigen, von Ihren Testberechtigungen in [!DNL Workfront] abhängt.

Auf der Seite des Testversands können Sie über das Menü im linken Bedienfeld auf folgende Bereiche zugreifen:

* **Aktualisierungen —** Kommentare, die im Testversand-Viewer gemacht wurden, werden hier mit dem Tag &quot;Testversand-Kommentar&quot;angezeigt. Sie können auch Kommentare zur Datei abgeben, genau wie Sie Kommentare zu einer Aufgabe oder einem Projekt abgeben (diese Kommentare erscheinen nicht im Korrekturabzug-Viewer).
* **Genehmigungen** – Dieser Abschnitt ist für Dokumentgenehmigungen und nicht für Proofing-Genehmigungen bestimmt. Die beiden Arten von Genehmigungen sind separate Prozesse in [!DNL Workfront] und sind nicht miteinander verknüpft. Wenn Sie Testversand-Workflows für Ihre Überprüfungen und Genehmigungen verwenden, wird dieser Abschnitt nicht verwendet.
* **Alle Versionen** – Verfolgen und verwalten Sie den Versionsverlauf des Korrekturabzugs. Möglicherweise ist es einfacher für Sie, auf diese Informationen im Bedienfeld „Zusammenfassung“ der Liste [!UICONTROL Dokumente] zuzugreifen.
* **Benutzerdefinierte Formulare** – Benutzerdefinierte Formulare werden bei Korrekturabzügen verwendet, um unternehmensspezifische Informationen zu erfassen. Diese Informationen können mit der Datei an integrierte Dokumentenspeichersysteme wie [!DNL Workfront] DAM oder Adobe Experience Manager übergeben werden. Benutzerdefinierte Formulare werden von Ihren System- oder Gruppenadmins für [!DNL Workfront] eingerichtet. Sprechen Sie mit Ihrem Team oder Ihren Admins, um zu erfahren, ob Sie benutzerdefinierte Formulare für Korrekturabzüge verwenden werden.
* **Proofing-Workflow** – Verwalten oder ändern Sie den Workflow, der dem Korrekturabzug zugewiesen ist. Sie können dieses Fenster auch über den Link [!UICONTROL Testversand-Workflow] auf dem Testversand in der Liste [!UICONTROL Dokumente] öffnen.

Sehen wir uns zwei der Abschnitte genauer an: [!UICONTROL Testen der Viewer-Einstellungen] und [!UICONTROL Testen der Aktivität].

### [!UICONTROL Proofing-Viewer-Einstellungen]

Mithilfe dieser Einstellungen können Sie den Zugriff auf den Korrekturabzug selbst steuern.

![Ein Bild der [!UICONTROL Proofing-Viewer-Einstellungen] auf der Seite des Korrekturabzugs, mit Hervorhebung der Option [!UICONTROL Proofing-Viewer-Einstellungen] im Menü des linken Bedienfelds.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Anmeldung erforderlich. Dieser Korrekturabzug kann nicht für Gastbenutzerinnen und Gastbenutzer freigegeben werden]** – Der Korrekturabzug kann nur für Personen freigegeben werden, die über eine [!DNL Workfront]-Proofing-Lizenz verfügen.
* **[!UICONTROL Erfordert die elektronische Unterzeichnung von Entscheidungen] —** Bei der Freigabe eines Testversands erfordert dies, dass der Empfänger über Testversandberechtigungen in [!DNL Workfront] verfügt und ihn zum &quot;elektronischen Signieren&quot;des Testversands zwingt, indem er bei einer Entscheidung über den Testversand sein Passwort eingibt. (Hinweis: Das Proofing-Passwort ist ein anderes als Ihr [!DNL Workfront]-Passwort. Das Kennwort zum Testen ist nicht leicht zugänglich, sodass die meisten Empfänger dieses Kennwort nicht kennen.) Adobe empfiehlt, mit Ihrem [!DNL Workfront] -Berater zu sprechen, bevor Sie diese Funktion verwenden.
* **[!UICONTROL Korrekturabzug sperren, wenn alle erforderlichen Entscheidungen getroffen sind ]** – Auf diese Weise wird der Korrekturabzug für alle weiteren Kommentare, Antworten, Entscheidungen usw. gesperrt, sobald alle Entscheidungen zu dem Korrekturabzug getroffen sind. Dadurch wird die gesamte Korrekturabzugsversion gesperrt, nicht nur ein bestimmter Schritt des Proofing-Workflows.
* **[!UICONTROL Download der Originaldatei zulassen] —** Testversandempfänger können die Originalquelldatei des Testversands vom Testversand-Viewer herunterladen.
* **[!UICONTROL Freigabe des Korrekturabzugs über öffentliche URL oder Einbettungs-Code zulassen]** – Empfängerinnen und Empfänger eines Korrekturabzugs können für alle einen öffentlich zugänglichen Korrekturabzug-Link freigeben.
* **[!UICONTROL Abonnieren des Korrekturabzugs über öffentliche URL oder Einbettungs-Code zulassen] –** Alle, die die öffentliche URL erhalten, können sich mit E-Mail-Adresse und Name (falls es sich nicht um Benutzende des Korrekturabzugs handelt) bzw. mit E-Mail-Adresse und Proofing-Passwort (falls es sich um eine Benutzerin bzw. einen Benutzer des Proofing handelt) zum Korrekturabzug hinzufügen. (Hinweis: Das Proofing-Passwort ist ein anderes als das [!DNL Workfront]-Passwort.)


### [!UICONTROL Proofing-Aktivität]

Auf dieser Seite werden die gesamten Aktivitäten des Testversands sowie die mit diesem Testversand gesendeten E-Mail-Nachrichten verfolgt.

![Ein Bild des Abschnitts [!UICONTROL Proofing-Aktivität] auf der Seite des Korrekturabzugs mit hervorgehobener [!UICONTROL Proofing-Aktivität] im Menü des linken Bedienfelds.](assets/proofing-activity-in-details.png)

Der Abschnitt **[!UICONTROL Aktivität]** gibt mit einem Zeitstempel an, wann Kommentare verfasst und Entscheidungen getroffen wurden. Zudem wird angegeben, von wem. Es wird auch verfolgt, wann die Schritte des Proofing-Workflows gestartet wurden, wann eine Empfängerin oder ein Empfänger den Korrekturabzug zum ersten Mal geöffnet hat und weitere Informationen, die im Zusammenhang mit Korrekturabzügen relevant sein können. Diese Details können hilfreich sein, wenn Sie Dinge herausfinden möchten, wie z. B. warum eine Workflow-Testphase nie gestartet wurde.

Der Abschnitt **[!UICONTROL Nachrichten]** gibt mit einem Zeitstempel an, wann E-Mail-Warnhinweise und -Nachrichten an Empfängerinnen und Empfänger gesendet wurden, von wem sie gesendet wurden und was die Nachricht enthalten hat. Dies kann bei der Fehlerbehebung hilfreich sein, wenn jemand sagt, dass er keine E-Mail über einen Testversand erhalten hat. Sie können überprüfen, ob und wann eine E-Mail gesendet wurde.

Adobe empfiehlt dem Testversand-Manager und Testversandinhaber, sich mit den Informationen in diesen beiden Abschnitten vertraut zu machen. Wenn Sie diese Informationen mit den Kenntnissen kombinieren, wie Sie die [!UICONTROL SOCD]-Fortschrittsleiste lesen, können Sie Ihre Korrekturabzüge wirklich verstehen und verwalten, unabhängig davon, wo sie sich im Proofing-Workflow befinden.

Nachdem Sie die Arbeit im Abschnitt [!UICONTROL Dokumentdetails] abgeschlossen haben, verwenden Sie die Breadcrumb-Leiste, um zum Abschnitt [!UICONTROL Dokumente] des Projekts, der Aufgabe oder der Ausgabe zurückzukehren, an die der Testversand angehängt ist.

![Ein Bild des Breadcrumb-Pfads in der Kopfzeile.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->

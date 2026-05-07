---
title: Korrekturabzugsbericht
description: Erfahren Sie, wie Sie den Fortschritt der Korrekturabzüge mithilfe der Berichtsfunktionen verwalten können.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
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
autotag-review: '2026-05-05T20:06:01.017Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 454
ht-degree: 100%

---

# Korrekturabzugsbericht

Mit den digitalen Proofing-Funktionen von [!DNL Workfront] können Sie Projekte und die dazugehörigen Überprüfungs-Workflows an einem Ort verwalten – [!DNL Workfront]. Verschaffen Sie sich mit Berichtstypen, Feldquellen und Feldnamen, die Überprüfungs- und Genehmigungsinformationen anzeigen, wertvolle Einblicke in die durchgeführte Proofing-Arbeit.

Wir empfehlen, mit Ihrer [!DNL Workfront]-Beraterin bzw. Ihrem -Berater zusammenzuarbeiten, um Berichte zu erstellen, die den Anforderungen Ihres Unternehmens entsprechen. Einige der Berichte erfordern Kenntnisse im Umgang mit dem Textmodus von [!DNL Workfront].

Beginnen Sie mit diesen grundlegenden Standardberichten, um Ihre Teams bei der Verwaltung von Korrekturabzügen zu unterstützen, die einen Überprüfungs- und Genehmigungsprozess in [!DNL Workfront] durchlaufen.

## [!UICONTROL Korrekturabzug-Genehmigung]

Mit diesem Berichtstyp können Sie ausstehende Korrekturabzugsgenehmigungen verfolgen, um sicherzustellen, dass die Fristen eingehalten werden.

![Wählen Sie [!UICONTROL Korrekturabzug-Genehmigung] aus dem Dropdown-Menü [!UICONTROL Neuer Bericht]](assets/proof-system-setups-proof-approval-report.png)

Zu den Ansichts- und Filteroptionen gehören [!UICONTROL Entscheidungsdatum], [!UICONTROL Korrekturabzug-Genehmigung], [!UICONTROL Genehmigungsstufe], [!UICONTROL Workflow-Vorlage] und [!UICONTROL Informationen zur anfragenden Person]. Bei der Berichterstellung im Textmodus können Sie eine Gruppierung erstellen, die die Liste nach Dokumentennamen organisiert. Siehe [Informationen zum grundlegenden Textmodus für Gruppierungen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=de).

Achten Sie bei der Erstellung von Korrekturabzugsgenehmigungsberichten darauf, dass Sie Ihnen Informationen aus der aktuellsten Version der Korrekturabzüge vorliegen. [!DNL Workfront] empfiehlt, diese Feldquelle und den Feldnamen in den Filter einzuschließen:

**[!UICONTROL Korrekturabzug-Genehmigung]>>[!UICONTROL Ist die aktuelle Version des Dokuments]**

![Registerkarte „Filter“ im Report Builder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Dies ist nützlich, wenn Sie Berichte zu Korrekturabzügen erstellen, die mehrere Versionen haben, damit der Bericht nur die aktuelle Version jedes Korrekturabzugs auflistet, der genehmigt werden muss. Dadurch werden die früheren Versionen herausgefiltert, an denen Sie nicht mehr arbeiten müssen.

## [!UICONTROL Dokumentversion]

Mit diesem Berichtstyp können Sie Versionen in [!DNL Workfront] verwalten und verfolgen.

![Wählen Sie [!UICONTROL Dokumentversion] aus dem Dropdown-Menü [!UICONTROL Neuer Bericht]](assets/proof-system-setups-document-version-report.png)

Zu den Ansichtsoptionen gehören Informationen zu [!UICONTROL Dokumentversion], [!UICONTROL Dokument], [!UICONTROL eingegeben von], [!UICONTROL Status der Korrekturabzug-Genehmigung], [!UICONTROL Erstellerin bzw. Ersteller des Korrekturabzugs] und [!UICONTROL Dokumentanbieter].

Gruppierungen können nach [!UICONTROL Dokumentversion], [!UICONTROL eingegeben von], [!UICONTROL Status der Korrekturabzug-Genehmigung] oder Informationen zur Eigentümerin bzw. zum Eigentümer des Korrekturabzugs vorgenommen werden.

Zu den Filtern gehören [!UICONTROL Dokumentversion], [!UICONTROL Zugriffsebene], [!UICONTROL Dokument], [!UICONTROL eingegeben von], [!UICONTROL Status der Korrekturabzug-Genehmigung], [!UICONTROL Erstellerin bzw. Ersteller des Korrekturabzugs] und Informationen zum Dokumentanbieter.

In dieser Ansichtsspalte können Sie den Namen der Proofing-Stufe anzeigen, die derzeit für jedes Dokument im Bericht aktiv ist:

**[!UICONTROL Dokumentversionen] >> [!UICONTROL Aktive Korrekturabzugsphasen]**

![Registerkarte „Filter“ im Report Builder](assets/proof-system-setups-active-proof-stages.png)

Wenn derzeit keine Phase aktiv ist, ist die Spalte leer.

Feldquelle >> Feldname ist auch als Filter in einem Bericht verfügbar.

Verwenden Sie die Feldquelle [!UICONTROL Erstellerin bzw. Ersteller des Korrekturabzugs], um Informationen über die Person, die den Korrekturabzug erstellt hat, zu melden. Wählen Sie die Feldquelle [!UICONTROL Name], um den Namen der Person, die den Korrekturabzug erstellt hat, in einer Ansicht anzuzeigen.

**[!UICONTROL Erstellerin bzw. Ersteller des Korrekturabzugs] >> [!UICONTROL Name]**

Diese Kombination aus Feldquelle >> Feldname ist auch als Filter verfügbar.

![Registerkarte „Filter“ im Report Builder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->

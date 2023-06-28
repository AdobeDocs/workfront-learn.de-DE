---
title: Grundlegendes zu gruppenspezifischen Validierungsprozessen
description: Erfahren Sie, wie Gruppenadministratoren Genehmigungsprozesse für die von ihnen verwalteten Gruppen erstellen oder bearbeiten können.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Grundlegendes zu gruppenspezifischen Validierungsprozessen

Sowohl System- als auch Gruppenadministratoren können Genehmigungsprozesse in [!DNL Workfront]. Systemadministratoren können Prozesse für die Verwendung im gesamten [!DNL Workfront] -System oder nur für eine bestimmte Gruppe. Gruppenadministratoren können Prozesse nur für die von ihnen verwaltete Gruppe erstellen oder bearbeiten.

Für einen Genehmigungsprozess, der von allen in [!DNL Workfront], stellen Sie sicher, dass [!UICONTROL &quot;Dieser Genehmigungsprozess kann von verwendet werden.&quot;] -Feld auf [!UICONTROL Alle Gruppen].

![[!UICONTROL Genehmigungsprozess bearbeiten] Fenster mit hervorgehobenem Gruppenfeld](assets/admin-fund-approval-processes-1.png)

Die in der [!UICONTROL &quot;Genehmigungsprozess starten, wenn der Status auf festgelegt ist&quot;] -Menü abhängig von der Auswahl im Feld &quot;Verwendet von&quot;. Mit [!UICONTROL Alle Gruppen] ausgewählt wurde, sind nur die systemweit gesperrten Status verfügbar.

Um einen Genehmigungsprozess für eine bestimmte Gruppe zu beschränken, wählen Sie den Namen dieser Gruppe aus der Liste für die [!UICONTROL &quot;Dieser Genehmigungsprozess kann von verwendet werden.&quot;] -Feld.

![[!UICONTROL Genehmigungsprozess bearbeiten] Fenster mit erweitertem Gruppenfeld](assets/admin-fund-approval-processes-2.png)

Die [!UICONTROL Alle Gruppen] ist für Gruppenadministratoren nicht verfügbar.

Wenn eine bestimmte Gruppe ausgewählt wird, werden nur die für diese Gruppe verfügbaren Status in der Variablen [!UICONTROL &quot;Genehmigungsprozess starten, wenn der Status auf festgelegt ist&quot;] Menü.

![[!UICONTROL Genehmigungsprozess bearbeiten] Fenster mit hervorgehobenem Statusfeld](assets/admin-fund-approval-processes-3.png)


---
title: Erstellen und Verwalten von Problemschwerpunkten
description: Erfahren Sie, wie Sie Schwerpunkte von Problemen einrichten und verwalten.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Erstellen und Verwalten von Problemschwerpunkten

## Einführung in Problembereiche

Ein Schweregrad kann verwendet werden, um anzugeben, wie schwerwiegend ein Problem ist oder wie es sich auf die durchgeführte Arbeit auswirken könnte.

![[!UICONTROL Schweregrad] im Menü [!UICONTROL Problemdetails] Fenster](assets/admin-fund-severity-issue-details.png)

Die [!UICONTROL Schweregrad] auf das Feld im [!UICONTROL Problemdetails]. Sie kann auch in Spaltenansichten auf Listen und in benutzerdefinierten Berichten enthalten sein.

[!DNL Workfront] hat fünf Standardschwerpunkte:

* [!UICONTROL Kosmetisch]
* [!UICONTROL Verwirrend]
* [!UICONTROL Programmfehler mit Umgehungslösung]
* [!UICONTROL Programmfehler ohne Umgehungslösung]
* [!UICONTROL Schwerer Fehler]

Systemadministratoren können diese Standardabstufungen umbenennen oder bei Bedarf neue erstellen.

Prioritätsstufen sind nur für Probleme verfügbar in [!DNL Workfront].

## Erstellen und Verwalten von Problemschwerpunkten

Als Systemadministrator können Sie bei Bedarf neue Abläufe erstellen, um den Workflow des Problems abzuschließen.

![[!UICONTROL Schweregrad] Seite in [!UICONTROL Einrichtung]](assets/admin-fund-severity-section.png)

1. Klicken **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** im linken Menübereich.
1. Auswählen **[!UICONTROL Schweregrad]**.
1. Klicken **[!UICONTROL Neuen Schweregrad hinzufügen]**.
1. Geben Sie dem Schweregrad einen Namen, der dem vorgesehenen Verwendungszweck entspricht.
1. Die **[!UICONTROL Wichtigkeit]** Zahl entspricht der Schwere des Problems. Die höchste Zahl entspricht dem höchsten Schweregrad. Die [!UICONTROL Wichtigkeit] number muss eindeutig sein.
1. Wählen Sie eine Farbe für Ihre Priorität aus. Dies wird in Diagrammberichten und an anderen Stellen in [!DNL Workfront].
1. Legen Sie eine der Prioritätsoptionen als **[!UICONTROL Standardschweregrad]**. Dies wird automatisch auf alle neuen Probleme in Workfront angewendet.
1. Geben Sie eine Beschreibung des Schweregrads an, z. B. wie dieser verwendet werden soll.
1. Klicken Sie auf eine Stelle außerhalb der zu speichernden Felder.

![[!UICONTROL Schweregrad] Liste](assets/admin-fund-severity-new.png)

### Ändern von Schwerpunkten

Wenn ein Schweregrad nicht mehr für Ihre Problem-Workflows relevant wird, kann er umbenannt, ausgeblendet oder gelöscht werden.

Wenn ein Schweregrad nicht mehr benötigt wird, [!DNL Workfront] empfiehlt, den Schweregrad auszublenden (klicken Sie auf die Schaltfläche [!UICONTROL Ausblenden] neben dem Feld im Setup-Bereich). Dadurch wird die Prioritätsoption zum Problem aus dem Dropdown-Menü entfernt, aber der Schweregrad historischer Daten wird beibehalten, sodass sie weiterhin zu Berichtszwecken verfügbar sind.

![[!UICONTROL Ausblenden] Spalte hervorgehoben [!UICONTROL Schweregrad] Seite in [!UICONTROL Einrichtung]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] empfiehlt, **nicht** Löschen Sie einen Schweregrad, der bereits bei Problemen verwendet wurde. Wenn Sie einen Schweregrad löschen, werden Sie aufgefordert, einen anderen Schweregrad zu ersetzen. Dies kann historische Daten ändern und die Berichterstellung beeinflussen.

![Fenster &quot;Schweregrad löschen&quot;](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->

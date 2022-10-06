---
title: Systemweite Problemstatus anpassen
description: Erfahren Sie, wie Sie die Namen des Problemstatus ändern, die Problemtypen, für die ein Status verwendet wird, steuern und die Status für die Anpassung auf Gruppenebene sperren/entsperren.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Systemweite Status anpassen

[!DNL Workfront] bietet eine Vielzahl von Standardstatuen, um die Problemmanagement-Workflows Ihres Unternehmens zu berücksichtigen. Diese Status können in die Terminologie Ihres Unternehmens umbenannt werden. Und Status können bestimmten Problemtypen zugewiesen werden.

Bei Bedarf können weitere Status erstellt werden. Nur Systemadministratoren können systemweite Status erstellen. Darüber hinaus steuern Systemadministratoren, welche Status von Gruppenadministratoren bearbeitet werden können.

![[!UICONTROL Probleme] Registerkarte auf [!UICONTROL Status] Seite in [!UICONTROL Einrichtung]](assets/admin-fund-all-issue-statuses.png)

## Vorhandenen Status ändern

[!DNL Workfront] empfiehlt eine Mindestanzahl von Status. Dies erleichtert die Auswahl des richtigen Status für Benutzer und führt zu einer kürzeren Liste der beizubehaltenden Status.

Sie können einen vorhandenen Status bearbeiten, um den Namen, die zugewiesenen Problemtypen, die zugehörige Farbe usw. zu ändern.

![Problemstatus-Liste mit [!UICONTROL Bearbeiten] Option hervorgehoben](assets/admin-fund-edit-issue-status.png)

1. Klicken **[!UICONTROL Einrichtung]** im **[!UICONTROL Hauptmenü]**.
1. Erweitern Sie die **[!UICONTROL Projektvoreinstellungen]** im linken Menübereich.
1. Auswählen **[!UICONTROL Status]**.
1. Wählen Sie die **[!UICONTROL Probleme]** Registerkarte und stellen Sie sicher, dass [!UICONTROL Systemstatus] in der oberen rechten Ecke angezeigt.
1. Auswählen **[!UICONTROL Übergeordnete Liste]** um die Status für alle Ausgabetypen anzuzeigen. Hier können Sie einen Problemstatus erstellen oder ändern.
1. Bewegen Sie den Mauszeiger über die rechte Seite des Status, den Sie umbenennen möchten, und klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Benennen Sie den Status neu oder ändern Sie ggf. andere Informationen.
1. Sperren Sie den Status, wenn diese Einstellungen für alle Benutzer in Ihrer [!DNL Workfront] -Instanz.
1. Entsperren Sie den Status, damit Gruppenadministratoren den Status nur für ihre Gruppen bearbeiten können.
1. Markieren Sie die Kästchen für den Problemtyp, auf den der Status angewendet werden soll.
1. Klicken **[!UICONTROL Speichern]**.

![Fenster zum Erstellen eines neuen Status](assets/admin-fund-edit-issue-status-2.png)

### Statuszuweisungen

Es können nicht alle Status allen Ausgabetypen zugewiesen werden. Die [!UICONTROL Status] Seite enthält Spalten, die zeigen, für welchen Problemtyp jeder Status verwendet werden kann.

![Auf der Registerkarte &quot;Probleme&quot;der Seite &quot;Status&quot;hervorgehobene Reihenfolge ändern](assets/admin-fund-issue-type-statuses.png)


Um nur die einem bestimmten Problemtyp zugewiesenen Status anzuzeigen, klicken Sie einfach oben im Fenster auf den Namen des Problemtyps.

![[!UICONTROL Problem] Tab von [!UICONTROL Status] Seite mit hervorgehobenen Spalten](assets/admin-fund-statuses-issue-type.png)

Von hier aus können Sie die Probleme in die Reihenfolge ziehen, in der sie im [!UICONTROL Status] Dropdown-Menü.

Um die Status zu bearbeiten, müssen Sie zum [!UICONTROL Übergeordnete Liste].

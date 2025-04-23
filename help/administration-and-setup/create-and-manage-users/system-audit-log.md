---
title: Grundlegendes zum Systemadministratorprotokoll
description: Erfahren Sie, wie Sie mithilfe des Systemadministratorprotokolls überprüfen können, wann Änderungen vorgenommen wurden und wann sie in die Elemente eingehen.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 100%

---

# Grundlegendes zum Systemadministratorprotokoll

Das Systemadministratorprotokoll ist das beste Mittel für Systemadmins, die Vorgänge in [!DNL Workfront] im Auge zu behalten. Betrachten Sie das Protokoll als die zentrale Informationsquelle darüber, wer wann welche Änderungen vorgenommen hat.

Sie können das Administratorprotokoll über den Abschnitt [!UICONTROL Voreinstellungen] im Bereich [!UICONTROL Setup] aufrufen. Standardmäßig werden die Daten der letzten sieben Tage angezeigt. Ändern Sie die Filterkriterien, um Daten aus verschiedenen Datumsbereichen anzuzeigen.

Bei der Durchführung bestimmter Aktionen zeichnet [!UICONTROL Workfront] diese im Abschnitt [!UICONTROL Administratorprotokolle] des Bereichs [!UICONTROL Setup] auf.

Das Dropdown-Menü ![[!UICONTROL Protokolltyp] auf der Seite [!UICONTROL Administratorprotokolle] unter [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

Jede aufgezeichnete bzw. protokollierte Aktion wird mit folgenden Informationen angezeigt:

* Datum und Uhrzeit der Änderung
* Protokolltyp
* Name der Person, die die Aktion abgeschlossen hat
* Objekt
* Alle mit der Aktion verbundenen Details
* IP-Adresse

![[!UICONTROL Administratorprotokoll] als Liste](assets/admin-fund-audit-log-2.JPG)

## Exportieren des Administratorprotokolls

Durch den Export der Administratorprotokolldaten können Systemadmins die Informationen für internes/externes Prüfpersonal oder Sicherheitsfachleute freigeben. Einige Unternehmen verlangen die Aufbewahrung bestimmter Protokolle zur Einhaltung der Cybersicherheitsvorschriften. Andere benötigen die in ein Sicherheitssystem importierten Informationen zur Analyse.

Administratorprotokolle können in eine CSV-Datei (kommagetrennte Werte) exportiert werden, die in einem Tabellenkalkulationsprogramm oder einem Texteditor geöffnet werden kann. Der Export ist auf jeweils 50.000 Zeilen begrenzt. Verwenden Sie daher die Filter, um die Liste einzugrenzen, wenn die Gesamtzahl 50.000 übersteigt.

Schaltfläche ![[!UICONTROL Exportieren] auf der Seite [!UICONTROL Administratorprotokolle]](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->

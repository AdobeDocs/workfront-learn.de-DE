---
title: Grundlegendes zum System-Auditprotokoll
description: Erfahren Sie, wie Sie mithilfe des Systemprüfungsprotokolls überprüfen können, wann Änderungen vorgenommen wurden und wann Artikel bearbeitet werden.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Informationen zum Systemprüfungsprotokoll

Das System-Auditprotokoll ist der beste Weg, um die Vorgänge im Auge zu behalten [!DNL Workfront]. Stellen Sie sich das Protokoll als Ihre Quelle der Wahrheit vor, für wen, welche Änderungen vorgenommen wurden und wann.

Rufen Sie das Auditprotokoll auf, indem Sie zum [!UICONTROL Voreinstellungen] im Abschnitt [!UICONTROL Einrichtung] Bereich. Standardmäßig werden Daten aus den letzten sieben Tagen angezeigt. Ändern Sie die Filterkriterien, um Daten aus verschiedenen Datumsbereichen anzuzeigen.

Wenn ein Benutzer bestimmte Aktionen ausführt, [!UICONTROL Workfront] erfasst sie in [!UICONTROL Auditprotokolle] Abschnitt [!UICONTROL Einrichtung] Bereich.

![[!UICONTROL Protokolltyp] Dropdown-Menü auf der [!UICONTROL Auditprotokolle] Seite in [!UICONTROL Einrichtung]](assets/admin-fund-audit-log-1.png)

Jede aufgezeichnete oder protokollierte Aktion zeigt Folgendes:

* Datum und Uhrzeit der Änderung
* Der Protokolltyp
* Der Name des Benutzers, der die Aktion abgeschlossen hat
* Das Objekt
* Alle Details, die mit der Aktion verknüpft sind
* Die IP-Adresse

![[!UICONTROL Auditprotokoll] Liste](assets/admin-fund-audit-log-2.JPG)

## Exportieren des Auditprotokolls

Durch den Export der Auditprotokolldaten können Systemadministratoren die Informationen an interne/externe Prüfer oder Sicherheitsspezialisten weitergeben. Einige Unternehmen verlangen, dass bestimmte Protokolle aufbewahrt werden, um die Vorschriften zur Cybersicherheit einzuhalten. Andere benötigen die in ein Sicherheitssystem importierten Informationen zur Analyse.

Audit-Protokolle können in eine CSV-Datei (kommagetrennte Werte) exportiert werden, die in eine Tabellenkalkulationsanwendung oder einen Texteditor geöffnet werden kann. Der Export ist auf 50.000 Zeilen gleichzeitig beschränkt. Verwenden Sie daher die Filter, um die Liste einzuschränken, wenn die Gesamtzahl 50.000 überschreitet.

![[!UICONTROL Export] Schaltfläche auf [!UICONTROL Auditprotokolle] page](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->

---
title: Einrichten von Ereignisbenachrichtigungen
description: Erfahren Sie, wie Sie steuern können, welche E-Mail- und In-App-Benachrichtigungen Benutzer erhalten, indem Sie Ereignisbenachrichtigungen verwalten.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Einrichten von Ereignisbenachrichtigungen

>[!NOTE]
>
>Aufgrund eines schrittweisen Rollouts ist die Funktionalität, die es System- und Gruppenadministratoren ermöglicht, Ereignisbenachrichtigungen zu verwalten, vorübergehend für einige nicht verfügbar [!DNL Workfront] -Kunden. In diesem Artikel finden Sie aktuelle Informationen zu dieser Version: Entsperren Sie die Konfiguration von Ereignisbenachrichtigungen für Gruppen.

Systemadministratoren legen fest, welche Benachrichtigungen Benutzer erhalten sollen [!DNL Workfront].

![[!UICONTROL E-Mail-Benachrichtigungen] im Fenster [!UICONTROL Einrichtung] area](assets/admin-fund-notifications-1.png)

Die [!UICONTROL Ereignisbenachrichtigungen] Liste nach Typ gruppiert. Für jede aufgelistete Ereignisbenachrichtigung werden fünf Informationen angezeigt:

* **[!UICONTROL Aktiv] —** Die [!UICONTROL Aktiv] können Sie eine Benachrichtigung systemweit aktivieren oder deaktivieren.
* **[!UICONTROL Name] —** Dies ist der Name der Benachrichtigung in [!DNL Workfront].
* **[!UICONTROL Beschreibung] —** In der Beschreibung wird kurz erläutert, welche Maßnahmen ergriffen wurden, um eine Benachrichtigung Trigger, oder welche Maßnahmen als Reaktion auf den Erhalt der Benachrichtigung getroffen werden müssen.
* **[!UICONTROL Email Subject] —** Was dem Benutzer in der Betreffzeile angezeigt wird, wenn die E-Mail an Benutzer gesendet wird.
* **[!UICONTROL Gruppenzugriff] —** Entsperren Sie Benachrichtigungen, damit sie von Gruppenadministratoren verwaltet werden können.

## Benachrichtigungen aktivieren

Um Benachrichtigungen auf globaler Systemebene zu verwalten, stellen Sie sicher, dass in der Suchleiste [!UICONTROL Systemereignisbenachrichtigungen].

Aktivieren Sie eine bestimmte Benachrichtigung, um sie für alle Benutzer verfügbar zu machen, indem Sie auf die Umschalter-Schaltfläche klicken, damit das blaue Feld angezeigt wird. Wenn das Blau ausgeblendet ist, ist die Benachrichtigung deaktiviert.

![[!UICONTROL Aktiv] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/admin-fund-notifications-2.png)

Nach Aktivierung einer Ereignisbenachrichtigung werden Nachrichten sofort gesendet, wenn das Ereignis eintritt.

## Verwaltung von Gruppenadministratoren zulassen

Gruppenadministratoren können von Systemadministratoren die Erlaubnis erhalten, die Benachrichtigungsliste je nach der Funktionsweise ihrer Gruppen und Untergruppen und den Workflows weiter anzupassen.

![[!UICONTROL Gruppenzugriff] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/ganotifications_01.png)

Damit Gruppenadministratoren Benachrichtigungen für ihre Gruppen und Untergruppen verwalten können, müssen die Benachrichtigungen auf Systemebene entsperrt werden.

* Navigieren Sie auf der Seite E-Mail-Benachrichtigungen zur Registerkarte Ereignisbenachrichtigung .

* Stellen Sie sicher, dass in der Suchleiste Systemereignisbenachrichtigungen aufgeführt sind.

* Entsperren Sie eine einzelne Benachrichtigung für alle Gruppenadministratoren, indem Sie in der Spalte Gruppenzugriff auf den Umschalter klicken, damit das blaue Symbol angezeigt wird.

* Entsperren Sie mehrere Benachrichtigungen gleichzeitig, indem Sie das Kontrollkästchen links neben jeder Benachrichtigung aktivieren und in der Symbolleiste oberhalb der Liste auf das Symbol Entsperren klicken.

![[!UICONTROL Gruppenzugriff] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/ganotifications_02.png)

Sperren Sie eine entsperrte Benachrichtigung, indem Sie auf den Umschalter klicken, damit die graue Meldung angezeigt wird. Sperren Sie mehrere Benachrichtigungen gleichzeitig, indem Sie die Kontrollkästchen aktivieren und in der Symbolleiste auf das Symbol Entsperren klicken.

![[!UICONTROL Gruppenzugriff] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/ganotifications_03.png)

Entsperrte Benachrichtigungen werden für Gruppenadministratoren der obersten Ebene angezeigt, um zu bestimmen, ob diese Benachrichtigung für ihre Gruppen und Untergruppen erforderlich ist. Untergruppen übernehmen die Benachrichtigungskonfigurationen von ihrer obersten übergeordneten Gruppe. ﻿


## Gruppenbenachrichtigungen verwalten

Sobald der Systemadministrator über die Optionen für entsperrte Benachrichtigungen verfügt, können Gruppenadministratoren die Benachrichtigungen einer Gruppe von der Seite &quot;Gruppe&quot;aus verwalten, indem sie im Menü des linken Bedienfelds auf Ereignisbenachrichtigungen klicken. Anschließend können Sie Benachrichtigungsoptionen aktivieren oder deaktivieren.

![[!UICONTROL Gruppenzugriff] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/managegroupnotifications_01.png)

Bei Bedarf können Systemadministratoren die Benachrichtigungen einer Gruppe von der Seite Benachrichtigungen aus verwalten, indem sie den Gruppennamen in die Suchleiste am oberen Rand des Fensters eingeben.

![[!UICONTROL Gruppenzugriff] Spalte auf [!UICONTROL E-Mail-Benachrichtigungen] page](assets/managegroupnotifications_02.png)

## Pro-Tipps

Es gibt einige Benachrichtigungen [!DNL Workfront] empfiehlt, den Benutzern zur Verfügung zu stellen.

Für die meisten Benutzer:

* [!UICONTROL Wenn eine Aufgabe abgeschlossen ist, die primär zugewiesenen Benutzer aller abhängigen Aufgaben per E-Mail benachrichtigen.]
* [!UICONTROL Jemand hat mich in die direkte Aktualisierung einbezogen]
* [!UICONTROL Jemand kommentiert meinen Arbeitselement]
* [!UICONTROL Das Fälligkeitsdatum ändert sich bei einer Aufgabe, der ich zugewiesen bin]


Insbesondere für Projektmanager:

* [!UICONTROL Ein Projekt, an dem ich arbeite, wird aktiv]
* [!UICONTROL Ein Projekt, das in meinem Besitz ist, ist in Verzug geraten.]
* [!UICONTROL Ein Problem wird einem Projekt in meinem Besitz hinzugefügt]
* [!UICONTROL Meilensteinaufgabe für ein Projekt abgeschlossen, dessen Eigentümer ich bin]

<!---
learn more URLs
--->

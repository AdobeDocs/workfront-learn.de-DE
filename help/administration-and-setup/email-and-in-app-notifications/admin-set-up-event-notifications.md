---
title: Einrichten von Ereignisbenachrichtigungen
description: Erfahren Sie, wie Sie steuern können, welche E-Mail- und In-App-Benachrichtigungen Benutzer und Benutzerinnen erhalten, indem Sie Ereignisbenachrichtigungen verwalten.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: ht
source-wordcount: '622'
ht-degree: 100%

---

<!--
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
-->

<!--
add URL link in the note at the top of the LP
-->

# Einrichten von Ereignisbenachrichtigungen

>[!NOTE]
>
>Aufgrund eines schrittweisen Rollouts ist die Funktionalität, die es System- und Gruppenadmins ermöglicht, Ereignisbenachrichtigungen zu verwalten, vorübergehend für einige [!DNL Workfront]-Kundinnen und -Kunden nicht verfügbar. In diesem Artikel finden Sie Aktualisierungen bezüglich der Version: Entsperren der Konfiguration von Ereignisbenachrichtigungen für Gruppen.

Systemadmins legen fest, welche Benachrichtigungen Benutzer und Benutzerinnen erhalten sollen [!DNL Workfront].

![[!UICONTROL E-Mail-Benachrichtigungen] im Bereich [!UICONTROL Setup]](assets/admin-fund-notifications-1.png)

Die Liste der [!UICONTROL Ereignisbenachrichtigungen] ist nach Typ gruppiert. Für jede aufgelistete Ereignisbenachrichtigung werden fünf Informationen angezeigt:

* **[!UICONTROL Aktiv]:** Mit der Spalte [!UICONTROL Aktiv] können Sie eine Benachrichtigung systemweit aktivieren oder deaktivieren.
* **[!UICONTROL Name]:** Dies ist der Name der Benachrichtigung in [!DNL Workfront].
* **[!UICONTROL Beschreibung]:** In der Beschreibung wird kurz erläutert, welche Maßnahmen ergriffen wurden, um eine Benachrichtigung auszulösen, oder welche Maßnahmen als Reaktion auf den Erhalt der Benachrichtigung getroffen werden müssen.
* **[!UICONTROL E-Mail-Betreff]:** Was in der Betreffzeile angezeigt wird, wenn die E-Mail an Benutzer und Benutzerinnen gesendet wird.
* **[!UICONTROL Gruppenzugriff]:** Entsperren Sie Benachrichtigungen, damit sie von Gruppenadmins verwaltet werden können.

## Aktivieren von Benachrichtigungen

Um Benachrichtigungen auf globaler Systemebene zu verwalten, stellen Sie sicher, dass auf der Suchleiste [!UICONTROL Systemereignisbenachrichtigungen] angezeigt wird.

Aktivieren Sie eine bestimmte Benachrichtigung, um sie für alle Benutzenden verfügbar zu machen, indem Sie auf die Umschaltfläche klicken, damit das Blau angezeigt wird. Wenn das Blau ausgeblendet ist, ist die Benachrichtigung deaktiviert.

Die Spalte ![[!UICONTROL Aktiv] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/admin-fund-notifications-2.png)

Nach der Aktivierung einer Ereignisbenachrichtigung werden Nachrichten sofort gesendet, wenn das Ereignis eintritt.

## Zulassen der Verwaltung durch Gruppenadmins

Gruppenadmins können von Systemadmins die Berechtigung erhalten, die Benachrichtigungsliste je nach Funktionsweise ihrer Gruppen und Untergruppen und den Workflows weiter anzupassen.

Die Spalte ![[!UICONTROL Gruppenzugriff] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/ganotifications_01.png)

Damit Gruppenadmins Benachrichtigungen für ihre Gruppen und Untergruppen verwalten können, müssen die Benachrichtigungen auf Systemebene entsperrt werden.

* Navigieren Sie dazu auf der Seite „E-Mail-Benachrichtigungen“ zur Registerkarte „Ereignisbenachrichtigung“.

* Stellen Sie sicher, dass in der Suchleiste „Systemereignisbenachrichtigungen“ angezeigt wird.

* Entsperren Sie eine einzelne Benachrichtigung für alle Gruppenadmins, indem Sie in der Spalte „Gruppenzugriff“ auf den Umschalter klicken, sodass das Symbol in Blau angezeigt wird.

* Entsperren Sie mehrere Benachrichtigungen gleichzeitig, indem Sie das Kontrollkästchen links neben jeder Benachrichtigung aktivieren und in der Symbolleiste über der Liste auf das Symbol zum Entsperren klicken.

Die Spalte ![[!UICONTROL Gruppenzugriff] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/ganotifications_02.png)

Sperren Sie eine entsperrte Benachrichtigung, indem Sie auf den Umschalter klicken, sodass das Symbol in Grau angezeigt wird. Sperren Sie mehrere Benachrichtigungen gleichzeitig, indem Sie die Kontrollkästchen aktivieren und dann in der Symbolleiste auf das Symbol zum Entsperren klicken.

Die Spalte ![[!UICONTROL Gruppenzugriff] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/ganotifications_03.png)

Entsperrte Benachrichtigungen werden für Gruppenadmins der obersten Ebene angezeigt, damit sie bestimmen können, ob diese Benachrichtigung für ihre Gruppen und Untergruppen erforderlich ist. Untergruppen übernehmen die Benachrichtigungskonfigurationen von der jeweiligen obersten übergeordneten Gruppe. ﻿


## Verwalten von Gruppenbenachrichtigungen

Sobald die Systemadmins Benachrichtigungsoptionen entsperrt haben, können Gruppenadmins die Benachrichtigungen einer Gruppe über die Seite der einzelnen Gruppe verwalten, indem sie im Menü des linken Bedienfelds auf „Ereignisbenachrichtigungen“ klicken. Anschließend können Sie Benachrichtigungsoptionen aktivieren oder deaktivieren.

Die Spalte ![[!UICONTROL Gruppenzugriff] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/managegroupnotifications_01.png)

Bei Bedarf können Systemadmins die Benachrichtigungen einer Gruppe auf der Seite „Benachrichtigungen“ verwalten, indem sie den Gruppennamen in die Suchleiste oben im Fenster eingeben.

Die Spalte ![[!UICONTROL Gruppenzugriff] auf der Seite [!UICONTROL E-Mail-Benachrichtigungen]](assets/managegroupnotifications_02.png)

## Profi-Tipps

Es gibt einige Benachrichtigungen in [!DNL Workfront], bei denen empfohlen wird, sie den Benutzenden zur Verfügung zu stellen.

Für die meisten Benutzenden:

* [!UICONTROL Wenn eine Aufgabe abgeschlossen ist, die primär zugewiesenen Benutzer aller abhängigen Aufgaben per E-Mail benachrichtigen]
* [!UICONTROL Jemand bezieht mich in eine gezielte Aktualisierung ein]
* [!UICONTROL Jemand kommentiert mein Arbeitselement]
* [!UICONTROL Das Fälligkeitsdatum einer Aufgabe, der ich zugewiesen bin, wird geändert]


Insbesondere für Projekt-Managerinnen und -Manager:

* [!UICONTROL Ein Projekt, an dem ich mitarbeite, ist jetzt aktiv]
* [!UICONTROL Ein Projekt, das in meinem Besitz ist, ist in Verzug geraten]
* [!UICONTROL Ein Problem wird einem Projekt in meinem Besitz hinzugefügt]
* [!UICONTROL Meilensteinaufgabe ist für ein Projekt, für das ich verantwortlich bin, abgeschlossen]

<!--
learn more URLs
-->

---
title: Grundlegendes zum Finanzzugriff
description: Erfahren Sie, wie Admins mit Finanz-Zugriffsrechten steuern können, wer die in Workfront verfolgten Finanzinformationen anzeigen und bearbeiten kann.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
hide: true
exl-id: ded6b570-3e2a-4372-867d-a370de30dc31
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:01:54.624Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 415
ht-degree: 95%

---

# Informationen zum Finanzzugriff

Wenn Ihr Unternehmen Finanzdaten mit [!DNL Workfront] erfasst, sind Sie als Systemadmin dafür verantwortlich, die Zugriffsrechte für die Anzeige und Bearbeitung dieser Informationen zu schützen und zu verwalten.

Zwei Dinge sind erforderlich, damit eine Person Finanzinformationen anzeigen oder bearbeiten kann:

1. Zugriffsberechtigungen müssen in der [!UICONTROL Zugriffsebene] aktiviert sein.
2. Die Berechtigung zur Nutzung dieser Zugriffsrechte für ein Objekt muss objektabhängig erteilt werden.

Beispielsweise kann einer Person die Berechtigung zum Anzeigen von Finanzdaten in ihrer Zugriffsebene gewährt werden. Sie kann jedoch nur Finanzdaten zu einer Aufgabe anzeigen, die für sie freigegeben ist und bei deren Freigabe außerdem die Finanzansicht aktiviert wurde.

So ist es möglich, dass eine Person, die qua [!UICONTROL Zugriffsebene] zum Einsehen von Finanzdaten berechtigt ist, die Finanzdaten für einige Objekte einsehen kann und für andere nicht, abhängig von den individuellen Freigabeoptionen dieser Objekte. Benutzende können jedoch Finanzen zu einem Objekt nur einsehen, wenn ihnen im Rahmen ihrer [!UICONTROL Zugriffsebene] die entsprechende Berechtigung erteilt wurde.

## Einstellungen der [!UICONTROL Zugriffsebene]

Der allgemeine Zugang zu Finanzdaten wird zunächst durch den [!DNL Workfront]-Lizenztyp gewährt.

**[!UICONTROL Plan]-Lizenzen berechtigen zu Folgendem:**

* Abrechnungseinträge verwalten
* Funktionsbezogene Fakturierung und Kostensätze verwalten und anzeigen
* Benutzerfakturierung und Kostensätze verwalten und anzeigen
* Ausgaben verwalten
* Finanzen anzeigen und bearbeiten

**[!UICONTROL Arbeits]-Lizenzen berechtigen zu Folgendem:**

* Ausgaben verwalten
* Finanzen anzeigen

**[!UICONTROL Überprüfungs]-Lizenzen berechtigen zu Folgendem:**

* Finanzen anzeigen

**Die Berechtigungen können über die [!UICONTROL Zugriffsebene] geändert werden. Die drei Optionen für den Zugriff auf Finanzdaten sind:**

* [!UICONTROL Kein Zugriff] – Die Person kann keine Finanzdaten anzeigen.
* [!UICONTROL Anzeigen] – Die Person kann die Daten überprüfen und freigeben.
* [!UICONTROL Bearbeiten] – Die Person kann die Daten erstellen, bearbeiten, löschen und weitergeben. (Nur für eine Planlizenz verfügbar.)

![Ein Bild mit allgemeinen Finanzdatenoptionen in einer Zugriffsebene](assets/setting-up-finances-8.png)

Beachten Sie, dass die Optionen [!UICONTROL Anzeigen] und [!UICONTROL Bearbeiten] zusätzliche Einstellungen für eine [!UICONTROL Plan]-Lizenz aufweisen. Klicken Sie auf das Zahnrad auf der Schaltfläche [!UICONTROL Anzeigen] für diese Optionen:

**[!UICONTROL Anzeigen]**

* Funktionsbezogene Fakturierung und Kostensätze anzeigen
* Benutzerfakturierung und Kostensätze anzeigen

![Ein Bild mit den Optionen zum Anzeigen der Finanzdaten in einer Zugriffsebene](assets/setting-up-finances-9.png)

**[!UICONTROL Bearbeiten]**

Diese beiden Optionen sind unter der Option [!UICONTROL Bearbeiten] verfügbar, zusammen mit:

* Funktionsbezogene Fakturierung und Kostensätze bearbeiten
* Benutzerfakturierung und Kostensätze bearbeiten

![Ein Bild mit den Bearbeitungsoptionen für Finanzdaten in einer Zugriffsebene](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Eine Person mit der Berechtigung, Ausgaben hinzuzufügen, kann auch die von ihr sowie die von ihrer direkt vorgesetzten Person hinzugefügten Ausgaben einsehen.

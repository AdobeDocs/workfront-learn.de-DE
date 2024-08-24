---
title: Informationen zum Finanzzugriff
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
source-git-commit: d7347d41099e0faf6b47a6fe0e58091105e4e41d
workflow-type: tm+mt
source-wordcount: '415'
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

* Abrechnungsdatensätze verwalten
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

Beachten Sie, dass die Optionen [!UICONTROL Ansicht] und [!UICONTROL Bearbeiten] zusätzliche Einstellungen für eine Lizenz vom Typ [!UICONTROL Plan] aufweisen. Klicken Sie auf das Zahnrad auf der Schaltfläche [!UICONTROL Anzeigen] für diese Optionen:

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

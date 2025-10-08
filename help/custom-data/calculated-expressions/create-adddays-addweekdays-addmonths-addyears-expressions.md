---
title: Erstellen der Ausdrücke ADDDAYS, ADDWEEKDAY, ADDMONTHS und ADDYEARS
description: Erfahren Sie, wie Sie in Adobe [!DNL Workfront]die ADD-Ausdrücke in einem berechneten Feld verwenden und erstellen können.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: ht
source-wordcount: '275'
ht-degree: 100%

---

# Erstellen der Ausdrücke ADDDAYS, ADDWEEKDAY, ADDMONTHS und ADDYEARS

In diesem Video lernen Sie Folgendes:

* Was die Ausdrücke ADDDAYS, ADDWEEKDAY, ADDMONTHS und ADDYEAR berechnen
* Wie ein ADDWEEKDAYS-Datenausdruck in einem berechneten Feld erstellt wird

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops=1)

## Zusätzliche Beispiele

Im Folgenden finden Sie einige zusätzliche ADDDAYS-, ADDWEEKDAY-, ADDMONTHS-, ADDYEAR-Ausdrücke, die Kundinnen und Kunden von Adobe Workfront erstellt haben.

**Hätte abgeschlossen sein sollen bis**

Die Kundin bzw. der Kunde wollte wissen, wann die Aufgabe auf der Grundlage des tatsächlichen Startdatums und der geplanten Dauer hätte abgeschlossen werden sollen. Das geplante Fertigstellungsdatum funktioniert in diesem Fall nicht, da es sich verschieben kann, wenn sich die Aufgabe verspätet, und das geplante Fertigstellungsdatum hilft nicht, wenn es bei früheren Aufgaben zu Verzögerungen kommt.

Der erstellte Ausdruck war „ADDDAYS({actualStartDate},{durationMinutes}/480)“.

Die Zeit im Feld „Dauer“ wird in Minuten gespeichert. In diesem Ausdruck kann das Feld „Dauer“ also nicht allein stehen, wenn die Zeit in Tagen angegeben werden soll. Dazu muss die Dauer durch 480 Minuten (480 Minuten = 8 Stunden = 1 Tag) geteilt werden

Aus diesem Grund enthält der zweite Wertebereich (Dauer/480).


**Fertigstellungsdatum der Rechnung**

In diesem Beispiel wird nicht nur der ADDDAYS-Ausdruck verwendet, sondern auch ein benutzerdefiniertes Feld, das zuvor im benutzerdefinierten Formular erstellt und gespeichert wurde.

Die Kundin bzw. der Kunde erfasst das Datum, an dem eine Rechnung eingereicht wird, über ein benutzerdefiniertes Datumsfeld mit der Bezeichnung „Rechnungsübermittlungsdatum“.

Nach der Übermittlung muss die Rechnung innerhalb von 30 Tagen ausgefüllt und archiviert werden. Um das Fertigstellungs- und Übermittlungsdatum automatisch zu erstellen, wird ein berechnetes ADDDAYS-Feld zusammen mit dem benutzerdefinierten Feld „Rechnungseinreichungsdatum“ verwendet. Der Ausdruck sieht wie folgt aus:

ADDDAYS({DE:Invoice Submission Date},30)

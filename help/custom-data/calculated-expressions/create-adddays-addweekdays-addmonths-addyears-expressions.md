---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-Ausdrücke erstellen
description: Erfahren Sie, wie Sie die ADD-Ausdrücke in einem berechneten Feld in Adobe verwenden und erstellen. [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-Ausdrücke erstellen

In diesem Video erfahren Sie:

* Was die ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-Ausdrücke berechnen
* Erstellen eines ADDWEEKDAYS-Datenausdrucks in einem berechneten Feld

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Zusätzliche Beispiele

Nachstehend finden Sie einige zusätzliche ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-Ausdrücke, die Adobe Workfront-Kunden erstellt haben.

**Hätte**

Der Kunde wollte wissen, wann die Aufgabe basierend auf dem tatsächlichen Startdatum und der geplanten Dauer abgeschlossen sein sollte. Das geplante Abschlussdatum funktioniert in diesem Fall nicht, da es verschoben werden kann, wenn die Aufgabe verspätet ist, und das geplante Abschlussdatum nicht hilfreich ist, wenn es zu Verzögerungen bei früheren Aufgaben kommt.

Der erstellte Ausdruck war ADDDAYS({ISTStartDate},{durationMinutes}/480)

Die Zeit im Feld Dauer wird in Minuten gespeichert. In diesem Ausdruck kann das Feld Dauer also nicht allein stehen, wenn die Zeit in Tagen dargestellt werden soll. Dazu muss die Dauer durch 480 Minuten (480 Minuten = 8 Stunden = 1 Tag) geteilt werden.

Aus diesem Grund enthält der zweite Wertfenster (Dauer/480).


**Rechnungsabschluss**

In diesem Beispiel wird nicht nur der ADDDAYS-Ausdruck verwendet, sondern auch ein benutzerdefiniertes Feld, das zuvor im benutzerdefinierten Formular erstellt und gespeichert wurde.

Der Kunde erfasst das Datum, an dem eine Rechnung über ein benutzerdefiniertes Datumsfeld mit dem Titel &quot;Rechnungsübermittlungsdatum&quot;übermittelt wird.

Nach der Übermittlung muss die Rechnung ausgefüllt und innerhalb von 30 Tagen eingereicht werden. Um dieses Fertigstellungs- und Anmeldedatum automatisch zu erzeugen, wird ein berechnetes ADDDAYS-Feld zusammen mit dem benutzerdefinierten Feld &quot;Rechnungsübermittlungsdatum&quot;verwendet. Der Ausdruck sieht wie folgt aus:

ADDDAYS({DE:Invoice Submission Date},30)

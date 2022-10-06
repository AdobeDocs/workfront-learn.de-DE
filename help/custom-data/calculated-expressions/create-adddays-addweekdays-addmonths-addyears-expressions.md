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
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-Ausdrücke erstellen

In diesem Video erfahren Sie:

* Was die ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-Ausdrücke berechnen
* Erstellen eines ADDWEEKDAYS-Datenausdrucks in einem berechneten Feld

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Zusätzliche Beispiele

Nachstehend finden Sie eine zusätzliche Adobe zu ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-Ausdrücken [!DNL Workfront] -Kunden erstellt haben.

**Hätte**

Der Kunde wollte wissen, wann die Aufgabe basierend auf dem tatsächlichen Startdatum und der geplanten Dauer abgeschlossen sein sollte. Das geplante Abschlussdatum funktioniert in diesem Fall nicht, da es verschoben werden kann, wenn die Aufgabe verspätet ist, und das geplante Abschlussdatum nicht hilfreich ist, wenn es zu Verzögerungen bei früheren Aufgaben kommt.

Der erstellte Ausdruck war ADDDAYS(Tatsächliches Startdatum,(Dauer/480))

Die Zeit im Feld Dauer wird in Minuten gespeichert. In diesem Ausdruck kann das Feld Dauer also nicht allein stehen, wenn die Zeit in Tagen dargestellt werden soll. Dazu muss die Dauer durch 480 Minuten (480 Minuten = 8 Stunden = 1 Tag) geteilt werden.

Aus diesem Grund enthält der zweite Wertfenster (Dauer/480).


**Rechnungsabschluss**

Dieses Beispiel umfasst ein anderes berechnetes Feld, das bereits im System erstellt und gespeichert wurde und sich im Ausdruck befindet.

Der Kunde hat das Datum erfasst, an dem die Rechnung über ein benutzerdefiniertes Datumsfeld mit dem Titel &quot;Rechnungsübermittlungsdatum&quot;im benutzerdefinierten Formular übermittelt wurde. Nach der Übermittlung haben sie 30 Tage Zeit, um die Rechnung auszufüllen und einzureichen. Um dieses Fertigstellungs- und Anmeldedatum automatisch zu erzeugen, wurde ein berechnetes Feld mit ADDDAYS und dem Feld Rechnungsübermittlungsdatum erstellt. Der Ausdruck sah wie folgt aus:

ADDDAYS(Invoice Submission Date,30)

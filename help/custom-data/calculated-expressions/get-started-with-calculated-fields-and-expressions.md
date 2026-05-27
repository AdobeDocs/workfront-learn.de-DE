---
title: Erste Schritte mit berechneten Feldern und Ausdrücken
description: Erfahren Sie, wie Sie Ausdrücke in berechneten Feldern erstellen können, um eindeutige benutzerdefinierte Daten über die Arbeit zu sammeln, die für Ihre Organisation durchgeführt wird.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
TQID: https://experienceleague.adobe.com/M1mfJ1cT5sXOC8-0qJAihKIBAJBHt1hCQJux3o3UEf8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 505
ht-degree: 100%

---

# Erste Schritte mit berechneten Feldern und Ausdrücken

<!--
**Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.
-->

Workfront bietet eine Vielzahl von Feldern, die in verschiedenen Geschäftsbereichen üblich sind und regelmäßig für die Arbeitsverwaltung verwendet werden. Felder wie das geplante Abschlussdatum, das Projekt-Budget, der Name der bzw. des Aufgabenverantwortlichen usw.

Jede Organisation verfügt jedoch über branchen- und unternehmensspezifische Daten, die gesammelt werden müssen, um zu verstehen, ob die Unternehmensziele erreicht werden. Nehmen wir beispielsweise an, Ihre Organisation möchte Folgendes verfolgen:

* Zu welchem Geschäftsbereich ein Projekt beitragen wird.
* Ob die Finanzierung durch Lieferanten, intern oder aus beiden Quellen erfolgt.
* Welche Auflösung für die verwendeten Bilder erforderlich ist.

Obwohl diese Felder nicht von Anfang an in [!DNL Workfront] integriert sind, können Sie benutzerdefinierte Dateneingabefelder und vorausgefüllte Antwortfelder mit Mehrfachauswahl über ein benutzerdefiniertes Formular erstellen.

Der Schwerpunkt dieses Lernpfads liegt auf dem berechneten Feld. Sie erfahren, was ein berechnetes Feld ist, welche verschiedenen Arten von Informationen Sie über Datenausdrücke in das berechnete Feld ziehen können und wie Sie diese berechneten Felder erstellen, um Ihre Datenerfassung und Berichterstellung zu verbessern.

![Setups des Ressourcen-Managements auf einer Seite](assets/GS01.png)

## Was ist ein berechnetes Feld?

In einem berechneten Feld werden benutzerdefinierte Daten gespeichert, die mithilfe von Datenausdrücken und vorhandenen Workfront-Feldern erstellt wurden.

![Workload Balancer mit Nutzungsbericht](assets/GS02.png)

Ihr Unternehmen verfügt beispielsweise über ein spezielles Projekt- oder Arbeitsnummerierungssystem, das die folgenden Daten enthält:

* Jahr der Erstellung des Projekts,
* Initialen der Projektbesitzerin bzw. des -besitzers und
* die [!DNL Workfront]-Projektreferenznummer.


Mithilfe von Ausdrücken in einem berechneten Feld können Sie jede bereits in [!DNL Workfront] gespeicherte Information verwenden und eine eindeutige Projekt-ID oder Arbeitsnummer erstellen, die dann zu einem Bericht wie diesem hinzugefügt werden kann:

![Workload Balancer mit Nutzungsbericht](assets/GS03.png)

Je nach den benötigten Daten können berechnete Felder einfach sein und einen oder zwei Ausdrücke verwenden, oder sie können komplizierter sein und mehrere eingebettete Ausdrücke verwenden. Denken Sie aber daran, dass Workfront für berechnete Felder nur bereits gespeicherte oder in das System abgerufene Daten verwenden kann.

## Textausdrücke

Textausdrücke suchen, zerlegen und kombinieren Informationen in [!DNL Workfront], um aussagekräftigere Daten zu erstellen oder bessere Einblicke in die Arbeit Ihrer Organisation zu erhalten.

Textausdrücke können beispielsweise für Folgendes verwendet werden:

* Anzeigen von „Mehr als 5.000 $“ in einer Spalte einer Projektansicht, wenn die Projektkosten über 5.000 $ liegen, oder von „Unter 5.000 $“, wenn die Ausgaben darunter liegen.

* Geben Sie jedem Projekt eine eindeutige Nummer, die das Jahr der Erstellung des Projekts sowie die [!DNL Workfront]-Referenznummer, den Projektnamen und die Initialen der Person, die das Projekt besitzt, beinhaltet.

* Erstellen Sie einen Bericht, der alle Projekte auflistet, die keinem Portfolio und/oder Programm zugewiesen sind, damit Sie diesen Bericht in Ihren Manager-Sitzungen verwenden können.

Textausdrücke können in einem benutzerdefinierten Feld verwendet werden, um diese Arten von Suchen und Kombinationen in Workfront durchzuführen.

Wenn Sie sich die möglichen Textausdrücke ansehen, finden Sie mehrere Optionen.

![Setups des Ressourcen-Managements auf einer Seite](assets/TE01.png)

Am häufigsten werden sechs Textausdrücke verwendet:

* ZUSAMMENFÜGEN
* LEFT / RIGHT
* CONTAINS
* IF
* ISBLANK
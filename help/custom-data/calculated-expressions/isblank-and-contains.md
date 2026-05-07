---
title: Verwenden der Ausdrücke ISBLANK und CONTAINS
description: Erfahren Sie, wie Sie die Ausdrücke ISBLANK und CONTAINS in einem berechneten Feld in Adobe [!DNL Workfront]verwenden und erstellen.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
TQID: https://experienceleague.adobe.com/q25cuV-wKAkoEJTzDIho1Ab-XTexGhEZCHReoE0TFxg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 400
ht-degree: 97%

---

# Verwenden der Ausdrücke ISBLANK und CONTAINS

Sowohl die CONTAINS- als auch die ISBLANK-Ausdrücke werden verwendet, um einfache true- oder false-Werte bereitzustellen. Der Unterschied besteht darin, dass der ISBLANK-Ausdruck prüft, ob das Feld überhaupt einen Wert enthält, während der CONTAINS-Textausdruck nach einer bestimmten Zeichenfolge in einem Feld sucht.

Um beispielsweise zu sehen, ob ein Projekt eine Beschreibung enthält, verwenden Sie den ISBLANK-Ausdruck. Wenn das Beschreibungsfeld leer ist, gibt der Ausdruck den Wert „true“ zurück. Wenn das Beschreibungsfeld nicht leer ist, wird der Wert „false“ zurückgegeben.

![Workload Balancer mit Nutzungsbericht](assets/isblank01.png)

Um in der Beschreibung nach einem bestimmten Wert zu suchen, z. B. „Wohltätigkeitsveranstaltung“, verwenden Sie den Textausdruck CONTAINS. Wenn in der Beschreibung „Wohltätigkeitsveranstaltung“ gefunden wird, lautet das berechnete Feld „true“. Es wird „false“ angezeigt, wenn kein „Wohltätigkeitsereignis“ gefunden wird.

![Workload Balancer mit Nutzungsbericht](assets/isblank02.png)

## ISBLANK

Der ISBLANK-Textausdruck enthält den Namen des Ausdrucks und einen Datenpunkt.

**ISBLANK({data point})**

![Workload Balancer mit Nutzungsbericht](assets/isblank03.png)

Im obigen Beispiel – wo Sie wissen möchten, ob das Projekt eine Beschreibung enthält – lautet der Ausdruck:

ISBLANK({description})

## CONTAINS

Der Textausdruck CONTAINS enthält den Namen des Ausdrucks, das gesuchte Wort oder die gesuchte Wortgruppe und das Feld, in dem gesucht werden soll.

**CONTAINS(„Phrase“,{fields})**

Stellen Sie sicher, dass Sie das gesuchte Wort oder die gesuchte Wortgruppe in Anführungszeichen setzen. Andernfalls ist der Ausdruck nicht gültig.

Im obigen Beispiel (Suche nach „Wohltätigkeitsveranstaltung“ in der Projektbeschreibung) lautet der Ausdruck:

**CONTAINS(„Wohltätigkeitsveranstaltung“,{description})**

![Workload Balancer mit Nutzungsbericht](assets/isblank04.png)

**Hinweis**: Beim CONTAINS-Ausdruck wird zwischen Groß- und Kleinschreibung unterschieden. Wenn beispielsweise „Wohltätigkeitsveranstaltung“ im Beschreibungsfeld großgeschrieben ist, schreiben Sie diesen Satz im Ausdruck groß.

**CONTAINS(„Wohltätigkeitsveranstaltung“,{description})**

Die Ausdrücke ISBLANK und CONTAINS eignen sich gut, wenn Sie sehen möchten, ob ein Wert überhaupt vorhanden ist. Es kann jedoch nützlicher sein zu wissen, was der Wert ist, ihn tatsächlich zu sehen oder eine Art Deskriptor zu haben, um bessere Einblicke zu erhalten.

Anstatt beispielsweise nur zu wissen, dass ein Projekt aus einer Anfrage konvertiert wurde, möchten Sie den Namen der ursprünglichen Anfrage kennen.

Verwenden Sie in diesem Fall den CONTAINS-Ausdruck in Verbindung mit einem IF-Ausdruck.

In den meisten Fällen werden die Textausdrücke ISBLANK und CONTAINS mit einem IF-Textausdruck verwendet.

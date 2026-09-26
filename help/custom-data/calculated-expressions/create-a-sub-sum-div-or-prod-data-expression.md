---
title: Erstellen eines SUB-, SUM-, DIV- oder PROD-Datenausdrucks
description: Erfahren Sie, wie Sie die grundlegenden mathematischen Ausdrücke in einem berechneten Feld in Adobe [!DNL Workfront] verwenden und erstellen.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
TQID: 'https://experienceleague.adobe.com/tR2rrepkXCZXLuqsLj7ljh377g26f-RQXdE-TMlFkyk'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 95%
---
# Erstellen eines SUB-, SUM-, DIV- oder PROD-Datenausdrucks

In diesem Video lernen Sie Folgendes:

* Funktionsweise der Ausdrücke SUB, SUM, DIV und PROD
* Erstellen eines SUB-Datenausdrucks in einem berechneten Feld

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on&enablevpops=1)

## Zusätzliche Informationen: ROUND-Ausdruck

### Erstellen eines ROUND-Ausdrucks

Der ROUND-Ausdruck rundet eine beliebige Zahl auf eine bestimmte Anzahl von Dezimalstellen.

Meistens wird der ROUND-Datenausdruck in Verbindung mit einem anderen Datenausdruck verwendet und wenn das Formatfeld entweder Text oder Zahl bleibt.

Erstellen wir ein berechnetes Feld, um den Unterschied zwischen den geplanten und tatsächlich erfassten Stunden für eine Aufgabe zu ermitteln, wofür der SUB-Ausdruck erforderlich ist und das wie folgt aussieht:

**SUB({workRequired},{actualWorkRequired})**

Da die Zeit in Minuten verfolgt wird und das bevorzugte Format die Informationen in Stunden anzeigen soll, muss der Ausdruck außerdem durch 60 geteilt werden und damit wie folgt aussehen:

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

Wenn das Format beim Erstellen des berechneten Felds im benutzerdefinierten Formular in „Zahl“ geändert wird, können Sie das Zahlenformat ändern, wenn Sie das Feld zu einer Ansicht hinzufügen.

![Workload Balancer mit Nutzungsbericht](assets/round01.png)

Wenn das Feldformat bei der Erstellung eines benutzerdefinierten Feldes jedoch auf „Text“ eingestellt ist, kann das Format in der Ansicht nicht einfach geändert werden. Es muss der ROUND-Ausdruck verwendet werden, um zu vermeiden, dass in Ihrem Projekt solche Zahlen angezeigt werden:

![Workload Balancer mit Nutzungsbericht](assets/round02.png)

<b>Verwenden des ROUND-Datenausdrucks in einem berechneten Feld</b>

Der ROUND-Ausdruck enthält den Namen des Ausdrucks (ROUND) und in der Regel zwei Datenpunkte. Bei diesen Datenpunkten kann es sich um einen Ausdruck oder ein Feld in Workfront handeln, gefolgt von einer Zahl, die angibt, wie viele Dezimalstellen Sie verwenden möchten.

Ein Ausdruck ist wie folgt strukturiert: ROUND(Datenpunkt, #)

In dem Ausdruck, der die Differenz zwischen Soll- und Ist-Stunden berechnet, verwenden Sie folgenden Ausdruck als ersten Datenpunkt: DIV(SUB({workRequired},{actualWorkRequired}),60). Stellen Sie dann sicher, dass die Zahl, die von diesem Ausdruck stammt, auf höchstens 2 Dezimalstellen gerundet wird.

![Workload Balancer mit Nutzungsbericht](assets/round03.png)

Der Ausdruck könnte wie folgt geschrieben werden: ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2).

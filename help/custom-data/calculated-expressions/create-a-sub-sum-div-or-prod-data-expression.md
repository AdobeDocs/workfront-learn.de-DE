---
title: Erstellen eines untergeordneten, SUM-, DIV- oder PROD-Datenausdrucks
description: Erfahren Sie, wie Sie die mathematischen Grundausdrücke in einem berechneten Feld in Adobe verwenden und erstellen. [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
source-git-commit: 527af78f92f2b85a30de69f31fce7b4b06491bdd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Erstellen eines untergeordneten, SUM-, DIV- oder PROD-Datenausdrucks

In diesem Video erfahren Sie:

* Was die Ausdrücke SUB, SUM, DIV und PROD tun
* Erstellen eines SUB-Datenausdrucks in einem berechneten Feld

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## Zusätzliche Informationen: ROUND-Ausdruck

### Erstellen eines ROUND-Ausdrucks

Der ROUND-Ausdruck nimmt eine beliebige Zahl und rundet sie auf eine bestimmte Anzahl von Dezimalstellen.

Meistens wird der ROUND-Datenausdruck in Verbindung mit einem anderen Datenausdruck verwendet und wenn das Formatfeld entweder Text oder Zahl bleibt.

Erstellen wir ein berechnetes Feld, um den Unterschied zwischen der geplanten und der tatsächlich angemeldeten Anzahl von Stunden für eine Aufgabe zu ermitteln, für die der SUB-Ausdruck erforderlich ist und wie folgt aussieht:

**SUB({workRequired},{ISTWorkRequired})**

Da die Zeit in Minuten verfolgt wird und das bevorzugte Format darin besteht, die Informationen in Stunden anzuzeigen, muss der Ausdruck auch durch 60 geteilt werden und wie folgt aussehen:

**DIV(SUB({workRequired},{ISTWorkRequired}),60)**

Wenn das Format beim Erstellen des berechneten Felds im benutzerdefinierten Formular in Zahl geändert wird, können Sie das Zahlenformat ändern, wenn Sie das Feld in einer Ansicht hinzufügen.

![Lastenausgleich mit Nutzungsbericht](assets/round01.png)

Wenn das Feldformat jedoch beim Erstellen eines benutzerdefinierten Felds als Text beibehalten wird, kann das Format in der Ansicht nicht einfach geändert werden. Der ROUND-Ausdruck muss verwendet werden, um zu vermeiden, dass in Ihrem Projekt solche Zahlen angezeigt werden:

![Lastenausgleich mit Nutzungsbericht](assets/round02.png)

<b>Verwenden des ROUND-Datenausdrucks in einem berechneten Feld</b>

Der ROUND-Ausdruck enthält den Namen des Ausdrucks (ROUND) und normalerweise zwei Datenpunkte. Bei diesen Datenpunkten kann es sich um einen Ausdruck oder ein Feld in Workfront handeln, gefolgt von einer Zahl, die angibt, wie viele Dezimalstellen Sie verwenden möchten.

Ein Ausdruck würde wie folgt strukturiert sein: ROUND(data point, #)

Verwenden Sie in dem Ausdruck, der die Differenz zwischen geplanten und tatsächlichen Stunden berechnet, diesen Ausdruck —DIV(SUB({workRequired},{tatsächlichWorkRequired}),60)—als ersten Datenpunkt. Stellen Sie dann sicher, dass die Zahl, die von diesem Ausdruck stammt, nicht mehr als 2 Stellen rechts von der Dezimalstelle umfasst.

![Lastenausgleich mit Nutzungsbericht](assets/round03.png)

Der Ausdruck könnte wie folgt geschrieben werden: ROUND(DIV(SUB({workRequired},{ISTWorkRequired}),60),2).

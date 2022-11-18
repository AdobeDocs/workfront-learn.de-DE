---
title: Anleitung zu Routern
description: Erfahren Sie, wie Sie mit einem Router Pokemon- oder Superhelden-Bundles den richtigen Pfad unter [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Anleitung zu Routern

## Übersicht

Verwenden Sie einen Router, um Pokemon oder Superhelden den richtigen Pfad zu übergeben und dann eine Aufgabe für jedes Zeichen zu erstellen.

![Ein Bild des Fusion-Szenarios](assets/universal-connectors-and-routing-2.png)

## Anleitung zu Routern

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## Übungs-URLs

* Website der Superhero-API: `https://www.superheroapi.com/`
* Erste URL für Übung: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Zweite URL für Übung: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Wenn Sie Probleme beim Zugriff auf Ihr eigenes Superhero-Token haben, können Sie dieses gemeinsam genutzte Token verwenden: 10110256647253588. Beachten Sie bitte, wie oft Sie die Superhero-API aufrufen, damit dieses gemeinsam genutzte Token für alle weiterhin funktioniert.

>[!TIP]
>
>Eine schrittweise Anleitung zum Abschließen der exemplarischen Vorgehensweise finden Sie im Abschnitt [Anleitung zu Routern](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) Übung.


## Suchelemente im Zuordnungsbereich

Mit dem Feld Suchelemente oben in den Zuordnungsbedienfeldern können Sie Felder im Bedienfeld schnell finden, auch wenn sie in Arrays verschachtelt sind. Bei der Suche wird nicht zwischen Groß- und Kleinschreibung unterschieden.

![Ein Bild des ersten Suchfelds](assets/universal-connectors-and-routing-3.png)

![Ein Bild des zweiten Suchfelds](assets/universal-connectors-and-routing-4.png)

## Tipps und Tricks zum Arbeiten mit APIs

Bis zu diesem Zeitpunkt haben Sie mit einer sehr einfachen API (Application Programming Interface) gearbeitet, die keine zusätzliche Authentifizierung erfordert, um Informationen abzurufen, die in dem Szenario benötigt werden. Im Folgenden finden Sie einige Tipps für die Navigation mit APIs und universellen Connectoren.

## Schritt 1: Bestimmen des API-Typs

Workfront und viele Softwaresysteme werden mit einer REST-API (Repräsentational State Transfer) erstellt, der derzeit am einfachsten und am meisten standardmäßigen API-Typ ist. Es gibt jedoch einige weitere, wie z. B.:

* SOAP (Simple Object Access Protocol) (die Proof-API von Workfront ist SOAP-basiert)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Um mehr zu erfahren, führen Sie eine Websuche nach API-Typen und Keywords mit Interesse durch.

>[!NOTE]
>
>Beim Herstellen einer Verbindung zu größeren Plattformen wie Salesforce bieten unterschiedliche Bereiche dieser Plattformen verschiedene APIs. Stellen Sie sicher, dass Sie die richtige für den Dienst finden, mit dem Sie eine Verbindung herstellen möchten.

## Schritt 2: Bestimmen Sie den Authentifizierungstyp, der für die API erforderlich ist.

Die API-Authentifizierung ist eine Form der Identifizierung, mit der der Zugriff auf einen Dienst gesteuert wird, z. B. wenn Sie versuchen, eine Verbindung über Workfront Fusion herzustellen. Dies hilft Ihnen, einem anderen System nachzuweisen, dass Sie berechtigt sind, auf das System zuzugreifen. OAuth 2 ist der am häufigsten verwendete Authentifizierungstyp. Erfahren Sie mehr über eine Internetsuche zur API-Authentifizierung.

Authentifizierung kann der schwierigste Aspekt der Arbeit mit einer API sein. Eine der wertvollsten Funktionen der universellen Connectoren von Workfront Fusion ist, dass Workfront Fusion die Authentifizierung für Sie handhaben kann, wenn Sie gängige Authentifizierungsmethoden wie einfache Authentifizierung wie OAuth 2, API-Schlüssel und andere verwenden. Nachdem Sie eine Verbindung mit dem entsprechenden Workfront Fusion-Modul für Ihre Authentifizierungsmethode (z. B. OAuth 2) erstellt haben, generiert Workfront Fusion bei jeder Ausführung Ihres Szenarios kontinuierlich API-Schlüssel und/oder Token.

Informationen zu den verschiedenen Authentifizierungstypen, die Workfront bereitstellt, finden Sie im Artikel Erweiterte Authentifizierungsübersicht in Experience League.

## Schritt 3: Lesen Sie die API-Dokumentation und suchen Sie erforderliche Endpunkte

Wenn eine API mit einem anderen System interagiert, werden die Touchpoints dieser Kommunikation als Endpunkte betrachtet. Ein Endpunkt ist der Ort, an dem APIs Anfragen senden und an dem sich die Ressource befindet.

Bei der Interaktion mit einer API mithilfe eines universellen Connectors müssen Sie wissen, welche Endpunkte die API unterstützt und welche Daten für jede Anfrage benötigt werden. In der API-Dokumentation sollten die Endpunkte einer API beschrieben und beschrieben werden, wie allgemeine Vorgänge wie Erstellen, Lesen, Aktualisieren oder Löschen ausgeführt werden. Die Durchführung dieser Aufrufe erfordert einige Verfahren, insbesondere wenn Sie mit API-Aufrufen oder der Arbeit mit einer neuen API noch nicht vertraut sind.

Erfahren Sie mehr über Workfront Fusion Universal Connectors und deren Einrichtung für die Verbindung mit den APIs, die Sie in Experience League benötigen.

## Schlussbemerkung

Sie können die gesamte Liste unserer vordefinierten App-Connectoren in Experience League überprüfen. Wenn Sie dem Produktteam von Workfront Fusion einen neuen App-Connector vorschlagen möchten, senden Sie Ihre Idee an Innovation Lab. Wenn Sie noch nicht eingereicht haben, erfahren Sie mehr über das Innovationslabor und darüber, wie Sie Ideen wählen und an der zweimal jährlich stattfindenden Priorisierung des Leaderboards teilnehmen können. Wenn Sie bereits Zugriff auf das Innovationslabor haben, melden Sie sich an und übermitteln Sie Ihre Ideen.

## Ihre Wendung

>[!NOTE]
>
>Übungen sind optional und nicht erforderlich, um die Fusion-Schulung abzuschließen.

Diese Übung baut auf dem auf, was Sie in der exemplarischen Vorgehensweise gelernt haben, aber die Lösung wird nicht bereitgestellt.

Erstellen Sie im Modul Mehrere Variablen für Pokemon-Zeichen festlegen eine Variable namens &quot;Stat (Level)&quot;. Ordnen Sie den Namen der Pokemon Stats dieser Variablen zu. Mit der Funktion für Array-Werte können Sie die Anzeige des Arrays ändern, sodass jeder Status eine neue Zeile ist, wie unten dargestellt.

**Hinweis:** Es gibt nur sechs verschiedene Pokemon-Statistiken mit einer entsprechenden Ebene.

![Ein Bild von Statistiken](assets/universal-connectors-and-routing-5.png)

**Herausforderung:** Überprüfen Sie, ob Sie die Array-Formeln verwenden können, um die Funktionen zu erhalten, die wie oben beschrieben als unterschiedliche Zeilen und nicht als durch ein Komma getrennte Zeichenfolge angezeigt werden. Im folgenden Screenshot ist ein Hinweis enthalten.

![Ein Bild eines Array-Namens](assets/universal-connectors-and-routing-6.png)

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)

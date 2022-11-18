---
title: Unvollständige Ausführungen
description: Erfahren Sie, was unvollständige Ausführungen sind und wie Sie einen Fehler handhaben, der zu einer unvollständigen Ausführung führt in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Unvollständige Ausführungen

Unvollständige Ausführungen können in Workfront Fusion gespeichert werden, wo sie später überprüft und gelöst werden können. Erfahren Sie, wie Sie diese fantastische Funktion nutzen können.

In diesem Video erfahren Sie:

* Was sind unvollständige Ausführungen?
* Umgang mit Fehlern, die zu einer unvollständigen Ausführung führen

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## Fehler, die zu unvollständigen Ausführungen führen

Es gibt mehrere Fehlerkategorien, die dazu führen, dass unvollständige Ausführungen gespeichert werden.

Die verschiedenen empfangenen Fehlertypen hängen von den APIs ab, mit denen Sie eine Verbindung herstellen. Bei dem Fehler kann es sich um Validierungsfehler handeln, die aus unvollständigen oder fehlerhaften Daten resultieren, meist aufgrund eines fehlenden Elements, das zur erfolgreichen Verarbeitung aller Daten eines Moduls erwartet wird. Oder die Fehler treten auf, wenn das endgültige Ziel aufgrund eines temporären oder langfristigen Verbindungsfehlers nicht verfügbar ist (z. B. während der Verbindung zum E-Mail- oder Remote-FTP-Server).

Tritt beim ersten Modul des Szenarios ein Fehler auf, wird die Ausführung sofort gestoppt und es wird keine unvollständige Ausführung gespeichert.

Wenn bei einem anderen Modul ein Fehler auftritt und keine Fehler-Handler-Route angehängt ist, dann:

* Wenn der Fehlertyp &quot;ConnectionError&quot;, &quot;RateLimitError&quot;, &quot;OutOfSpaceError&quot;oder &quot;ModuleTimeoutError&quot;ist, wird ein unvollständiger Ausführungs-Datensatz MIT automatischer Wiederholung gespeichert.
* Wenn der Fehlertyp DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError oder MaxResultsExceededError lautet, wird ein unvollständiger Ausführungsprotokoll OHNE automatische Wiederholung gespeichert.
* Wenn der Fehlertyp etwas Anderes als den oben genannten ist, schlägt die Ausführung fehl.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)

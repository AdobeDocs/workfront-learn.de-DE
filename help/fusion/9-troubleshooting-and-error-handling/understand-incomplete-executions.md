---
title: Informationen zu unvollständigen Ausführungen
description: Erfahren Sie, was unvollständige Ausführungen sind und wie Sie in [!DNL Adobe Workfront Fusion]einen Fehler handhaben, der zu einer unvollständigen Ausführung führt.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 100%

---

# Informationen zu unvollständigen Ausführungen

Unvollständige Ausführungen können in Workfront Fusion gespeichert werden, wo sie später überprüft und gelöst werden können. Erfahren Sie, wie Sie diese fantastische Funktion nutzen können.

In diesem Video lernen Sie Folgendes:

* Unvollständige Ausführungen
* Umgang mit Fehlern, die zu einer unvollständigen Ausführung führen

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## Fehler, die zu unvollständigen Ausführungen führen

Es gibt mehrere Fehlerkategorien, die dazu führen, dass unvollständige Ausführungen gespeichert werden.

Die verschiedenen Fehlertypen, die Sie erhalten, hängen von den APIs ab, mit denen Sie sich verbinden. Bei dem Fehler kann es sich um einen Validierungsfehler handeln, der auf unvollständige oder fehlerhafte Daten zurückzuführen ist, meist aufgrund eines fehlenden Elements, das für die erfolgreiche Verarbeitung aller Daten, die ein Modul durchlaufen, erwartet wird. Oder die Fehler treten auf, wenn das endgültige Ziel aufgrund eines temporären oder langfristigen Verbindungsfehlers nicht verfügbar ist (z. B. während der Verbindung zum E-Mail- oder Remote-FTP-Server).

Tritt beim ersten Modul des Szenarios ein Fehler auf, wird die Ausführung sofort gestoppt und keine unvollständige Ausführung gespeichert.

Wenn bei einem anderen Modul ein Fehler auftritt und keine Fehler-Handler-Route angehängt ist, passiert Folgendes:

* Wenn der Fehlertyp „ConnectionError“, „RateLimitError“, „OutOfSpaceError“ oder „ModuleTimeoutError“ ist, wird ein Eintrag über eine unvollständige Ausführung MIT automatischer Wiederholung gespeichert.
* Wenn der Fehlertyp „DataError“, „InvalidConfigurationError“, „InvalidAccessTokenError“, „UnexpectedError“, „MaxFileSizeExceededError“ oder „MaxResultsExceededError“ lautet, wird ein Eintrag über eine unvollständige Ausführung OHNE automatische Wiederholung gespeichert.
* Bei allen anderen als den oben genannten Fehlertypen schlägt die Ausführung fehl.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=de)

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
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# Informationen zu unvollständigen Ausführungen

Unvollständige Ausführungen können in Workfront Fusion gespeichert werden, wo sie später überprüft und gelöst werden können. Erfahren Sie, wie Sie diese fantastische Funktion nutzen können.

In diesem Video lernen Sie Folgendes:

* Unvollständige Ausführungen
* Umgang mit Fehlern, die zu einer unvollständigen Ausführung führen

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## Fehler, die zu unvollständigen Ausführungen führen

Es gibt mehrere Fehlerkategorien, die dazu führen, dass unvollständige Ausführungen gespeichert werden.

Die verschiedenen Fehlertypen, die Sie erhalten, hängen von den APIs ab, mit denen Sie sich verbinden. Bei dem Fehler kann es sich um einen Validierungsfehler handeln, der auf unvollständige oder fehlerhafte Daten zurückzuführen ist, meist aufgrund eines fehlenden Elements, das für die erfolgreiche Verarbeitung aller Daten, die ein Modul durchlaufen, erwartet wird. Oder die Fehler treten auf, wenn das endgültige Ziel aufgrund eines temporären oder langfristigen Verbindungsfehlers nicht verfügbar ist (z. B. während der Verbindung zum E-Mail- oder Remote-FTP-Server).

Tritt beim ersten Modul des Szenarios ein Fehler auf, wird die Ausführung sofort gestoppt und keine unvollständige Ausführung gespeichert.

Wenn bei einem anderen Modul ein Fehler auftritt und keine Fehler-Handler-Route angehängt ist, passiert Folgendes:

* Wenn der Fehlertyp „ConnectionError“, „RateLimitError“, „OutOfSpaceError“ oder „ModuleTimeoutError“ ist, wird ein Eintrag über eine unvollständige Ausführung MIT automatischer Wiederholung gespeichert.
* Wenn der Fehlertyp „DataError“, „InvalidConfigurationError“, „InvalidAccessTokenError“, „UnexpectedError“, „MaxFileSizeExceededError“ oder „MaxResultsExceededError“ lautet, wird ein Eintrag über eine unvollständige Ausführung OHNE automatische Wiederholung gespeichert.
* Bei allen anderen als den oben genannten Fehlertypen schlägt die Ausführung fehl.

## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Workfront Fusion-Dokumentation](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

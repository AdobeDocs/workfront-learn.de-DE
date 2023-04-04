---
title: Webhooks-Anleitung
description: Erfahren Sie, wie Sie mit einem Webhook eine App erstellen können, um festzustellen, ob ein Kunde alt genug ist, um Alkohol zu kaufen, und alles in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhooks-Anleitung

## Übersicht

Mit diesem Szenario wird eine Convenience Store-App erstellt, mit der leicht festgestellt werden kann, ob ein Kunde alt genug ist, um Alkohol zu kaufen. Der Kassierer muss einfach den Namen und das Geburtsdatum des Kunden SOWIE ein verifiziertes Client-Token an eine bereitgestellte URL posten. Nach der Eingabe wird unser Szenario Trigger, die entsprechende Antwort zu berechnen und an den Anfragenden zurückzugeben.

![Ein Bild, das das Switch-Modul verwendet](assets/beyond-basic-modules-5.png)

## Webhooks-Anleitung

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on)

>[!TIP]
>
>Eine schrittweise Anleitung zum Abschließen der exemplarischen Vorgehensweise finden Sie im Abschnitt [Webhooks-Anleitung](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) Übung.

## Postman-Einrichtung

Um der exemplarischen Vorgehensweise zu folgen, müssen Sie die kostenlose Postman-Anwendung herunterladen. Gehen Sie wie folgt vor, um zum richtigen Bereich von Postman für die Übung zu navigieren.

1. Erstellen Sie einen Arbeitsbereich und öffnen Sie ihn.
1. Klicken Sie auf die Registerkarte Neu und erstellen Sie eine neue Sammlung mit dem Namen Trinkalter .
1. Klicken Sie erneut auf die Registerkarte Neu und erstellen Sie eine neue GET namens GET Geburtsdatum.
1. Ändern Sie die Anfrageaktion von GET in POST.
1. Navigieren Sie zum Untertab &quot;Hauptteil&quot;unter dem Feld POST-URL .
1. Wählen Sie unter der Unterregisterkarte Autorisierung Formulardaten aus.
1. Erstellen Sie drei Schlüssel für Name, Geburtsdatum und clientToken.

![Ein Bild, das das Switch-Modul verwendet](assets/beyond-basic-modules-6.png)

## Ihre Wendung

>[!NOTE]
>
>Übungen und Herausforderungen sind optional und nicht erforderlich, um eine Fusion-Schulung abzuschließen.

Diese Übung baut auf dem auf, was Sie in der exemplarischen Vorgehensweise gelernt haben, aber die Lösung wird nicht bereitgestellt.

Erstellen Sie einen Workfront-Webhook, der auf neu erstellte Updates wartet, und protokollieren Sie dann das Datum, den Namen der Person, die die Aktualisierung vorgenommen hat, und den Inhalt der Aktualisierung. Senden Sie sich diese Informationen per E-Mail.

**Hinweis**: Verwenden Sie das Workfront Watch Events Trigger-Modul, um Ihren Webhook zu erstellen. In Workfront werden Aktualisierungen auch als Notizen bezeichnet.

**Herausforderung**: Können Sie die URL finden und hinzufügen, für die die Aktualisierung vorgenommen wurde, um einfachen Zugriff zu erhalten?


## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)

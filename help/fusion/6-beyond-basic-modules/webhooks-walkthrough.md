---
title: Webhooks – Anleitung
description: Erfahren Sie, wie Sie in [!DNL Adobe Workfront Fusion]mit einem Webhook eine App erstellen, die prüft, ob eine Kundin oder ein Kunde alt genug ist, um Alkohol zu kaufen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: ht
source-wordcount: '339'
ht-degree: 100%

---

# Webhooks – Anleitung

In diesem Szenario wird eine App für ein Lebensmittelgeschäft entwickelt, mit der leicht geprüft werden kann, ob eine Person alt genug ist, um Alkohol zu kaufen. Die Kassiererin bzw. der Kassierer muss lediglich den Namen und das Geburtsdatum der Person UND ein verifiziertes Kunden-Token an eine bereitgestellte URL senden. Nach der Eingabe wird unser Szenario ausgelöst, um die entsprechende Antwort zu berechnen und an den Menschen zurückzuschicken, der die Anfrage gestellt hat.

![Ein Bild zur Verwendung des Switch-Moduls](assets/beyond-basic-modules-5.png)

## Webhooks – Anleitung

Workfront empfiehlt, sich das Anleitungsvideo anzusehen, bevor Sie versuchen, die Übung in Ihrer eigenen Umgebung neu zu erstellen.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops=1)


## Postman-Einrichtung

Um die Übung mit der exemplarischen Vorgehensweise durchführen zu können, müssen Sie die kostenlose Postman-App herunterladen. Gehen Sie wie folgt vor, um zum richtigen Postman-Bereich für die Übung zu gelangen.

1. Erstellen Sie einen Arbeitsbereich und öffnen Sie ihn.
1. Klicken Sie auf die Registerkarte „Neu“ und erstellen Sie eine neue Sammlung mit dem Namen „Trinkfähiges Alter“.
1. Klicken Sie erneut auf die Registerkarte „Neu“ und erstellen Sie eine neue GET-Anfrage mit dem Namen „GET Geburtsdatum“.
1. Ändern Sie die Anfrageaktion von GET in POST.
1. Gehen Sie zur Unterregisterkarte „Textkörper“ unterhalb des Feldes „POST URL“.
1. Wählen Sie in der Unterregisterkarte „Autorisierung“ die Option „Formulardaten“.
1. Erstellen Sie drei Schlüssel für Name, Geburtsdatum und clientToken.

![Bild zur Verwendung des Switch-Moduls](assets/beyond-basic-modules-6.png)

## Sie sind dran

>[!NOTE]
>
>Die Übungen und Herausforderungen sind optional und nicht notwendig, um die Fusion-Schulung abzuschließen.

Diese Übung baut auf dem auf, was Sie in der exemplarischen Vorgehensweise gelernt haben, aber die Lösung wird nicht bereitgestellt.

Erstellen Sie einen Workfront-Webhook, der auf neue Aktualisierungen wartet und dann das Datum, den Namen der Person, die die Aktualisierung vorgenommen hat, und den Inhalt der Aktualisierung protokolliert. Senden Sie sich diese Informationen per E-Mail zu.

**Hinweis**: Verwenden Sie das Trigger-Modul „Workfront – Ereignisse beobachten“, um Ihren Webhook zu erstellen. In Workfront werden Aktualisierungen auch als Notizen bezeichnet.

**Herausforderung**: Können Sie die URL, unter der die Aktualisierung vorgenommen wurde, finden und hinzufügen, um den Zugang zu erleichtern?


## Möchten Sie mehr erfahren? Wir empfehlen Folgendes:

[Dokumentation zu Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)

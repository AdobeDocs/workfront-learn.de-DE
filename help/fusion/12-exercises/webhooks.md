---
title: Webhooks-Übung
description: Erfahren Sie, wie Sie mit Webhooks initiierte Szenarien erstellen, auslösen und verwalten.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
recommendations: noDisplay,noCatalog
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '654'
ht-degree: 100%

---

# Webhooks-Übung

Erfahren Sie, wie Sie mit Webhooks initiierte Szenarien erstellen, auslösen und verwalten.

## Übungsübersicht

Der Zweck dieses Szenarios besteht darin, eine App zu erstellen, um sie an Supermärkte zu verkaufen, damit diese einfach feststellen können, ob eine Kundin oder ein Kunde alt genug ist, um Alkohol zu kaufen. Das Kassenpersonal muss einfach den Namen und das Geburtsdatum der Person an eine URL posten, die zur Verfügung gestellt wird. Dieser Post löst das Szenario aus, das die Antwort berechnet und sie an die Person, die die Anfrage gestellt hat, zurückgibt.

1. Das Szenario besteht aus drei Webhooks.
1. Das Trigger-Modul ist ein benutzerdefinierter Webhook, der auf einen Post lauscht.
1. Wenn es einen Post erhält, wird dieser an eines der nächsten Module ausgegeben.
1. Das nächste Modul gibt eine Antwort an die Person zurück, die die Anfrage gestellt hat.

   ![Webhooks – Bild 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Zu befolgende Schritte

**Richten Sie den Trigger-Webhook ein.**

1. Erstellen Sie ein neues Szenario und nennen Sie es „Webhooks verwenden“.
1. Fügen Sie für den Trigger das benutzerdefinierte Webhook-Modul aus der Webhooks-App hinzu.
1. Klicken Sie auf „Hinzufügen“, um einen neuen Webhook zu erstellen.
1. Geben Sie den Webhook-Namen „App für Alkoholmindestalter“ ein.
1. Lassen Sie IP-Einschränkungen leer, d. h. jeder kann Daten an den Webhook senden.
1. Klicken Sie auf Speichern.


   ![Webhooks – Bild 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. Zurück im Bedienfeld „Webhooks-Zuordnung“ wurde eine URL für diesen spezifischen Webhook erstellt. Klicken Sie auf „Adresse in Zwischenablage kopieren“, um diese URL zu kopieren.
1. Klicken Sie auf „OK“.
1. Klicken Sie auf „Einmal ausführen“.
1. Verwenden Sie die URL in Postman, um einen Namen und ein Geburtsdatum an Ihren benutzerdefinierten Webhook zu senden. Anweisungen zum Einrichten von Postman finden Sie im Tutorial [Exemplarische Vorgehensweise zu Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=de).

   **Das Bedienfeld des Webhooks-Moduls sollte wie folgt aussehen:**

   ![Webhooks – Bild 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Der Webhook befindet sich jetzt in einem Status, in dem er Daten zur Bestimmung der Datenstruktur überwacht.**

1. Sie können die Datenstruktur der Payload definieren, die Sie erwarten (Datenstrukturen werden später besprochen). Wenn Sie keine Datenstruktur definieren, bestimmt Fusion die Datenstruktur automatisch, wenn der Post gesendet wird.
1. Auf der Postman-Seite möchten Sie an die kopierte URL senden. Der Post sollte grundlegende Formulardaten enthalten. Für dieses Beispiel benötigen Sie drei Felder: Name, Geburtsdatum und clientToken.

   ![Webhooks – Bild 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Nachdem Sie auf „Von Postman senden“ geklickt haben, sollten Sie einen Hinweis erhalten, dass der Post akzeptiert wurde.
1. Dies ist der Punkt, an dem Ihr Szenario zeigt, dass die Datenstruktur erfolgreich ermittelt wurde.
1. Sie können sehen, dass die Daten empfangen wurden, indem Sie den Ausführungsinspektor öffnen.

   ![Webhooks – Bild 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Richten Sie das Routing für Client-Token ein.**

1. Fügen Sie dem Trigger-Modul einen Router hinzu.
1. Fügen Sie im oberen Pfad ein Webhook-Antwortmodul hinzu. Dies ist unser Pfad für den Fall, dass das Client-Token nicht übereinstimmt.
1. Legen Sie den Status auf 401 fest.
1. Legen Sie den Hauptteil auf {„Fehler“: „Anfrage konnte nicht authentifiziert werden. Bitte überprüfen Sie Ihr clientToken“} fest.

   ![Webhooks – Bild 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Erstellen Sie einen Filter zwischen dem Router und dem Webhook-Antwortmodul. Geben Sie ihm den Namen „Client-Token stimmt nicht überein“.
1. Verwenden Sie für die Bedingung das Feld „clientToken“ aus dem Trigger-Modul und führen Sie einen numerischen Vergleich des Typs „Ist nicht gleich“ mit der Zahl 5121933 durch.

   ![Webhooks – Bild 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. Fügen Sie im unteren Pfad ein weiteres Webhook-Antwortmodul hinzu. Dies ist unser Pfad für den Fall, dass das Client-Token übereinstimmt.
1. Legen Sie den Status auf 200 fest.
1. Verwenden Sie beim Einrichten des Hauptteils die Funktionen des Bedienfelds „Zuordnung“, um zu testen, ob die Person 21 oder älter ist. Falls sie es ist, geben Sie „Sie sind alt genug, um Alkohol zu kaufen!“ zurück, und ansonsten: „Pech gehabt …“

   ![Webhooks – Bild 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Erstellen Sie auf dem unteren Pfad einen Filter zwischen dem Router und dem Webhook-Antwortmodul. Nennen Sie ihn „Client-Token stimmt überein“.
1. Verwenden Sie für die Bedingung das Feld „clientToken“ aus dem Trigger-Modul und führen Sie einen numerischen Vergleich des Typs „Ist gleich“ mit der Zahl 5121933 durch.


   ![Webhooks – Bild 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Klicken Sie auf die Schaltfläche „Planung“ unter „Einmal ausführen“, um Ihr Szenario zu aktivieren, sodass jedes Mal, wenn ein neuer Post eingeht, er die beiden Pfade durchläuft und eine Antwort generiert wird.

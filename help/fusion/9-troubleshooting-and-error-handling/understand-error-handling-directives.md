---
title: Grundlegendes zu Fehlerbehandlungsanweisungen
description: Erfahren Sie mehr über die Fehlerbehandlungsanweisungen, die eine Fortsetzung der Ausführung in [!DNL Adobe Workfront Fusion]ermöglichen, und diejenigen, die die Ausführung anhalten.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:23.288Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 100%

---

# Grundlegendes zu Fehlerbehandlungsanweisungen

In diesem Video lernen Sie Folgendes:

* Die drei Fehlerbehandlungsanweisungen, die eine Fortsetzung der Ausführung ermöglichen
* Die beiden Fehlerbehandlungsanweisungen, die die Ausführung anhalten

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops=1)

## Anweisungen − Szenario (Fortsetzung)

### Wieder aufnehmen

* Es wird eine Ersatzausgabe angegeben und an das Modul geliefert, bei dem ein Fehler auftritt.
* Die nachfolgenden Module werden verarbeitet.
* Der Szenario-Ausführungsstatus wird als „erfolgreich“ gekennzeichnet.

![Ein Bild einer Anweisung „Wieder aufnehmen“](assets/troubleshooting-and-error-handling-2.png)

### Unterbrechen

* Der Zustand der Szenarioausführung wird in der Warteschlange für unvollständige Ausführungen gespeichert, wo der Fehler manuell behoben werden kann. Es gibt jedoch einige Ausnahmen, die hier genannt werden.
* Die nachfolgenden Module werden nicht verarbeitet.
* Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.
* Der Ausführungsstatus des Szenarios ist als „Warnung“ gekennzeichnet.

![Ein Bild einer Anweisung „Unterbrechen“](assets/troubleshooting-and-error-handling-3.png)

### Ignorieren

* Der Fehler wird ignoriert und die nachfolgenden Module werden nicht verarbeitet.
* Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.
* Der Szenario-Ausführungsstatus wird als „erfolgreich“ gekennzeichnet.

![Ein Bild einer Anweisung „Ignorieren“](assets/troubleshooting-and-error-handling-4.png)

## Anweisungen − Szenario stoppt

### Rollback

* Die Ausführung des Szenarios wird sofort gestoppt, und es wird eine Rollback-Phase für alle Module eingeleitet, um sie in ihren Ausgangszustand zurückzusetzen.
* Die nachfolgenden Module werden nicht verarbeitet.
* Mit Ausnahme einiger weniger Fehlertypen wird das Szenario nach der in den Szenarioeinstellungen angegebenen „Anzahl aufeinanderfolgender Fehler“ deaktiviert.
* Der Szenario-Ausführungsstatus ist als „Fehler“ gekennzeichnet.

>[!NOTE]
>
>Dies ist das Standardverhalten, wenn dem Modul keine Fehlerbehandlungsroute zugeordnet ist und die Einstellung „Speichern unvollständiger Ausführungen zulassen“ in den Szenarioeinstellungen nicht aktiviert ist.

![Ein Bild einer Rollback-Anweisung](assets/troubleshooting-and-error-handling-5.png)

### Zusichern

* Der Fehler wird ignoriert und die nachfolgenden Module werden nicht verarbeitet.
* Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.
* Der Szenario-Ausführungsstatus wird als „erfolgreich“ gekennzeichnet.

![Ein Bild einer Commit-Anweisung](assets/troubleshooting-and-error-handling-6.png)

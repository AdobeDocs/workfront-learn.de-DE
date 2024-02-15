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
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '318'
ht-degree: 100%

---

# Grundlegendes zu Fehlerbehandlungsanweisungen

In diesem Video lernen Sie Folgendes:

* Die drei Fehlerbehandlungsanweisungen, die eine Fortsetzung der Ausführung ermöglichen
* Die beiden Fehlerbehandlungsanweisungen, die die Ausführung anhalten

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## Anweisungen − Szenario (Fortsetzung)

### Wieder aufnehmen

* Es wird eine Ersatzausgabe angegeben und an das Modul geliefert, bei dem ein Fehler auftritt.
* Die nachfolgenden Module werden verarbeitet.
* Der Status der Szenarioausführung wird als „erfolgreich“ gekennzeichnet.

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
* Der Status der Szenarioausführung wird als „erfolgreich“ gekennzeichnet.

![Ein Bild einer Anweisung „Ignorieren“](assets/troubleshooting-and-error-handling-4.png)

## Anweisungen − Szenario stoppt

### Rollback

* Die Ausführung des Szenarios wird sofort gestoppt, und es wird eine Rollback-Phase für alle Module eingeleitet, um sie in ihren Ausgangszustand zurückzusetzen.
* Die nachfolgenden Module werden nicht verarbeitet.
* Mit Ausnahme einiger weniger Fehlertypen wird das Szenario nach der in den Szenarioeinstellungen angegebenen „Anzahl aufeinanderfolgender Fehler“ deaktiviert.
* Der Status der Szenarioausführung ist als „Fehler“ gekennzeichnet.

>[!NOTE]
>
>Dies ist das Standardverhalten, wenn dem Modul keine Fehlerbehandlungsroute zugeordnet ist und die Einstellung „Speichern unvollständiger Ausführungen zulassen“ in den Szenarioeinstellungen nicht aktiviert ist.

![Ein Bild einer Rollback-Anweisung](assets/troubleshooting-and-error-handling-5.png)

### Zusichern

* Der Fehler wird ignoriert und die nachfolgenden Module werden nicht verarbeitet.
* Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.
* Der Status der Szenarioausführung wird als „erfolgreich“ gekennzeichnet.

![Ein Bild einer Commit-Anweisung](assets/troubleshooting-and-error-handling-6.png)

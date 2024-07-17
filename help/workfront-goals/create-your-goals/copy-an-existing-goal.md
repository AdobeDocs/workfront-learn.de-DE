---
title: Kopieren eines bestehenden Ziels
description: Erfahren Sie, wie Sie ein bestehendes Ziel in [!DNL Workfront Goals]kopieren.
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 100%

---

# Kopieren eines bestehenden Ziels

Nehmen wir an, sie möchten am Quartalsende ein bestehendes Ziel für den nächsten Zeitraum neu erstellen. Oder vielleicht haben Sie das Ziel nicht erreicht und müssen es auf den nächsten Zeitraum ausdehnen. Wie lässt sich dieses Ziel am besten erreichen? Sie möchten ein bestehendes Ziel kopieren und ändern.

Das Kopieren eines bestehenden Ziels ist auch dann sinnvoll, wenn mehrere Team-Mitglieder ähnliche Ziele haben und Sie für jedes von ihnen ein Ziel erstellen müssen.

<!--
Pro-tips graphic
-->

Beachten Sie vor dem Kopieren von Zielen Folgendes:

* Alle Informationen aus dem ursprünglichen Ziel werden kopiert, mit Ausnahme des Zielzeitraums (da dieser in der Vergangenheit liegt).
* Sie können die Ergebnisse eines vorhandenen Ziels kopieren, wodurch sie in das neue Ziel übertragen werden.
* Kopierte Ergebnisse werden standardmäßig demselben Eigentümer zugewiesen.
* Sie können den Fortschritt des vorhandenen Ziels nicht in ein neues Ziel kopieren.
* Beim Kopieren eines Ziels können Sie die damit verbundenen Aktivitäten nicht mit kopieren.

## Wie man ein Ziel kopiert

1. Klicken Sie auf einen Zielnamen, um das Bedienfeld **[!UICONTROL Zieldetails]** zu öffnen.
1. Klicken Sie auf die drei Punkte und wählen Sie dann **[!UICONTROL Kopieren]**.
1. Aktualisieren Sie eine der folgenden Informationen für das kopierte Ziel:
   * **Neues Ziel** – Dies ist der Name des neuen Ziels. Standardmäßig ist dies der Name des ursprünglichen Ziels.
   * **Zeitraum** – Der Zeitraum, in dem Sie das Ziel erreichen wollen. Wählen Sie einen Zeitraum aus dem Dropdown-Menü aus oder klicken Sie auf „Benutzerdefinierte Daten definieren“, um einen benutzerdefinierten Zeitraum anzugeben. Der Standardzeitraum ist immer das aktuelle Quartal.
   * **Eigentümer** – Der Eigentümer des Ziels. Dies kann eine Person, ein Team, eine Gruppe oder ein Unternehmen sein. Standardmäßig ist es der Eigentümer des ursprünglichen Ziels.
   * **Beschreibung** – Zusätzliche Informationen zum Ziel.

1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Ergebnisse kopieren]**, wenn zum ursprünglichen Ziel Ergebnisse hinzugefügt wurden und Sie diese in das neue Ziel kopieren möchten. Die Ergebnisse des kopierten Ziels haben dieselben Eigentümer, Namen und Messwerte wie die Ergebnisse des ursprünglichen Ziels.

1. Klicken Sie auf **[!UICONTROL Speichern]**. Das kopierte Ziel wird mit dem Status „Entwurf“ gespeichert.

   ![Ein Bild des Fensters [!UICONTROL Zieldetails] in [!DNL Workfront Goals] mit der Option [!UICONTROL Kopieren]](assets/03-workfront-goals-copy-a-goal.png)

1. Klicken Sie auf **[!UICONTROL Aktivieren]**, um den Status des Ziels in „Aktiv“ zu aktualisieren. Das Ziel muss mit einer Aktivität oder einem Ergebnis verbunden sein, damit es „aktiviert“ wird.

1. Klicken Sie auf das **X** oben rechts im Fenster [!UICONTROL Zieldetails], um es zu schließen.

Wenn Sie ein Ziel kopiert haben, das in einem früheren Zeitraum nicht abgeschlossen wurde, und im folgenden Zeitraum weiter daran arbeiten möchten, gehen Sie wie folgt vor:

1. Rufen Sie das ursprüngliche Ziel im Abschnitt **[!UICONTROL Zielliste]**, **[!UICONTROL Einchecken]** oder **[!UICONTROL Impuls]** auf.
1. Kommentieren Sie das Ziel, um anzugeben, dass es kopiert und ein aktuelleres Ziel erstellt wurde.
1. Schließen Sie das ursprüngliche Ziel, um die während des ursprünglichen Zeitraums erzielten Fortschritte beizubehalten. Klicken Sie auf die drei Punkte im Bedienfeld **[!UICONTROL Zieldetails]** und dann im Menü auf **[!UICONTROL Schließen]**.
1. Aktualisieren Sie den [!UICONTROL Ausgangswert] des neuen Ergebnisses entsprechend des **[!UICONTROL Zielwerts]** des vorherigen Ergebnisses, sodass Ihr neuer Zielfortschritt mit der Berechnung ab dem im vorherigen Zeitraum erreichten Punkt beginnt.

---
title: Vorhandenes Ziel kopieren
description: Erfahren Sie, wie Sie ein vorhandenes Ziel kopieren in [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Vorhandenes Ziel kopieren

Nehmen wir an, es ist das Ende eines Quartals und Sie möchten ein vorhandenes Ziel für den nächsten Zeitraum neu erstellen. Oder vielleicht haben Sie das Ziel nicht erreicht und müssen in den nächsten Zeitraum hineinreichen. Was ist die beste Option, um dieses Ziel zu erreichen? Sie möchten ein vorhandenes Ziel kopieren und ändern.

Das Kopieren eines vorhandenen Ziels ist auch dann nützlich, wenn mehrere Teammitglieder ähnliche Ziele haben und Sie für jedes dieser Ziele ein Ziel erstellen müssen.

<!--
Pro-tips graphic
-->

Beachten Sie vor dem Kopieren von Zielen Folgendes:

* Alle Informationen aus dem ursprünglichen Ziel werden kopiert, mit Ausnahme des Zielzeitraums (da dieser in der Vergangenheit liegt).
* Sie können die Ergebnisse eines vorhandenen Ziels kopieren und sie werden in das neue Ziel übertragen.
* Kopierte Ergebnisse werden standardmäßig demselben Eigentümer zugewiesen.
* Sie können den Fortschritt des vorhandenen Ziels nicht in ein neues Ziel kopieren.
* Sie können die Aktivitäten eines Ziels nicht kopieren, wenn Sie ein Ziel kopieren.

## Kopieren eines Ziels

1. Klicken Sie auf einen Zielnamen, um die **[!UICONTROL Zieldetails]** Bereich.
1. Klicken Sie auf das 3-Punkt-Symbol und wählen Sie **[!UICONTROL Kopieren]**.
1. Aktualisieren Sie eine der folgenden Informationen für das kopierte Ziel:
   * **Neues Ziel**—Dies ist der Name des neuen Ziels. Die Standardeinstellung ist der Name des ursprünglichen Ziels.
   * **Zeitraum**—Der Zeitraum, in dem Sie das Ziel erreichen möchten. Wählen Sie einen Zeitraum aus dem Dropdown-Menü aus oder klicken Sie auf Benutzerdefinierte Datumswerte definieren , um einen benutzerdefinierten Zeitraum anzugeben. Der Standardzeitraum ist immer das aktuelle Quartal.
   * **Inhaber**—Der Eigentümer des Ziels. Dabei kann es sich um einen Benutzer, ein Team, eine Gruppe oder ein Unternehmen handeln. Die Standardeinstellung ist der Eigentümer des ursprünglichen Ziels.
   * **Beschreibung**—Zusätzliche Informationen zum Ziel.

1. Überprüfen Sie die **[!UICONTROL Ergebnisse kopieren]** , wenn dem ursprünglichen Ziel Ergebnisse hinzugefügt wurden und Sie sie in das neue Ziel kopieren möchten. Die Ergebnisse des kopierten Ziels haben denselben Eigentümer, dieselben Namen und die gemessenen Werte wie die Ergebnisse des ursprünglichen Ziels.

1. Klicken Sie auf **[!UICONTROL Speichern]**. Das kopierte Ziel wird mit dem Status Entwurf gespeichert.

   ![Ein Bild der [!UICONTROL Zieldetails] Bedienfeld in [!DNL Workfront Goals] mit dem [!UICONTROL Kopieren] option](assets/03-workfront-goals-copy-a-goal.png)

1. Klicken **[!UICONTROL Aktivieren]**, wodurch der Zielstatus auf &quot;Aktiv&quot;aktualisiert wird. Das Ziel muss über eine zugehörige Aktivität oder ein zugehörigen Ergebnis verfügen, um &quot;aktiviert&quot;zu können.

1. Klicken Sie auf **X** oben rechts im [!UICONTROL Zieldetails] -Bedienfeld, um es zu schließen.

Wenn Sie ein Ziel kopiert haben, das in einem früheren Zeitraum nicht erreicht wurde, und im folgenden Zeitraum daran weiter arbeiten möchten, gehen Sie wie folgt vor:

1. Navigieren Sie zum ursprünglichen Ziel im **[!UICONTROL Zielliste]**, **[!UICONTROL Einchecken]** oder **[!UICONTROL Puls]** Abschnitt.
1. Kommentar zum Ziel, um anzugeben, dass es kopiert und ein aktuelleres Ziel erstellt wurde.
1. Schließen Sie das ursprüngliche Ziel, um die während des ursprünglichen Zeitraums erzielten Fortschritte beizubehalten. Klicken Sie auf das 3-Punkt-Symbol im **[!UICONTROL Zieldetails]** Bedienfeld und wählen Sie **[!UICONTROL Schließen]** aus dem Menü.
1. Aktualisieren Sie die [!UICONTROL Initial] -Wert des neuen Ergebnisses, das mit der **[!UICONTROL Target]** -Wert des vorherigen Ergebnisses, sodass Ihr neuer Zielfortschritt mit der Berechnung ab dem im vorherigen Zeitraum erreichten Punkt beginnt.

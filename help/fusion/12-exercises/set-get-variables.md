---
title: Variablen festlegen/abrufen
description: Erfahren Sie, wie Sie mit den Modulen Set and Get Variable die Felder verwenden können, die in einem Pfad in einem anderen Pfad verfügbar sind.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Variablen festlegen/abrufen

Erfahren Sie, wie Sie mit den Modulen Set and Get Variable die Felder verwenden können, die in einem Pfad in einem anderen Pfad verfügbar sind.

## Übungsübersicht

Suchen Sie nach Informationen zu einem Projekt in Workfront und senden Sie eine E-Mail mit zugehörigen Informationen.

![Set Get variables Image 1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Schritte, die ausgeführt werden müssen

1. Erstellen Sie ein neues Szenario und nennen Sie es &quot;Freigabe von Variablen zwischen Routing-Pfaden&quot;.
1. Wählen Sie für den Trigger das Suchmodul in der Workfront-App aus.

   + Setzen Sie den Record Type auf Project.
   + Wählen Sie für die Ergebnismenge &quot;Alle übereinstimmenden Datensätze&quot;.
   + Legen Sie für Suchkriterien den Status Gleich CUR fest.
   + Wählen Sie für Ausgaben ID, Name, Beschreibung und Sponsor-ID aus.

   ![Set Get variables Image 2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Set Get variables Image 3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Klicken Sie auf OK und benennen Sie dieses Modul &quot;Aktuelle Projekte suchen&quot;um.
1. Fügen Sie ein weiteres Modul hinzu und wählen Sie das Workfront-Datensatzmodul lesen aus.

   + Wählen Sie für den Datensatztyp Benutzer aus.
   + Wählen Sie für Ausgaben &quot;Name&quot;.
   + Ordnen Sie die Sponsor-ID aus dem Suchmodul dem Feld ID zu.

1. Klicken Sie auf OK.
1. Benennen Sie das Modul &quot;Finden Sie Sponsor Name&quot; um.

   ![Set Get variables Image 4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Speichern Sie das Szenario und klicken Sie einmal auf Ausführen .

   Wenn Sie einen Fehler beim Modul &quot;Datensatz lesen&quot;erhalten, liegt dies wahrscheinlich daran, dass das Suchmodul ein Projekt ohne aufgelisteten Sponsor findet.

   **Um diesen Fehler zu vermeiden, erstellen Sie zwei Pfade: eine für Projekte, die eine Sponsor-ID besitzen, und eine für Projekte, die dies nicht tun.**

1. Fügen Sie einen Router zwischen den beiden Modulen hinzu, indem Sie auf das Schraubenschlüsselsymbol zwischen dem Router und dem Modul Datensatz lesen klicken. Richten Sie einen Filter mit der Bezeichnung &quot;Sponsor ist vorhanden&quot;ein und legen Sie die Bedingung auf &quot;Sponsor ID Exists&quot;fest.

   ![Set Get variables Image 5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Klicken Sie auf den Router, um einen weiteren Pfad zu erstellen. Fügen Sie ein Modul E-Mail senden aus der E-Mail-App hinzu.

   + Geben Sie Ihre eigene E-Mail-Adresse in das Feld &quot;An&quot;ein.
   + Geben Sie im Feld &quot;Betreff&quot;die Bezeichnung &quot;Aktuelle Projektinformationen&quot;ein.
   + Geben Sie im Feld Inhalt den Projektnamen, die Beschreibung und den Sponsor ein.
   + Sie können die Sponsornamenausgabe nicht aus dem Datensatzmodul lesen abrufen. Sie können nur über das Suchmodul vor dem Router auf die Sponsor-ID zugreifen. Sie müssen eine Möglichkeit finden, über den anderen Router-Pfad auf den Namen des Sponsors zuzugreifen.

   ![Set Get variables Image 6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Klicken Sie zunächst auf OK und benennen Sie dieses Modul &quot;Projektinformationen senden&quot;um.

   **Verwenden Sie Variablen festlegen/abrufen , um Daten zwischen verschiedenen Pfaden freizugeben.**

1. Fügen Sie nach dem Modul Find sponsor name ein Tool-Modul Set variable hinzu.

   + Legen Sie &quot;Sponsor Name&quot;als Variablennamen fest.
   + Belassen Sie die Lebensdauer der Variablen auf einen Zyklus.
   + Weisen Sie das Feld der Namensausgabe aus dem Modul &quot;Find sponsor name&quot;zu.

1. Klicken Sie auf OK und benennen Sie dann das Modul &quot;Set Sponsor Name&quot; um.

   ![Set Get variables Image 7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Klicken Sie anschließend mit der rechten Maustaste zwischen dem Router und dem Modul E-Mail senden , um ein Tool-Modul Get variable hinzuzufügen. Geben Sie im Feld Variablenname den Namen &quot;Sponsor&quot;ein.
1. Klicken Sie auf OK. Benennen Sie das Modul &quot;Name des Sponsors abrufen&quot;um.

   ![Festlegen von Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Gehen Sie zurück zum Modul E-Mail senden und ordnen Sie den Wert aus dem Modul Sponsor-Name abrufen dem Inhaltsfeld zu. Klicken Sie auf OK.

   ![Festlegen von Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Bevor Sie das Szenario testen, empfehlen wir, die Anzahl der von Ihnen verarbeiteten Projekte zu begrenzen, um eine Flut von E-Mails zu vermeiden.

1. Gehen Sie zu Ihrem Workfront-Testlaufwerk und suchen Sie nach dem Northstar Fashion Exhibitors-Messeprojekt. Dies ist ein aktuelles Projekt, das einen Sponsor hat. Kopieren Sie die Projekt-ID aus der URL.

   ![Set Get variables Image 10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. Klicken Sie in Ihrem Szenario auf das Modul Aktuelle Projekte suchen . Fügen Sie den Suchkriterien eine weitere Bedingung hinzu, indem Sie auf die grüne Schaltfläche &quot;Add AND rule&quot;(UND-Regel hinzufügen) klicken. Geben Sie an, dass die ID mit der kopierten Projekt-ID übereinstimmen muss. Klicken Sie auf OK.
1. Speichern Sie das Szenario und klicken Sie einmal auf Ausführen .
1. Überprüfen Sie die Ausführungsinspektoren und die E-Mail, die Sie erhalten.

   ![Set Get variables Image 11](../12-exercises/assets/set-get-variables-walkthrough-11.png)

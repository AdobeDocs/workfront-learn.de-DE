---
title: Suchen und Organisieren von Assets in [!UICONTROL Workfront DAM]
description: Erfahren Sie, wie Sie nach Assets suchen, in Ordnern suchen, Suchergebnisse optimieren, Metadaten und Keywords als Suchfilter verwenden und vieles mehr in [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Mitarbeiter: Suchen von Assets

In diesem Video erfahren Sie, wie Sie:

* Suchen nach Assets
* Suchen in Ordnern
* Optimieren von Suchergebnissen
* Metadaten und Keywords als Suchfilter verwenden
* Ordnerdetails anzeigen
* Anzeigen und Aktualisieren von Asset-Metadaten und Keywords

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## Grundlegende Suchkriterien

Bei einer einfachen Suche werden Dateinamen, Metadatenfelder, Schlüsselwörter und Asset-Inhalt untersucht (je nach Asset-Typ). Der Ordnername ist nicht enthalten.

Die meisten Suchergebnisse sind exakte Treffer. Eine Ausnahme von dieser &quot;exakten Übereinstimmung&quot;-Regel ist, wenn die Variable [!UICONTROL Workfront DAM] durchsucht das Dateinamenfeld. [!UICONTROL Workfront DAM] gibt eine teilweise Übereinstimmung des Dateinamens zurück, anstatt nur exakte Übereinstimmung mit dem Dateinamen zu erhalten.

## Benutzer beim Suchen

Obwohl die grundlegenden Suchfunktionen häufig die benötigten Assets finden, müssen Sie möglicherweise von Zeit zu Zeit zusätzliche Suchparameter verwenden.

### Teilübereinstimmung

Um eine teilweise Übereinstimmung zu finden, fügen Sie dem Suchbegriff ein Sternchen hinzu. Das Sternchen darf nur am Ende eines Wortes verwendet werden.

### AND-Operator

Um Ergebnisse zu finden, die mehrere Suchbegriffe enthalten, geben Sie UND zwischen den Wörtern ein. Die Wörter sind in beliebiger Reihenfolge zu finden. Bei der Suche über alle Felder hinweg sind beide Wörter möglicherweise nicht im selben Feld vorhanden. Beispielsweise findet der Turm &quot;Paris AND&quot;Assets, die beide Wörter in einem der Felder enthalten.

### ODER-Operator

Verwenden Sie den ODER -Operator, um Assets zu finden, die einen der Suchbegriffe enthalten. Beispielsweise findet Paris ODER Arc Assets, die eines der Wörter enthalten, aber nicht unbedingt beides.

### Satz

Verwenden Sie doppelte Anführungszeichen um die Wörter, um einen genauen Wortlaut zu finden. Alle Worte werden zusammen und in der richtigen Reihenfolge gefunden. Beispielsweise findet &quot;Eiffelturm&quot;diese Wörter in genau dieser Reihenfolge.

### Negativer Operator

Wenn Sie ein Wort aus den Suchergebnissen ausschließen möchten, setzen Sie ein Minuszeichen (-) vor das Wort. Achten Sie darauf, dass zwischen dem Minuszeichen und dem Wort kein Leerzeichen steht. Um beispielsweise Assets auszuschließen, die in den Metadaten das Wort &quot;Turm&quot;enthalten, kann Ihre Suche als &quot;Paris -Turm&quot;eingerichtet werden.

### Operator für leeres Feld

Um nach Assets zu suchen, die keine Informationen in einem bestimmten Metadatenfeld enthalten, geben Sie das Feld ein, das Sie in diesem Format suchen möchten: ?[xxxxxxx]. Wenn Sie beispielsweise Assets suchen möchten, denen keine Keywords zugewiesen sind, geben Sie ? ein.[Keyword] im Suchfeld.

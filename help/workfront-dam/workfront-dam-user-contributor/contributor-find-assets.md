---
title: Grundlegendes zur Asset-Suche als Mitwirkende
description: Erfahren Sie, wie Sie in [!UICONTROL Workfront DAM] nach Assets suchen, in Ordnern suchen, Suchergebnisse optimieren sowie Metadaten und Schlüsselwörter als Suchfilter verwenden.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 100%

---

# Grundlegendes zur Asset-Suche als Mitwirkende

In diesem Video lernen Sie Folgendes:

* Suchen nach Assets
* Suchen in Ordnern
* Optimieren von Suchergebnissen
* Verwenden von Metadaten und Schlüsselwörtern als Suchfilter
* Anzeigen von Ordnerdetails
* Anzeigen und Aktualisieren von Asset-Metadaten und Schlüsselwörtern

>[!VIDEO](https://video.tv.adobe.com/v/3453932/?quality=12&learn=on&enablevpops=1&captions=ger)

## Grundlegende Suchkriterien

Bei einer einfachen Suche wird nach Dateinamen, Metadatenfeldern, Schlüsselwörter und Asset-Inhalt (je nach Asset-Typ) gesucht. Der Ordnername wird nicht einbezogen.

Die meisten Suchergebnisse sind exakte Treffer. Eine Ausnahme von dieser Regel für „exakte Treffer“ besteht, wenn [!UICONTROL Workfront DAM] das Dateinamenfeld durchsucht. [!UICONTROL Workfront DAM] gibt eine teilweise Übereinstimmung mit dem Dateinamen zurück, anstatt nur exakte Treffer für den Dateinamen.

## Verwenden von Operatoren beim Suchen

Auch wenn die grundlegenden Suchfunktionen häufig die benötigten Assets finden, müssen Sie möglicherweise von Zeit zu Zeit zusätzliche Suchparameter verwenden.

### Teilweise Übereinstimmungen

Um eine teilweise Übereinstimmung zu finden, fügen Sie dem Suchbegriff ein Sternchen hinzu. Das Sternchen darf nur am Ende eines Wortes verwendet werden.

### UND-Operator

Um Ergebnisse zu finden, die mehrere Suchbegriffe enthalten, geben Sie UND zwischen den Wörtern ein. Die Wörter können in beliebiger Reihenfolge gefunden werden. Bei der Suche über alle Felder hinweg sind beide Wörter möglicherweise nicht im selben Feld vorhanden. Beispielsweise findet „Paris UND Turm“ Assets, die in einem der Felder beide Wörter enthalten.

### ODER-Operator

Verwenden Sie den ODER-Operator, um Assets zu finden, die einen der Suchbegriffe enthalten. Beispielsweise findet „Paris ODER Arc“ Assets, die eines der Wörter enthalten, aber nicht unbedingt beide.

### Ausdruck

Schließen Sie die Wörter in doppelte Anführungszeichen ein, um einen genauen Ausdruck zu finden. Alle Wörter werden zusammen und in der vorgegebenen Reihenfolge gefunden. Zum Beispiel werden bei der Suche nach „Deutsche Bank Park“ nur Assets zurückgegeben, die diese Wörter in genau dieser Reihenfolge enthalten.

### Negativer Operator

Wenn Sie ein Wort aus den Suchergebnissen ausschließen möchten, setzen Sie ein Minuszeichen (-) vor das Wort. Achten Sie darauf, dass sich zwischen dem Minuszeichen und dem Wort kein Leerzeichen befindet. Um z. B. Assets auszuschließen, die das Wort „Turm“ in den Metadaten enthalten, könnte Ihre Suche „Paris -Turm“ lauten.

### Operator für leere Felder

Um nach Assets zu suchen, die in einem bestimmten Metadatenfeld keine Informationen enthalten, geben Sie das Feld, das Sie suchen möchten, in diesem Format ein: ?[xxxxx]. Wenn Sie beispielsweise nach Assets suchen möchten, denen keine Schlüsselwörter zugewiesen sind, geben Sie „?“ ein[Schlüsselwort]“ im Suchfeld ein.

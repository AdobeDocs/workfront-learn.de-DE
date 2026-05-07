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
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:25:54.114Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 407
ht-degree: 89%

---

# Grundlegendes zur Asset-Suche als Mitwirkende

In diesem Video lernen Sie Folgendes:

* Suchen nach Assets
* Suchen in Ordnern
* Optimieren von Suchergebnissen
* Verwenden von Metadaten und Schlüsselwörtern als Suchfilter
* Anzeigen von Ordnerdetails
* Anzeigen und Aktualisieren von Asset-Metadaten und Schlüsselwörtern

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on&enablevpops=1)

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

Um Assets zu finden, die in einem bestimmten Metadatenfeld keine Informationen enthalten, geben Sie das Feld ein, das Sie in diesem Format suchen möchten: ?[xxxxx]. Wenn Sie beispielsweise nach Assets suchen möchten, denen keine Keywords zugewiesen sind, geben Sie im Suchfeld [Keyword] ein.

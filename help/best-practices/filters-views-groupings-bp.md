---
title: Best Practice – Filter, Ansichten und Gruppierungen
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Filtern, -Ansichten und -Gruppierungen empfehlen.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 100%

---

# Best Practice – Filter, Ansichten und Gruppierungen

## Was ist eine „Best Practice“ für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des „Warum“ vertraut zu machen.

Die Frage „Warum sind das Best Practices?“ nach der Übersichtsliste finden Sie weitere Details zu einigen der Best Practices und dazu, warum Prozesse, Werkzeuge usw. als solche angesehen werden und Sie sie in Ihrer Workfront-Instanz implementieren sollten.

</br>
</br>

## Best Practices für Filter, Ansichten und Gruppierungen

* Reduzieren Sie durch die Nutzung von Filtern, Ansichten und Gruppierungen die Anzahl der benutzerspezifischen Berichte, die Sie auf einer Objektliste erstellen, um die benötigten Daten abzurufen.

* Verwenden Sie die Listensteuerelemente in Layout-Vorlagen, um nicht benötigte Filter, Ansichten und Gruppierungen für häufig verwendete Objekte (Projekte, Aufgaben, Programme usw.) auszublenden.

* Geben Sie über die Listensteuerelemente der Layout-Vorlagen benutzerdefinierte Filter, Ansichten und Gruppierungen frei, die für die Workflows und Prozesse Ihres Unternehmens relevant sind.

* Verwenden Sie beim Erstellen von Filtern für den Projekt-, den Aufgaben- oder den Problemstatus die Option (Objekt)>>„Status entspricht der Feldquelle/dem Feldnamen“ mit dem Gleichheitsmodifikator, nicht Projekt>>„Status Feldquelle/Feldname“.

</br>
</br>

## Warum sind das Best Practices?

**Best Practice**

Reduzieren Sie durch die Nutzung von Filtern, Ansichten und Gruppierungen die Anzahl der benutzerspezifischen Berichte, die Sie auf einer Objektliste erstellen, um die benötigten Daten abzurufen.

**Das sind die Gründe**

Die Erstellung von einmaligen Nutzungsberichten für jedes Datensegment, das Sie sehen möchten, ist zeitaufwendig und füllt das Workfront-System unnötig.

Weitere Informationen zum Erstellen von Berichten mit Eingabeaufforderungen finden Sie im Kapitel „Einrichtung und Verwendung von Berichtsaufforderungen“ im Video [Grundlegendes zu Berichtseinstellungen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html?lang=de).

Weitere Informationen zum Erstellen von Berichten mit benutzerdefinierten Eingabeaufforderungen finden Sie unter [Erstellen von benutzerdefinierten Eingabeaufforderungen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html?lang=de).

</br>
</br>

**Best Practice**

Verwenden Sie die Listensteuerelemente in Layout-Vorlagen, um nicht benötigte Filter, Ansichten und Gruppierungen für häufig verwendete Objekte (Projekte, Aufgaben, Programme usw.) auszublenden.

**Das sind die Gründe**

Weniger ist mehr. Das Ausblenden von Optionen für Filter, Ansichten und Gruppierungslisten, die für die täglichen Workflows Ihrer Benutzenden nicht relevant sind, führt zu kleineren Listen, wodurch Benutzende schneller das Benötigte finden können.

Weitere Informationen zum Ausblenden von Filtern, Ansichten oder Gruppierungen mit Layout-Vorlagen finden Sie unter [Anpassen von Berichtslisten mit Layout-Vorlagen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=de).

</br>
</br>

**Best Practice**

Geben Sie über die Listensteuerelemente der Layout-Vorlagen benutzerdefinierte Filter, Ansichten und Gruppierungen frei, die für die Workflows und Prozesse Ihres Unternehmens relevant sind.

**Das sind die Gründe**

Wenn Sie Filter, Ansichten und Gruppierungen erstellt haben, die spezifische Informationen zu den täglichen Prozessen der Benutzenden anzeigen, können Sie diese ganz einfach über die Layout-Vorlagen freigeben. Dadurch wird sichergestellt, dass jede zugewiesene Layout-Vorlage über die Filter-, Ansicht- und Gruppierungsoptionen verfügt, die für ihre Workflows relevant sind.

Das Anpassen der Informationen, die Sie Ihren Benutzenden über die Layout-Vorlagen anzeigen möchten, ist außerdem zeitsparend für System- und Gruppenadmins, da sie nicht jeden Filter, jede Ansicht und jede Gruppierungsoption einzeln freigeben müssen.

Weitere Informationen darüber, wie Sie Filter, Ansichten oder Gruppierungen mit Layout-Vorlagen gemeinsam nutzen können, finden Sie unter [Anpassen von Berichtslisten mit Layout-Vorlagen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=de).

</br>
</br>

**Best Practice**

Verwenden Sie beim Erstellen von Filtern für den Projekt-, den Aufgaben- oder den Problemstatus die Option (Objekt)>>„Status entspricht der Feldquelle/dem Feldnamen“ mit dem Gleichheitsmodifikator, nicht Projekt>>„Status Feldquelle/Feldname“.

**Das sind die Gründe**

Durch die Verwendung von (Objekt)>>„Entspricht“ werden alle benutzerdefinierten Status, denen dieser spezifische Status im Feld „Entspricht“ zugewiesen ist, in die Statuseinstellungen aufgenommen. Die Einrichtung des Filters als (Objekt)>>„Status“ > „Gleich“ erfordert hingegen, dass Sie bestimmte Statuten für den Filter auswählen. Dies könnte eine Herausforderung für die Wartung darstellen, wenn Sie diese neuen Status in verschiedenen Filtern berücksichtigen müssen. Jeder Filter muss nämlich geöffnet und mit dem neuen Status aktualisiert werden.

Wenn Sie z. B. alle aktuellen Projekte sehen möchten, können Sie Ihren Filter so einrichten, dass er Projekt>>„Status“ > „Gleich“ > „Aktuell“ lautet. Wenn jedoch jemand einen benutzerdefinierten Status namens „Aktiv“ hinzufügt und ihn mit „Aktuell“ gleichsetzt, findet dieser Filter keine Projekte mit dem Status „Aktiv“. Wenn Sie jedoch Projekt>> „Status entspricht“ > „Gleich“ > „Aktuell“ verwenden, sucht der Filter Objekte mit dem Status „Aktuell“ oder „Aktiv“, da beide im Feld „Entspricht” den Eintrag „Aktuell” enthalten.

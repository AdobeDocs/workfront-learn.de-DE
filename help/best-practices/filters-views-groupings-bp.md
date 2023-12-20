---
title: Best Practice - Filter, Ansichten und Gruppierungen
description: Erfahren Sie mehr über Best Practices-Empfehlungen von Adobe Workfront-Experten zum Einrichten, Verwalten und Verwenden von Workfront-Filtern, -Ansichten und -Gruppierungen.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Best Practice - Filter, Ansichten und Gruppierungen

## Was ist eine Adobe Workfront-Best Practice?

Best Practices sind Richtlinien, die einen effektiven, effizienten Handlungsweg darstellen, von Ihnen und den Benutzern in Ihrem Unternehmen einfach übernommen werden und in Ihrem gesamten Unternehmen erfolgreich repliziert werden können.

Beachten Sie bei der Überprüfung dieser Empfehlungen, dass einige Workfront-Best Practices universell sind, während andere genauer auf das Thema eingehen können. Verwenden Sie diese Best Practices als Framework, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Auf dieser Seite navigieren

Wenn Sie durch diese Seite blättern, finden Sie zunächst eine allgemeine Liste aller Best Practices für das Thema. Auf diese Weise können Sie die Empfehlungen überprüfen, ohne sich mit den Details des &quot;Warum&quot;vertraut zu machen.

Die &quot;Warum sind diese Best Practices?&quot; -Bereich, der sich hinter der allgemeinen Liste befindet, detaillierter über einige der Best Practices und darüber, warum sie als Prozess, Tool usw. betrachtet werden, sollten Sie eine Implementierung mit Ihrer Workfront-Instanz in Erwägung ziehen.

</br>
</br>

## Best Practices für Filter, Ansichten und Gruppierungen

* Reduzieren Sie die Anzahl der benutzerspezifischen Berichte, die Sie durch die Nutzung von Filtern, Ansichten und Gruppierungen auf einer Objektliste erstellen, um die benötigten Daten abzurufen.

* Verwenden Sie die Listensteuerelemente in Layoutvorlagen, um nicht benötigte Filter, Ansichten und Gruppierungen für häufig verwendete Objekte (Projekte, Aufgaben, Programme usw.) auszublenden.

* Geben Sie benutzerdefinierte Filter, Ansichten und Gruppierungen frei, die für die Workflows und Prozesse Ihres Unternehmens relevant sind, und zwar über die Listensteuerelemente der Layoutvorlagen.

* Verwenden Sie beim Erstellen von Filtern für den Projektstatus, den Aufgabenstatus oder den Problemstatus (Objekt)>>Status entspricht dem Feld-Quell-/Feldnamen mit dem Gleichheitsmodifikator und nicht mit dem Feld Projekt >>Status-Feldquelle/-Feldnamen.

</br>
</br>

## Warum sind diese Best Practices?

**Best Practice**

Reduzieren Sie die Anzahl der benutzerspezifischen Berichte, die Sie durch die Nutzung von Filtern, Ansichten und Gruppierungen auf einer Objektliste erstellen, um die benötigten Daten abzurufen.

**Deshalb**

Die Erstellung von einmaligen Nutzungsberichten für jedes Datensegment, das Sie sehen möchten, ist zeitaufwendig und führt zu einer Optimierung des Workfront-Systems.

Anweisungen zum Erstellen von Berichten mit Eingabeaufforderungen finden Sie im Kapitel &quot;Einrichtung und Verwendung von Berichtsaufforderungen&quot;im [Grundlegendes zu Berichtseinstellungen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html) Video.

Anweisungen zum Erstellen von Berichten mit benutzerdefinierten Eingabeaufforderungen finden Sie unter [Benutzerdefinierte Eingabeaufforderungen erstellen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html).

</br>
</br>

**Best Practice**

Verwenden Sie die Listensteuerelemente in Layoutvorlagen, um nicht benötigte Filter, Ansichten und Gruppierungen für häufig verwendete Objekte (Projekte, Aufgaben, Programme usw.) auszublenden.

**Deshalb**

Weniger ist mehr. Das Ausblenden von Filter-, Anzeige- und Gruppierungslisten-Optionen, die für die täglichen Workflows Ihrer Benutzer nicht relevant sind, führt zu einer Verkleinerung der Listen, wodurch Benutzer schneller das benötigten finden können.

Anweisungen zum Ausblenden von Filtern, Ansichten oder Gruppierungen mit Layoutvorlagen finden Sie unter [Berichtslisten mit Layoutvorlagen anpassen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**Best Practice**

Geben Sie benutzerdefinierte Filter, Ansichten und Gruppierungen frei, die für die Workflows und Prozesse Ihres Unternehmens relevant sind, und zwar über die Listensteuerelemente der Layoutvorlagen.

**Deshalb**

Wenn Sie Filter, Ansichten und Gruppierungen erstellt haben, die Informationen zu den täglichen Prozessen der Benutzer anzeigen, ist es einfach, diese über die Layoutvorlagen freizugeben. Dadurch wird sichergestellt, dass jede zugewiesene Layout-Vorlage über Filter-, Ansicht- und Gruppierungsoptionen verfügt, die für ihre Workflows relevant sind.

Das Anpassen der Informationen, die Sie Ihren Benutzern über die Layoutvorlagen anzeigen möchten, ist außerdem zeitsparend für System- und Gruppenadministratoren, da sie nicht jeden Filter, jede Ansicht und jede Gruppierungsoption einzeln freigeben müssen.

Anweisungen zum Freigeben von Filtern, Ansichten oder Gruppierungen für Layoutvorlagen finden Sie unter [Berichtslisten mit Layoutvorlagen anpassen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**Best Practice**

Verwenden Sie beim Erstellen von Filtern für den Projektstatus, den Aufgabenstatus oder den Problemstatus (Objekt)>>Status entspricht dem Feld-Quell-/Feldnamen mit dem Gleichheitsmodifikator und nicht mit dem Feld Projekt >>Status-Feldquelle/-Feldnamen.

**Deshalb**

Mithilfe von (Objekt)>>Gleich mit schließen Sie alle benutzerdefinierten Status ein, denen dieser spezifische Status im Feld Gleich mit in den Statuskonfigurationen zugewiesen ist. Beim Einrichten des Filters unter (Objekt) > Status > Gleich müssen Sie hingegen bestimmte Status für den Filter auswählen. Dies könnte eine Wartungsaufgabe darstellen, wenn Sie diese neuen Status in verschiedenen Filtern berücksichtigen müssen. Jeder Filter muss geöffnet und mit dem neuen Status aktualisiert werden.

Wenn Sie beispielsweise alle aktuellen Projekte sehen möchten, können Sie Ihren Filter so einrichten, dass er Projekt > Status > Gleich > Aktuell liest. Wenn jedoch jemand einen benutzerdefinierten Status namens &quot;Aktiv&quot;hinzufügt und ihn mit &quot;Aktuell&quot;gleicht, findet dieser Filter keine Projekte mit dem Status &quot;Aktiv&quot;. Wenn Sie jedoch Projekt > Status entspricht > Gleich > Aktuell verwenden, sucht der Filter Objekte mit dem Status Aktuell oder Aktiv, da beide im Feld Gleicht mit über Aktuelles verfügen.

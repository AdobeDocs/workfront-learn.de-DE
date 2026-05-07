---
title: Best Practice – Status
description: Erfahren Sie, was Adobe Workfront-Fachleute als Best Practices für das Einrichten, Verwalten und Verwenden von Workfront-Status empfehlen.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
TQID: https://experienceleague.adobe.com/Kn7jpCG-G7sEt6kKykK0MBlFTHkiXUqVC6mrodKm-rA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 591
ht-degree: 87%

---

# Best Practice – Status

## Was ist eine Best Practice für Adobe Workfront?

Best Practices sind Richtlinien, die eine effektive, effiziente Vorgehensweise darstellen, die von Ihnen und den Benutzenden in Ihrem Unternehmen leicht übernommen werden können und die sich in Ihrem Unternehmen erfolgreich wiederholen lassen.

Bei der Durchsicht dieser Empfehlungen sollten Sie bedenken, dass einige Best Practices von Workfront universell sind, während andere eher themenspezifisch sind. Verwenden Sie diese Best Practices als Rahmen, um die Einrichtung und Verwendung Ihrer Workfront-Systeme zu unterstützen.

## Navigieren auf dieser Seite

Wenn Sie durch diese Seite scrollen, finden Sie zunächst eine allgemeine Liste aller Best Practices zu dem Thema. So können Sie die Empfehlungen durchgehen, ohne in die Details des „Warum“ einzutauchen.

Der Bereich „Warum sind diese Best Practices?“, der nach der allgemeinen Liste zu finden ist, bietet detailliertere Informationen zu einigen der Best Practices und warum sie als Prozess, Tool usw. angesehen werden. Sie sollten die Implementierung mit Ihrer Workfront-Instanz in Betracht ziehen.

</br>
</br>

## Best Practices für Status

* Behalten Sie beim Umbenennen der Standardstatus von Workfront den ursprünglichen Zweck des Status bei.

* Wenn Sie einen benutzerdefinierten Projektstatus für „Abgebrochen“ erstellen, müssen Sie den Status mit „Eingestellt“ gleichsetzen.

* Halten Sie globale benutzerdefinierte Status auf ein Minimum beschränkt.

* Verwenden Sie keine Projektstatus anstelle von Aufgaben, um den Fortschritt eines Projekts anzuzeigen.


</br>
</br>



## Warum sind das Best Practices?

**Best Practice**

Behalten Sie beim Umbenennen der Standardstatus von Workfront den ursprünglichen Zweck des Status bei.



**Das sind die Gründe**

Einige Aktionen in Workfront werden durch Standardstatus des Systems ausgelöst. Eine Änderung der Statusabsicht kann sich auf das Verhalten von Workfront in bestimmten Situationen wie die Berichterstellung usw. auswirken.



Der Standard-Aufgabenstatus „Abgeschlossen“ weist Workfront beispielsweise an, den Fertigstellungsgrad einer Aufgabe auf 100 % zu ändern. Der Status „Abgeschlossen“ teilt Workfront auch mit, dass die Arbeit an abhängigen Aufgaben beginnen kann. Wenn Sie den Namen des Status in „Warten“ geändert haben, um anzugeben, dass die Bearbeitung einer Aufgabe ausgesetzt ist, geht Workfront davon aus, dass die Aufgabe abgeschlossen ist, und startet die nächsten Schritte im Projekt.

</br>
</br>



**Best Practice**

Wenn Sie einen benutzerdefinierten Projektstatus für „Abgebrochen“ erstellen, müssen Sie den Status mit „Eingestellt“ gleichsetzen.



**Das sind die Gründe**

Wenn Sie „Abgebrochen“ mit „Abgeschlossen“ gleichsetzen, können Sie den Status nicht verwenden, um ein Projekt abzubrechen, solange nicht alle Aufgaben als abgeschlossen markiert und alle Probleme geschlossen sind. Wenn Sie „Abgebrochen“ mit „Eingestellt“ gleichsetzen, können Sie das Projekt abbrechen, ohne etwas im historischen Eintrag zu ändern.


</br>
</br>

**Best Practice**

Halten Sie globale benutzerdefinierte Status auf ein Minimum beschränkt.



**Das sind die Gründe**

Weniger ist mehr. Zu viele benutzerdefinierte Status führen nicht nur zu unnötiger Wartung, sondern auch zu Verwirrung, insbesondere bei der Arbeit an funktionsübergreifenden Projekten. Machen Sie stattdessen benutzerdefinierte Status gruppenspezifisch. Dadurch bleibt Ihre Workfront-Umgebung sauberer und ist besser für eine künftige Erweiterung auf andere Gruppen gerüstet. Arbeiten Sie mit Ihrem Governance-/Aufsichtsausschuss und den Interessengruppen zusammen, um die Status zu ermitteln, die die Gruppen Ihres Unternehmens benötigen.


</br>
</br>

**Best Practice**

Verwenden Sie keine Projektstatus anstelle von Aufgaben, um den Fortschritt eines Projekts anzuzeigen.



**Das sind die Gründe**

Halten Sie den Projektstatus einfach, um allgemeine Fortschrittsphasen wie Planung, Aktuell, Abgeschlossen usw. anzuzeigen. Anhand der Aufgaben, Aufgabenstatus und des Prozentsatzes der abgeschlossenen Aufgabe können Sie sehen, wie die Arbeit am Projekt insgesamt voranschreitet. Diese Indikatoren auf Aufgabenebene münden in den prozentualen Fertigstellungsgrad, den Projektzustand und den Projektfortschrittsstatus, die alle bessere und genauere Indikatoren für den Projektfortschritt sind als der Projektstatus. Darüber hinaus bieten diese Informationen auf Aufgabenebene bessere Berichte zu Projekten.

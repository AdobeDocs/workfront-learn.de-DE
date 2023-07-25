---
title: Antworten auf häufig gestellte Fragen zu Anforderungswarteschlangen
description: Antworten auf häufig gestellte Fragen zu Anforderungswarteschlangen in [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ce2aad1cd0ecb7d568ed9a01d97147cbd126ca05
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Häufige Fragen zu Anforderungswarteschlangen

**Warum kann ich eine Anforderungswarteschlange sehen, mein Benutzer jedoch nicht?**

Im [!UICONTROL Warteschlangendetails] -Registerkarte Ihrer Anforderungswarteschlange/Ihres -Projekts festlegen, stellen Sie sicher, dass Ihr Benutzer den Kriterien &quot;Wer kann dieser Warteschlange Anforderungen hinzufügen?&quot;entspricht. -Feld.

**Ich habe Benutzern Zugriff auf die Warteschlange gewährt, aber jetzt können sie auch das Projekt für die Anforderungswarteschlange sehen. Warum?**

Dies hängt damit zusammen, wie Sie ihnen Zugriff auf die Anforderungswarteschlange gewährt haben.

Wenn Sie die [!UICONTROL Freigabe] über die Landingpage des Anforderungswarteschlangenprojekts aus, haben Sie diesen Benutzern Zugriff gewährt, um das Projekt in der Liste der Projekte anzuzeigen.

Wenn Sie ihnen jedoch nur Zugriff gewähren möchten, um eine Anforderung an die Warteschlange zu senden, gehen Sie zur Warteschlangeneinrichtung und wählen Sie die entsprechende Option unter &quot;Wer kann diesem Projekt Anforderungen hinzufügen&quot;.

**Kann ich eine Anfrage in ein Projekt umwandeln?**

Ja. Sie können Probleme je nach Bedarf in Aufgaben oder Projekte konvertieren.

Weitere Informationen finden Sie in diesem Artikel . [Konvertierungsprobleme](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**Wo finde ich eine Anforderungswarteschlange zum Bearbeiten?**

Sie können die [!UICONTROL Suche] in der Navigationsleiste ein oder finden Sie sie in der Liste [!UICONTROL Projekte] Bereich.

Wenn Sie eine Anforderung aus der Anforderungswarteschlange öffnen, können Sie im Bereich &quot;Breadcrumbs&quot;auf den Projektnamen klicken.

**Kann ich die Informationen von einem benutzerdefinierten Anforderungsformular in ein benutzerdefiniertes Projekt-Formular übertragen?**

Ja. Wenn Sie ein benutzerdefiniertes Formular erstellen, wählen Sie beide [!UICONTROL Projekt] und [!UICONTROL Problem] als Objekttypen. Hängen Sie das benutzerdefinierte Formular an die Anforderung an. Wenn Sie die Anforderung in ein Projekt konvertieren, wird das benutzerdefinierte Formular automatisch an das neue Projekt angehängt und die in allen Feldern enthaltenen Werte werden sowohl in der Anforderung als auch in den benutzerdefinierten Formularen des Projekts angezeigt.

**Ich sehe mir einen Projekt- oder Aufgabenbericht an. Wie finde ich heraus, von welcher Anforderung dieses Objekt stammt?**

Sie können auf Felder im **[!UICONTROL Konvertierte Ausgabe]** und **[!UICONTROL Urheber einer konvertierten Ausgabe]** -Felderquellen, um diese Informationen zu Ihren Projekt- und Aufgabenberichten hinzuzufügen.

**Wie lässt sich am besten nach Anforderungswarteschlangen in einem Bericht filtern?**

Wenn Ihr Projektfilter **Warteschlange >>Ist öffentlich>>Gleich>>Keine** Ihr Bericht zeigt nur Projekte an, die **NOT** Warteschlangen anfordern.

Wenn Ihr Projektfilter **Warteschlange >>Ist öffentlich>>Nicht gleich>>Keine** Ihr Bericht zeigt nur Projekte an, die **ARE** Warteschlangen anfordern.

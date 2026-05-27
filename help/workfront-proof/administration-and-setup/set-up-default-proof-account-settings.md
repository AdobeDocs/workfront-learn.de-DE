---
title: Einrichten der Standardeinstellungen für ein Korrekturabzugskonto
description: Erfahren Sie, wie Sie Standardkontoeinstellungen einrichten, die global für alle Korrekturabzüge und Proofing-Benutzende gelten.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:04:10.059Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 569
ht-degree: 95%

---

# Einrichten der Standardeinstellungen für ein Korrekturabzugskonto

Legen Sie Standardkontoeinstellungen fest, die global für alle Korrekturabzüge und Proofing-Benutzende gelten – Land, Sprache und Zeitzone. Wenn Sie Benutzende über mehrere Zeitzonen oder Länder hinweg haben, können Sie diese Einstellungen bei Bedarf am Benutzerprofil jeder Person anpassen.

![Fenster mit Kontoeinstellungen für das Proofing](assets/proof-system-setups-default-account-settings.png)

1. Wählen Sie aus dem [!DNL Workfront's] [!UICONTROL Hauptmenü] die Option **[!UICONTROL Proofing]** aus.
1. Wählen Sie **[!UICONTROL Kontoeinstellungen]** in der oberen Navigationsleiste aus.
1. Wählen Sie die Registerkarte **[!UICONTROL Details]** aus.
1. Navigieren Sie zum Feld [!UICONTROL Land] und wählen Sie **[!UICONTROL Bearbeiten]** aus. Wählen Sie als Standard das Land aus, in dem sich die meisten Proofing-Benutzenden befinden.
1. Wählen Sie **[!UICONTROL Speichern]** für diese Einstellung aus.
1. Navigieren Sie zum Feld [!UICONTROL Standardsprache] und wählen Sie **[!UICONTROL Bearbeiten]** aus. Wählen Sie als Standard die Sprache aus, die die meisten Proofing-Benutzenden verwenden.
1. Wählen Sie für diese Einstellung **[!UICONTROL Speichern]** aus.
1. Navigieren Sie zum Feld [!UICONTROL Zeitzonen-Standard] und wählen Sie **[!UICONTROL Bearbeiten]** aus. Wählen Sie als Standard die Zeitzone aus, in der sich die meisten Proofing-Benutzenden befinden. Dies ist die Zeitzone, die von manuell eingerichteten Korrekturabzug-Workflows erkannt wird. Sie gilt ebenfalls für Vorlagen von Korrekturabzug-Workflows, aber für jede Vorlage kann auch eine Zeitzone festgelegt werden.
1. Wählen Sie für diese Einstellung **[!UICONTROL Speichern]** aus.

## Best Practices


| Best Practice | Das sind die Gründe |
|---|---|
| Passen Sie die Backend-Einstellungen für den Korrekturabzug an, damit Benutzende Fristen im 12-Stunden-Zeitformat sehen können. | Wählen Sie die Option F j, Y, gi:a in den Korrekturabzugseinstellungen für Benutzer aus, die die Fristen für den Korrekturabzug in einem AM/PM-Format anzeigen möchten. Für Gebiete, in denen das 12-Stunden-Zeitformat gängig ist, sorgt dies für mehr Klarheit bei den Fristen. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Benutzer“. Bearbeiten Sie dort für jede Person das Feld „Datumsformat“. |
| Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Frist für den Korrekturabzug fest. | Wenn eine standardmäßige Korrekturabzugsfrist – Hochladedatum + x Anzahl von Werktagen – festgelegt ist und die Person, die den Korrekturabzug erstellt hat, vergisst, eine Frist hinzuzufügen, wendet Workfront diese Frist automatisch auf jeden hochgeladenen Korrekturabzug an. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Einstellungen“ > „Korrrekturabzugs-Standardeinstellungen“ im Feld „Frist (+ Werktage)“. |
| Blenden Sie die Korrekturabzugsentscheidungs-Option „Nicht relevant“ aus. | Diese Entscheidungsoption führt bei genehmigenden Personen häufig zu Verwirrung, da Organisationen oft nicht definieren, wann die Option „Nicht relevant“ verwendet werden soll. Die Option „Nicht relevant“ weist im Allgemeinen darauf hin, dass der Korrekturabzug für die Empfängerin oder den Empfänger des Korrekturabzugs nicht relevant ist und dass diese Person keine Genehmigungs- oder Ablehnungsentscheidung treffen muss. Durch die Auswahl von „Nicht relevant“ kann der Korrekturabzug-Workflow fortgesetzt werden.<br> <br>Die Option „Nicht relevant“ ist in den meisten Korrekturabzug-Workflows nicht erforderlich.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“. |
| Ordnen Sie die Optionen für die Korrekturabzugsentscheidung in den Korrekturabzugseinstellungen nicht neu an. | Jede Einstellung für die Korrekturabzugsentscheidung umfasst einen bestimmten Wert bzw. eine bestimmte Gewichtung, was bei einer Neuanordnung in Bezug auf Ihre Korrekturabzugskonfigurationen zu Verwirrung führen kann. Die Entscheidungsreihenfolge und der Wert/die Gewichtung werden als Trigger für die Aktivierung der Korrekturphase und beim Reporting verwendet.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“. |
| Legen Sie Benutzerstandardeinstellungen für Korrekturabzugsrollen und E-Mail-Warnhinweise fest. | Diese Einstellungen werden automatisch angegeben, wenn Sie einen Korrekturabzug-Workflow zuweisen. Auf diese Weise wird der Vorgang beschleunigt und trägt zur Konsistenz der Korrekturabzug-Workflows bei.<br> <br>Hinweis: Die Standardeinstellungen für Benutzende finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Benutzer“. Wählen Sie dann die Person aus, für die die Standardeinstellungen festgelegt werden sollen. |

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
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: ht
source-wordcount: '563'
ht-degree: 100%

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
| Passen Sie die Backend-Einstellungen für den Korrekturabzug an, damit Benutzende Fristen im 12-Stunden-Zeitformat sehen können. | Wählen Sie in den Korrekturabzugseinstellungen die Option „F j, Y, gi:a“ für Benutzende aus, die die Korrekturabzugsfristen/-zeiten im AM/PM-Format sehen möchten. Für Gebiete, in denen das 12-Stunden-Zeitformat gängig ist, sorgt dies für mehr Klarheit bei den Fristen. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Benutzer“. Bearbeiten Sie dort für jede Person das Feld „Datumsformat“. |
| Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Frist für den Korrekturabzug fest. | Wenn eine standardmäßige Korrekturabzugsfrist – Hochladedatum + x Anzahl von Werktagen – festgelegt ist und die Person, die den Korrekturabzug erstellt hat, vergisst, eine Frist hinzuzufügen, wendet Workfront diese Frist automatisch auf jeden hochgeladenen Korrekturabzug an. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Einstellungen“ > „Korrrekturabzugs-Standardeinstellungen“ im Feld „Frist (+ Werktage)“. |
| Blenden Sie die Korrekturabzugsentscheidungs-Option „Nicht relevant“ aus. | Diese Entscheidungsoption führt bei genehmigenden Personen häufig zu Verwirrung, da Organisationen oft nicht definieren, wann die Option „Nicht relevant“ verwendet werden soll. Die Option „Nicht relevant“ weist im Allgemeinen darauf hin, dass der Korrekturabzug für die Empfängerin oder den Empfänger des Korrekturabzugs nicht relevant ist und dass diese Person keine Genehmigungs- oder Ablehnungsentscheidung treffen muss. Durch die Auswahl von „Nicht relevant“ kann der Korrekturabzug-Workflow fortgesetzt werden.<br> <br>Die Option „Nicht relevant“ ist in den meisten Korrekturabzug-Workflows nicht erforderlich.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“. |
| Ordnen Sie die Optionen für die Korrekturabzugsentscheidung in den Korrekturabzugseinstellungen nicht neu an. | Jede Einstellung für die Korrekturabzugsentscheidung umfasst einen bestimmten Wert bzw. eine bestimmte Gewichtung, was bei einer Neuanordnung in Bezug auf Ihre Korrekturabzugskonfigurationen zu Verwirrung führen kann. Die Entscheidungsreihenfolge und der Wert/die Gewichtung werden als Trigger für die Aktivierung der Korrekturphase und beim Reporting verwendet.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Entscheidungen“. |
| Legen Sie Benutzerstandardeinstellungen für Korrekturabzugsrollen und E-Mail-Warnhinweise fest. | Diese Einstellungen werden automatisch angegeben, wenn Sie einen Korrekturabzug-Workflow zuweisen. Auf diese Weise wird der Vorgang beschleunigt und trägt zur Konsistenz der Korrekturabzug-Workflows bei.<br> <br>Hinweis: Die Standardeinstellungen für Benutzende finden Sie im Workfront-Hauptmenü unter „Proofing“ > „Kontoeinstellungen“ > „Benutzer“. Wählen Sie dann die Person aus, für die die Standardeinstellungen festgelegt werden sollen. |

---
title: Standardeinstellungen für Testversandkonto einrichten
description: Erfahren Sie, wie Sie Standardkontoeinstellungen einrichten, die global für alle Benutzer von Testsendungen und Testsendungen gelten.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Standardeinstellungen für Testversandkonto einrichten

Legen Sie Standardkontoeinstellungen fest, die global für alle Testsendungen und Testversand-Benutzer gelten - Land, Sprache und Zeitzone. Wenn Sie Benutzer über mehrere Zeitzonen oder Länder hinweg haben, können Sie diese Einstellungen bei Bedarf am Benutzerprofil jedes Einzelnen anpassen.

![Fenster mit Kontoeinstellungen für die Prüfung](assets/proof-system-setups-default-account-settings.png)

1. Auswählen **[!UICONTROL Testing]** von [!DNL Workfront's] [!UICONTROL Hauptmenü].
1. Auswählen **[!UICONTROL Kontoeinstellungen]** in der oberen Navigationsleiste.
1. Wählen Sie die **[!UICONTROL Details]** Registerkarte.
1. Navigieren Sie zu [!UICONTROL Land] Feld und wählen Sie **[!UICONTROL Bearbeiten]**. Wählen Sie als Standard das Land aus, in dem sich die meisten Testversand-Benutzer befinden.
1. Auswählen **[!UICONTROL Speichern]** für diese Einstellung.
1. Navigieren Sie zu [!UICONTROL Standardsprache] Feld und wählen Sie **[!UICONTROL Bearbeiten]**. Wählen Sie die Sprache aus, die die meisten Testversand-Benutzer als Standard verwenden.
1. Auswählen **[!UICONTROL Speichern]** für diese Einstellung.
1. Navigieren Sie zu [!UICONTROL Zeitzonen-Standard] Feld und wählen Sie **[!UICONTROL Bearbeiten]**. Wählen Sie die Zeitzone aus, in der sich die meisten Testversand-Benutzer als Standard befinden. Dies ist die Zeitzone, die von manuell eingerichteten Testversand-Workflows erkannt wird. Sie gilt auch für Testversand-Workflow-Vorlagen, aber jede Vorlage kann über eine Zeitzone verfügen.
1. Auswählen **[!UICONTROL Speichern]** für diese Einstellung.

## Best Practices


| Best Practice | Deshalb |
|---|---|
| Passen Sie die Back-End-Einstellungen für den Testversand an, damit Benutzer Termine im 12-Stunden-Uhrzeitformat sehen können. | Wählen Sie die Option F j, Y, gi:a in den Testversandeinstellungen für Benutzer aus, die die Testversandfristen/-zeiten im AM/PM-Format sehen möchten. Für Bereiche, die eine 12-Stunden-Uhr verwenden, hilft dies bei der Klarheit der Termine. <br> <br>Hinweis: Diese Einstellung können Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Benutzer > vornehmen und für jeden Benutzer das Feld Datumsformat bearbeiten. |
| Legen Sie im Rahmen der Systemeinstellungen eine standardmäßige Testversand-Deadline fest. | Wenn der Ersteller eines Testversands vergisst, einen Termin hinzuzufügen, wendet Workfront diesen Termin automatisch auf jeden hochgeladenen Testversand an. <br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Einstellungen > Testversand-Standard > Versandgültigkeit (+ Geschäftstage) -Feld. |
| Blenden Sie die Option Nicht relevante Testversandentscheidung aus. | Diese Entscheidungsoption führt bei Genehmigern häufig zu Verwirrung, da Organisationen häufig nicht definieren, wann die Option Nicht relevant verwendet werden soll. Die Option Nicht relevant weist im Allgemeinen darauf hin, dass der Testversand für den Testversand-Empfänger nicht relevant ist und dass er keine genehmigte oder abgelehnte Entscheidung treffen muss. Durch die Auswahl von Nicht relevant kann der Testversand-Workflow fortgesetzt werden.<br> <br>Die Option Nicht relevant ist in den meisten Testversand-Workflows nicht erforderlich.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Entscheidungen. |
| Ordnen Sie die Testversand-Entscheidungsoptionen in den Testversandeinstellungen nicht neu an. | Jede Einstellung der Testversandentscheidung enthält einen bestimmten Wert/eine bestimmte Gewichtung, die bei einer Neuanordnung Verwirrung in Ihren Testversandkonfigurationen verursachen kann. Die Entscheidungsreihenfolge und der Wert/die Gewichtung werden als Trigger für die Aktivierung der Testphase und in Berichten verwendet.<br> <br>Hinweis: Diese Einstellung finden Sie im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Entscheidungen. |
| Legen Sie Benutzerstandardeinstellungen für Testadressen und E-Mail-Warnungen fest. | Diese Einstellungen werden automatisch ausgefüllt, wenn Sie einen Testversand-Workflow zuweisen, den Prozess beschleunigen und zur Konsistenz der Testversand-Workflows beitragen.<br> <br>Hinweis: Die Standardeinstellungen der Benutzer werden im Workfront-Hauptmenü > Testversand > Kontoeinstellungen > Benutzer > angezeigt. Wählen Sie dann den Benutzer aus, für den die Standardeinstellungen festgelegt werden sollen. |

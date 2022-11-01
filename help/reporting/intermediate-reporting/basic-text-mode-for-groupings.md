---
title: Grundlegendes zum Textmodus für Gruppierungen
description: Erfahren Sie, was der Textmodus ist, welche Binnenmajuskel-Groß-/Kleinschreibung ist und welchen einfachen Textmodus Sie in Ihren Gruppierungen in Workfront verwenden können.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
source-git-commit: 6a695f84e92b576795e69aa843dd96f88b53a355
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Grundlegendes zum Textmodus für Gruppierungen

>[!IMPORTANT]
>
>Voraussetzungen:
>
>* Berichterstellungselemente
>* Berichtkomponenten verstehen
>* Basisgruppierung erstellen


In diesem Video erfahren Sie:

* Textmodus
* Was für ein Kamel ist
* Grundlegender &quot;Plug-and-Play&quot;-Textmodus, den Sie in Ihren Gruppierungen verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## 4 Elterngruppen

Im folgenden Textmodus werden Aufgaben basierend auf bis zu vier Ebenen von Eltern gruppiert und nicht vorhandene Eltern leer gelassen.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Ein Bildschirmbild mit vier übergeordneten Elementen gruppierten Projektaufgaben](assets/4-parents-grouping.png)


## Prozentuale vollständige Gruppierung

Im folgenden Textmodus werden Aufgaben basierend auf ihrem prozentualen Abschluss gruppiert. Aufgaben werden in eine der folgenden Kategorien eingeteilt, wenn sie gruppiert sind:

* 0%
* 1 % bis 25 %
* 26 % bis 50 %
* 51 % bis 75 %
* 76 % bis 99 %
* 100 %

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Ein Screenshot mit Projektanforderungen gruppiert nach Prozentsatz der Abschlüsse](assets/percent-complete-grouping.png)

## statusEquatesWith, dann status

Im folgenden Textmodus werden Aufgaben nach statusEquatesWith und dann nach Status gruppiert.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![Ein Bildschirmbild mit nach statusEquatesWith gruppierten Projektaufgaben](assets/status-equates-with.png)



---
title: Grundlegendes zum Textmodus für Ansichten
description: Erfahren Sie, was der Textmodus ist, welche Binnenmajuskel-Schreibweise verwendet wird und welchen grundlegenden Textmodus Sie in Ihren Ansichten in Workfront verwenden können.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Grundlegendes zum Textmodus für Ansichten


>[!IMPORTANT]
>
>Voraussetzungen:
>
>* Berichterstellungselemente
>* Berichtkomponenten verstehen
>* Basisansicht erstellen


In diesem Video erfahren Sie:

* Textmodus
* Was für ein Kamel ist
* Einige grundlegende Textmodi &quot;Plug-and-Play&quot;, die Sie in Ihren Ansichten verwenden können

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## Aufgabe - Ansicht &quot;4 übergeordnete Elemente&quot;

Erstellen Sie zunächst eine Spalte für den Aufgabennamen und den übergeordneten Namen und verwenden Sie dann den folgenden Textmodus, um die anderen drei Spalten zu erstellen.

### Aufgabe - Übergeordneter übergeordneter Name

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### Aufgabe - Übergeordnetes Element des übergeordneten Namens

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### Aufgabe - Übergeordnetes Element des übergeordneten Namens

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![Ein Bildschirmbild mit der Ansicht der vier übergeordneten Elemente](assets/4-parents-view.png)

## Benutzer - Iterationen, die Listen in Benutzeransichten anzeigen

### Benutzer - Alle Aufgabenrollen

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Benutzer - Alle Vorgangsrollen zeigen die primäre

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Benutzer - Alle Teams

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>Es gibt ein Team -Feld, auf das über die Benutzeroberfläche zugegriffen werden kann. Es zeigt alle Teams durch Kommas getrennt an, aber im obigen Textmodus wird jedes Team in einer separaten Zeile angezeigt.


### Benutzer - Alle Gruppen

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Benutzer - Alle Gruppen, die die Startseite anzeigen

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Benutzer - Direkte Berichte

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Benutzer - Künftiges PTO

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit der Listenansicht &quot;Benutzer&quot;](assets/user-lists-view-large.png)

## Aufgabe - So zeigen Sie Aufgabenzuweisungen an und arbeiten an einem Status

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit der Ansicht &quot;Zuweisungen und Status&quot;](assets/assignments-and-status-view.png)


## Aufgabe - So zeigen Sie Rolle und Zuordnung für mehrere Aufgabenzuweisungen an

### Aufgabe - Rolle + Stunden

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Aufgabe - Zuweisung + Prozentzuweisung

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Ein Bildschirmbild mit der Ansicht &quot;Zuweisungen und Rollen&quot;](assets/assignments-roles-and-percent-view.png)

## Aufgabe - Projektübergreifende Vorläufer und Nachfolger

### Aufgabenfilter (optional)

**Anzeigen aller Aufgaben, die mindestens einen projektübergreifenden Vorgänger haben**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Aufgabe - Anzeigen von Vorgängernamen und Projektvorläufern in

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### Aufgabe - Anzeigen der Nachfolnamen und des Nachfolgers in

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### Aufgabe - Anzeigen des voraussichtlichen Abschlussdatums der Vorgänger

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### Aufgabe - Status von Vorgängern anzeigen

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### Aufgabe - Prozentualer Abschluss des Projekts des projektübergreifenden Vorgängers anzeigen

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit der Ansicht der projektübergreifenden Vorgänger und Nachfolger](assets/cross-project-predecessors-and-successors.png)


## Aufgabe - Iteration, die alle zugewiesenen Personen anzeigt und die jede Person zugewiesen haben

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Ein Screenshot mit allen zugewiesenen Personen, denen jede Person zugewiesen wurde](assets/all-assignees-and-requesters.png)

## Aufgabe/Projekt - Iteration, die alle benutzerdefinierten Formulare in einem Projekt oder einer Aufgabe anzeigt

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Ein Bildschirmbild mit allen benutzerdefinierten Formularen in einem Projekt](assets/all-custom-forms-on-a-project.png)


## Projekt - Iteration, die alle Hauptkontakte für Resolvables in der Projektansicht anzeigt

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit Primärkontakten für Auflösungen](assets/primary-contacts-for-resolvables.png)

## Projekt - Iteration, die alle Mitglieder des Projektteams anzeigt

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![Ein Bildschirmbild, das alle Mitglieder des Projekt-Teams anzeigt](assets/all-project-team-members.png)

## Projekt - Iteration, die das entryDate aller lösbaren Probleme für ein Projekt anzeigt

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![Ein Bildschirmbild mit dem entryDate aller gelösten Probleme für ein Projekt](assets/resolvables-entry-date.png)

## Projekt - Zeigt die Startseite der ursprünglichen Projektanforderungsinstanz an

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Ein Bildschirmbild mit der Startseite des Projektanfragenden](assets/requestor-home-group.png)

## Projekt - Anzeigen, ob das Projekt eine Anforderungswarteschlange ist

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![Ein Bildschirmbild, das anzeigt, ob das Projekt eine Anforderungswarteschlange ist](assets/project-is-a-request-queue.png)

## Problem - Iteration, die alle aufgelösten Team-Mitglieder anzeigt

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit allen aufgelösten Team-Mitgliedern](assets/all-resolve-project-team-members.png)

## Problem - Iteration, die alle Teams des Hauptkontakts des Problems anzeigt

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![Ein Bildschirmbild mit allen primären Kontaktteams](assets/all-primary-contact-teams.png)

## Dokument - Iteration der Ordneranzeige in einem Dokumentbericht

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Ein Bildschirmbild mit einem Ordner in einem Dokumentbericht](assets/folder-in-a-document-report.png)

## Dokument - Iteration des übergeordneten Ordners in einem Dokumentbericht

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Ein Bildschirmbild mit einem übergeordneten Ordner in einem Dokumentbericht](assets/parent-folder-in-a-document-report.png)

## Dokument - Datum der Dokumentgenehmigung

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![Ein Bildschirmbild mit der Ansicht &quot;Document Approval Dates&quot;](assets/document-approval-dates.png)

## Korrekturabzug-Genehmigungen

### Genehmigung für Testversand - Projektname anzeigen

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Validierung des Testversands - Aufgabenname anzeigen

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Ein Bildschirmbild mit dem Projekt und der Aufgabe einer Testversand-Validierung](assets/proof-approval-project-and-task.png)


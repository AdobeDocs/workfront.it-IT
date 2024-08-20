---
title: Panoramica Del Tipo Di Licenza Quando Si Utilizza Adobe Workfront Planning
description: L’accesso a Adobe Workfront Planning dipende dal tipo di licenza, oltre che dalle autorizzazioni per gli oggetti.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning

{{planning-important-intro}}

Il tipo di licenza di Adobe Workfront funziona in combinazione con le autorizzazioni di Adobe Workfront Planning per concedere i seguenti accessi:

* Visualizzare, contribuire o gestire le aree di lavoro
* Visualizzare o gestire le visualizzazioni.

Per informazioni sulle autorizzazioni per gli oggetti in Workfront Planning, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Relazione tra i tipi di licenza di Workfront e le autorizzazioni di Workfront Planning

La tabella seguente descrive la relazione tra il tipo di licenza di un utente in Adobe Workfront e il livello di autorizzazioni che è possibile concedere agli oggetti di Adobe Workfront Planning in base a tale licenza.

La concessione di autorizzazioni utente a un&#39;area di lavoro consente inoltre di concedere autorizzazioni ai tipi di record, ai record e ai campi.


| Tipo di licenza Adobe Workfront* | Autorizzazioni massime consentite in Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nuovo: Standard <br> o <br>Corrente: Piano | Gli utenti possono gestire le aree di lavoro. Possono creare, modificare o eliminare aree di lavoro, tipi di record, record e campi. <br> Gli amministratori di sistema dispongono delle autorizzazioni di gestione per tutte le aree di lavoro, incluse quelle non create. |
| Nuovo: Light, Collaboratore <br> o <br>Corrente: Lavoro, Richiedente, Revisore | Gli utenti possono visualizzare le aree di lavoro condivise, nonché i tipi di record, i record e i campi di tali aree di lavoro. <br> Gli utenti non possono creare, modificare o eliminare aree di lavoro, tipi di record, record o campi. |

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Replace the table above with the following at GA:


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| Light or Contributor  | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

### Tipi di licenze e autorizzazioni dell’area di lavoro

Solo gli utenti con una licenza Standard (o Plan) possono disporre delle autorizzazioni Contribute o Manage per le aree di lavoro. Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le aree di lavoro condivise con loro.

Gli amministratori di sistema possono visualizzare tutte le aree di lavoro del sistema, anche quelle che non hanno creato.

Il numero di oggetti di Workfront Planning che è possibile impostare è limitato. Per informazioni, vedere [Panoramica delle limitazioni degli oggetti di Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

>[!INFO]
>
>**ESEMPIO:**
>
>I richiedenti (o i collaboratori, in base al nuovo modello di licenza) non possono contribuire o gestire le aree di lavoro e i relativi oggetti.
>
>Nella casella Condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per contribuire a o gestire un’area di lavoro quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disabilitati.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


<!--Replace all the content in the section above with the following at Planning GA


Only users with a Standard license can have Contribute or Manage permissions to workspaces. Users with all other license types can have View permissions to workspaces shared with them. 

System administrators can view all workspaces in the system, even the ones they did not create. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot contribute to or manage workspaces and their objects. 
>
>There is an indication in the sharing box that users cannot be granted permissions to contribute to or manage a workspace when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)
-->


### Tipi di licenze e autorizzazioni di visualizzazione

Solo gli utenti con una licenza Standard (o Plan) possono disporre delle autorizzazioni Manage (Gestione) per le visualizzazioni. Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le visualizzazioni condivise con loro.

>[!INFO]
>
>**ESEMPIO:**
>
>I collaboratori (o i richiedenti e i revisori) non possono gestire le visualizzazioni. Possono applicare filtri, ordinamenti o raggruppamenti temporanei alle visualizzazioni a cui possono accedere.
>
>Nella casella di condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per gestire una visualizzazione quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disattivati.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above in this section with the following at GA:

Only users with a Standard license can have Manage permissions to views. Users with all other license types can have View permissions to views shared with them. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot manage views. They can apply temporary filters, sorts, or groupings to views they can access. 
>
>There is an indication in the sharing box that users cannot be granted permissions to manage a view when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-light-user.png)-->



<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->
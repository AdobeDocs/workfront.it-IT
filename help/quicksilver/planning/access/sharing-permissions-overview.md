---
title: Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning
description: È possibile condividere o rimuovere le autorizzazioni per un'area di lavoro o una vista di Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning

{{planning-important-intro}}

È possibile condividere o rimuovere le autorizzazioni per un&#39;area di lavoro o una visualizzazione in Adobe Workfront Planning.

Questo articolo descrive i livelli di autorizzazione per gli oggetti di Workfront Planning.

Per informazioni su come condividere aree di lavoro o visualizzazioni, vedere i seguenti articoli:

* [Condividere le aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

* [Condividere le visualizzazioni](/help/quicksilver/planning/access/share-views.md)

## Oggetti condivisibili in Adobe Workfront Planning

È possibile condividere i seguenti oggetti:

* Aree di lavoro

  Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro. Le visualizzazioni non sono condivise.

* Viste

  È necessario concedere agli utenti, inclusi gli amministratori di sistema, le autorizzazioni per accedere alle visualizzazioni separatamente dalle autorizzazioni per l’accesso alle aree di lavoro. Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

Potete condividere un workspace o una vista con le seguenti entità:

* Utenti
* Gruppi

<!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->

## Considerazioni sulla condivisione di oggetti in Adobe Workfront Planning

* Il tipo di licenza Adobe Workfront funziona insieme alle autorizzazioni di Workfront Planning per consentire l’accesso alla visualizzazione, al contributo o alla gestione delle aree di lavoro e dei relativi oggetti.

  Per informazioni su come i tipi di licenza influiscono sui livelli di autorizzazione per Workfront Planning, vedere [Panoramica sui tipi di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Gli amministratori di sistema possono gestire tutte le aree di lavoro del sistema, incluse quelle che non hanno creato.
* Gli altri utenti, inclusi gli amministratori di sistema, possono accedere solo alle visualizzazioni create o condivise con loro. Gli amministratori di sistema possono disporre delle autorizzazioni necessarie solo per gestire una visualizzazione.
* È possibile condividere con altri utenti un collegamento a un&#39;area di lavoro o a una visualizzazione.

  Per poter accedere all&#39;area di lavoro o alla pagina del tipo di record visualizzata nella vista selezionata, gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront.

## Condivisione delle autorizzazioni per gli oggetti di Adobe Workfront Planning

Le tabelle delle sezioni seguenti illustrano il livello di autorizzazioni che è possibile selezionare quando si condivide un&#39;area di lavoro o una visualizzazione e le funzionalità consentite da ogni livello.

>[!IMPORTANT]
>
>Non tutti gli utenti possono disporre dei livelli di autorizzazione descritti di seguito. La licenza individuale degli utenti determina il livello di autorizzazioni che possono ricevere per gli oggetti di Workfront Planning.
>
>Solo gli utenti con licenza Standard (o Plan) possono disporre delle autorizzazioni Contribute o Manage per le aree di lavoro e delle autorizzazioni Manage per le visualizzazioni.
> 
>Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le aree di lavoro e le visualizzazioni.
>
>Per informazioni, vedere [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Autorizzazioni Workspace

È necessario concedere agli utenti le autorizzazioni per le aree di lavoro per consentire loro di accedere alle seguenti entità:

* Aree di lavoro
* Tipi di record
* Record
* Campi

Di seguito sono riportati i livelli di autorizzazione per le aree di lavoro:

|        | Gestire | Contribuisci | Viste |
|--------|--------|------------|-------|
| Modif | ✓ |            |       |
| Condividi | ✓ |            |       |
| Elimina | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni del tipo di record

Le autorizzazioni del tipo di record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

Di seguito sono riportati i livelli di autorizzazione per i tipi di record:


|        | Gestire | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni record

Le autorizzazioni dei record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

Di seguito sono riportati i livelli di autorizzazione per i record:


|        | Gestire | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ | ✓ |       |
| Modifica | ✓ | ✓ |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni campo

Le autorizzazioni per i campi vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.
Le autorizzazioni seguenti fanno riferimento ai campi stessi e non ai valori associati a ciascun campo. Per modificare i valori dei campi è necessario disporre delle autorizzazioni per la modifica dei record.

|        | Gestire | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |


### Visualizza autorizzazioni

È necessario concedere autorizzazioni separate alle visualizzazioni record. La concessione delle autorizzazioni all&#39;area di lavoro non consente di concedere le autorizzazioni alle visualizzazioni record nell&#39;area di lavoro.

È necessario concedere agli utenti le autorizzazioni per le visualizzazioni per consentire loro di accedere ai seguenti elementi di visualizzazione:

* Filtri
* Visibilità del campo
* Ordina
* Raggruppamento
* Altezza riga
* Impostazioni


<!--You can share views internally or publicly. -->

Di seguito sono riportati i livelli di autorizzazione per le visualizzazioni e gli elementi di visualizzazione:

|        | Gestisci (solo le persone invitate possono accedere) | Visualizza (solo le persone invitate possono accedere) | Tutti nell&#39;area di lavoro possono visualizzare* |
|--------|--------|-------|------------------------------|
| Modifica | ✓ |       |                            |
| Elimina | ✓ |       |                            |
| Condividi | ✓ |       |                           |
| Visualizza | ✓ | ✓ | ✓ |
| Accedere alla visualizzazione | ✓ | ✓ | ✓ |
| Applicare filtri, raggruppamenti e ordinamenti temporanei | ✓ | ✓ | ✓ |

*Gli utenti devono disporre di autorizzazioni View (Visualizzazione) o superiori per un&#39;area di lavoro per poter accedere a questa visualizzazione.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->
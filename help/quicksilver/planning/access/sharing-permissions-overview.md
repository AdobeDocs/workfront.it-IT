---
title: Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning
description: Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. In questo articolo vengono descritte le informazioni generali sulla condivisione o la rimozione delle autorizzazioni per un'area di lavoro o una visualizzazione di Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/eF7kBTsursbrsXr8Lo6ql6U5JBLQDvi6nw4JDpRxClw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: d45d85aecbcdabf2c02c347b80c7ee56b97efff0
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 5%
---
<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Panoramica delle autorizzazioni di condivisione in Pianificazione di Adobe Workfront


<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile condividere o rimuovere le autorizzazioni per un&#39;area di lavoro, un tipo di record o una visualizzazione di Adobe Workfront Planning.

È inoltre possibile condividere i moduli di richiesta di Planning. Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

In questo articolo vengono descritti i livelli di autorizzazione per le aree di lavoro di Workfront Planning, i tipi di record, i record, i campi e le visualizzazioni.

## Oggetti condivisibili in Adobe Workfront Planning

È possibile condividere manualmente alcuni oggetti di Workfront Planning, mentre altri oggetti ereditano tali autorizzazioni da altri oggetti.

In Workfront Planning è possibile condividere manualmente i seguenti oggetti:

* Aree di lavoro

  * Puoi condividere le aree di lavoro all’interno della tua organizzazione con utenti, gruppi, team, aziende e ruoli.
  * Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro.
  * Quando si condivide un&#39;area di lavoro, le visualizzazioni non vengono condivise. Le visualizzazioni sono condivise separatamente.

  Per ulteriori informazioni, vedere [Condividi aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

* Tipi di record

  * Puoi condividere i tipi di record all’interno della tua organizzazione con utenti, gruppi, team, aziende e ruoli.
  * Il livello di autorizzazioni concesse per l&#39;area di lavoro viene visualizzato come Autorizzazioni ereditate per il tipo di record.
  * Non è possibile condividere un tipo di record con un livello di autorizzazione superiore a quello dell&#39;utente nell&#39;area di lavoro.

  Per ulteriori informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).

* Record

  * Puoi condividere i record con le persone all’interno della tua organizzazione, con utenti, gruppi, team, aziende e ruoli.
  * Per impostazione predefinita, gli utenti ereditano le autorizzazioni dall’area di lavoro e dal tipo di record.
  * Non è possibile condividere un record con un livello di autorizzazione superiore o inferiore a quello dell&#39;utente sul tipo di record.

  Per ulteriori informazioni, vedere [Condividi record](/help/quicksilver/planning/access/share-records.md).

<!--
* Fields

    * In the Production environment, field permissions are inherited from record types. 

    * Field permissions grant access to field values, and not to field settings. 
    * You must have both permissions to a record and to a field to see the values of that field for a record. 

    <div class="preview">

    * In the Preview environment, consider the following: 

        * You can share fields inside your organization, with users, groups, teams, companies, and job roles. 
        * Access to a field comes from combining the following settings:

            * **Inherited permissions**: By default, a field inherits the same access someone has on the record type. You can turn off Inherited permissions and give users a lower access to the field than they have for the record type. 
            * The **Everyone with access to the record type can view** or **Only invited people can access** selection. You can either allow everyone with permissions to the workspace to view the field or give permissions only to individual entities. 
    
    For more information, see [Share fields](/help/quicksilver/planning/access/share-fields.md). 

    </div>
-->

* Viste

  * È necessario concedere agli utenti, inclusi gli amministratori di sistema, le autorizzazioni per accedere alle visualizzazioni separatamente dalle relative autorizzazioni per accedere alle aree di lavoro.
  * Quando si condivide una visualizzazione, vengono condivisi tutti gli elementi della visualizzazione, inclusi filtri, raggruppamenti, ordinamento o Impostazioni.
  * Quando si condivide una visualizzazione, i record visibili nella visualizzazione non vengono condivisi. I record devono essere condivisi condividendo le aree di lavoro.
  * È possibile condividere una visualizzazione pubblicamente con persone esterne all&#39;organizzazione quando si genera un collegamento pubblico per una visualizzazione. Gli utenti che accedono alla pagina record da un collegamento pubblico possono visualizzare tutti i record e i relativi campi, inclusi quelli collegati.

  Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).


## Considerazioni sulla condivisione di oggetti in Adobe Workfront Planning

* Il tipo di licenza Adobe Workfront funziona insieme alle autorizzazioni di Workfront Planning per consentire l’accesso alla visualizzazione, al contributo o alla gestione delle aree di lavoro e dei relativi oggetti.

  Per informazioni su come i tipi di licenza influiscono sui livelli di autorizzazione per Workfront Planning, vedere [Panoramica sui tipi di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Gli amministratori di sistema possono gestire tutte le aree di lavoro del sistema, incluse quelle che non hanno creato.
* Gli altri utenti, inclusi gli amministratori di sistema, possono accedere solo alle visualizzazioni create o condivise con loro. Gli amministratori di sistema possono disporre delle autorizzazioni necessarie solo per gestire una visualizzazione.

* Quando si condividono aree di lavoro e tipi di record con altri utenti, il livello di autorizzazione del tipo di record viene ereditato automaticamente dai record e dai campi associati per impostazione predefinita.

* È possibile condividere gli oggetti Planning nei modi seguenti:

  * Internamente, è possibile condividere oggetti di Workfront Planning con le seguenti entità Workfront:

    * Utenti
    * Gruppi
    * Team
    * Aziende
    * Mansioni

    È possibile condividere un oggetto Planning con un massimo di 100 entità per oggetto.

  * Internamente, condividendo un collegamento a un&#39;area di lavoro o a una vista con altri utenti di Planning. Esistono i seguenti scenari:

    * Gli utenti che ricevono il collegamento a un’area di lavoro devono essere utenti attivi e accedere a Workfront per accedere all’area di lavoro.
    * Gli utenti che ricevono un collegamento di condivisione interna per una visualizzazione devono essere utenti attivi e accedere a Workfront per accedere alla visualizzazione.
  * Esternamente, condividendo un collegamento di condivisione pubblica a una visualizzazione con utenti esterni che non dispongono di un account Workfront.

## Condivisione delle autorizzazioni per gli oggetti di Adobe Workfront Planning

Le tabelle delle sezioni seguenti illustrano il livello di autorizzazioni che è possibile selezionare quando si condivide un&#39;area di lavoro o una visualizzazione e le funzionalità consentite da ogni livello.

>[!IMPORTANT]
>
>Non tutti gli utenti possono disporre dei livelli di autorizzazione descritti di seguito. La licenza individuale degli utenti determina il livello di autorizzazioni che possono ricevere per gli oggetti di Workfront Planning.
>
>Solo gli utenti con licenza Standard (o Plan) possono disporre delle autorizzazioni Contribute (Contribuisci) o Manage (Gestisci) per le aree di lavoro e delle autorizzazioni Manage (Gestisci) per le viste.
> 
>Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le aree di lavoro e le visualizzazioni.
>
>Per informazioni, vedere [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Autorizzazioni per le aree di lavoro

È necessario concedere agli utenti le autorizzazioni per le aree di lavoro per consentire loro di accedere alle seguenti entità:

* Aree di lavoro
* Tipi di record
* Record
* Campi

Di seguito sono riportati i livelli di autorizzazione per le aree di lavoro:

|        | Gestione | Contribuisci | Visualizzazione |
|--------|--------|------------|-------|
| Modifica | ✓ |            |       |
| Condividi | ✓ |            |       |
| Elimina | ✓ |            |       |
| Visualizzazione | ✓ | ✓ | ✓ |

<!--
<span class="permissions">In addition to the permissions described in the above table, you can also change the owner of a workspace when sharing it. For information, see [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md).</span>
-->

### Autorizzazioni per i tipi di record

<!--
 old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Le autorizzazioni del tipo di record vengono sempre ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

È possibile rimuovere le autorizzazioni ereditate del tipo di record ricevute dall&#39;area di lavoro.

È possibile assegnare agli utenti autorizzazioni inferiori per il tipo di record rispetto a quelle disponibili nell&#39;area di lavoro.

Tuttavia, non è possibile effettuare le seguenti operazioni:

* Concedere autorizzazioni più elevate per il tipo di record rispetto a quelle disponibili per gli utenti nell&#39;area di lavoro.
* Concedere ai responsabili dell&#39;area di lavoro autorizzazioni inferiori per un tipo di record.
* Rimuovere le autorizzazioni di visualizzazione al tipo di record o all&#39;area di lavoro rimuovendo gli utenti dalle autorizzazioni del tipo di record.

Esistono i seguenti scenari:

| Autorizzazioni Workspace | Autorizzazioni ereditate automaticamente per un tipo di record | Autorizzazioni possibili per il tipo di record quando le autorizzazioni ereditate sono disattivate (concesse manualmente) |
|--------|--------|-------------|
| Gestione | Gestione | Gestisci, Rimuovi autorizzazioni* |
| Contribuisci | Contribuisci | Autorizzazioni Contribute, View, Remove* |
| Visualizzazione | Visualizzazione | Visualizza, Rimuovi autorizzazioni* |

>[!NOTE]
>
>Quando si rimuovono le autorizzazioni da un tipo di record, gli utenti conservano comunque le autorizzazioni di visualizzazione per l&#39;area di lavoro e per tutti i tipi di record, a meno che non si rimuovano le relative autorizzazioni dall&#39;area di lavoro.

### Autorizzazioni per i record

Per impostazione predefinita, le autorizzazioni dei record vengono ereditate dal tipo di record quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

<!--
In the Production environment, the following are the levels of permissions for records: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |     ✓       |       |
| Delete | ✓      |     ✓       |       |
| Edit   | ✓      |    ✓        |       |
| View   | ✓      | ✓          | ✓     |
-->

Di seguito sono riportati i livelli di autorizzazione per i record:

|        | Gestione | Visualizzazione |
|--------|--------|-------|
| Crea | ✓ |       |
| Elimina | ✓ |       |
| Modifica | ✓ |       |
| Visualizzazione | ✓ | ✓ |

Le autorizzazioni dei record vengono sempre ereditate quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

È possibile rimuovere le autorizzazioni ereditate del record ricevute dal tipo di record. I responsabili di Workspace e i creatori di record conservano le autorizzazioni di gestione per il record.

Non è possibile assegnare agli utenti autorizzazioni di livello inferiore o superiore per il record rispetto a quelle disponibili per il tipo di record.

Esistono i seguenti scenari:

| Autorizzazioni per Workspace e il tipo di record | Autorizzazioni ereditate automaticamente per un record | Possibili autorizzazioni di record quando le autorizzazioni ereditate sono disattivate (concesse manualmente) |
|--------|--------|-------------|
| Gestione | Gestione | Gestisci, Rimuovi autorizzazioni* |
| Contribuisci | Gestione | Gestisci, Rimuovi autorizzazioni* |
| Visualizzazione | Visualizzazione | Visualizza, Rimuovi autorizzazioni* |

>[!NOTE]
>
>*Quando si rimuovono le autorizzazioni da un record, gli utenti conservano comunque le autorizzazioni di visualizzazione per l&#39;area di lavoro e il tipo di record, a meno che non si rimuovano le relative autorizzazioni dall&#39;area di lavoro.

### Autorizzazioni per registrare i campi


#### Autorizzazioni per registrare i campi nell’ambiente di produzione


Le autorizzazioni per la modifica delle impostazioni dei campi vengono ereditate dal tipo di record quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

Le autorizzazioni seguenti fanno riferimento alle impostazioni dei campi e non ai valori associati a ciascun campo. Per modificare i valori dei campi è necessario disporre delle autorizzazioni per la modifica dei record.

|        | Gestione | Contribuisci | Visualizzazione |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizzazione | ✓ | ✓ | ✓ |


<div class="preview">

#### Autorizzazioni per registrare i campi nell’ambiente di anteprima

Le autorizzazioni per le impostazioni dei campi vengono ereditate dal tipo di record quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

Le autorizzazioni seguenti fanno riferimento alle impostazioni dei campi e non ai valori associati a ciascun campo.

|        | Gestione | Contribuisci | Visualizzazione |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizzazione | ✓ | ✓ | ✓ |


Le autorizzazioni per i valori dei campi vengono ereditate dal tipo di record e funzionano insieme alle autorizzazioni per i record.

Puoi gestire le autorizzazioni per i valori dei singoli campi e limitare i campi che potrebbero contenere informazioni riservate.

È possibile concedere le seguenti autorizzazioni ai valori dei campi condividendo un campo:

|        | Gestione | Visualizzazione |
|--------|--------|------|
| Elimina | ✓ |      |
| Modifica | ✓ |      |
| Visualizzazione | ✓ | ✓ |

Per accedere ai campi, gli utenti devono disporre almeno delle autorizzazioni di visualizzazione per il tipo di record.

</div>

### Autorizzazioni per le visualizzazioni

È necessario concedere autorizzazioni separate alle visualizzazioni record. La concessione delle autorizzazioni all&#39;area di lavoro non consente di concedere le autorizzazioni alle visualizzazioni record nell&#39;area di lavoro.

È necessario concedere agli utenti le autorizzazioni per le visualizzazioni per consentire loro di accedere ai seguenti elementi di visualizzazione:

* Filtri
* Visibilità del campo
* Ordina
* Raggruppamento
* Altezza riga
* Impostazioni

È possibile condividere le visualizzazioni internamente o pubblicamente.

Di seguito sono riportati i livelli di autorizzazione per le visualizzazioni e gli elementi di visualizzazione:

| Condivisione interna | Gestisci (solo le persone invitate possono accedere) | Visualizza (solo le persone invitate possono accedere) | Tutti nell&#39;area di lavoro possono visualizzare* |
|--------|--------|-------|------------------------------|
| Modifica | ✓ |       |                            |
| Elimina | ✓ |       |                            |
| Condividi | ✓ |       |                           |
| Visualizzazione | ✓ | ✓ | ✓ |
| Applica | ✓ | ✓ | ✓ |

| Condivisione pubblica | Visualizzazione |
|--------|-------|
| Visualizzazione | ✓ |
| Applica | ✓ |

>[!NOTE]
>
>*Gli utenti devono disporre di autorizzazioni View (Visualizzazione) o superiori per un&#39;area di lavoro per poter accedere a questa visualizzazione.


<!--
old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->

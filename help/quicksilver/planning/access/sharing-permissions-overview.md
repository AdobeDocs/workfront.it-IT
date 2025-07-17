---
title: Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning
description: Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. In questo articolo vengono descritte le informazioni generali sulla condivisione o la rimozione delle autorizzazioni per un'area di lavoro o una visualizzazione di Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

È possibile condividere o rimuovere le autorizzazioni per un&#39;area di lavoro, un tipo di record o una visualizzazione di Adobe Workfront Planning.

È inoltre possibile condividere i moduli di richiesta di Planning. Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

In questo articolo vengono descritti i livelli di autorizzazione per le aree di lavoro di Workfront Planning, i tipi di record, i record, i campi e le visualizzazioni.

## Oggetti condivisibili in Adobe Workfront Planning

È possibile condividere manualmente alcuni oggetti di Workfront Planning, mentre altri oggetti ereditano tali autorizzazioni da altri oggetti.

In Workfront Planning è possibile condividere manualmente i seguenti oggetti:

* Aree di lavoro

   * È possibile condividere le aree di lavoro con altri utenti all&#39;interno dell&#39;organizzazione.
   * Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro.
   * Quando si condivide un&#39;area di lavoro, le visualizzazioni non vengono condivise. Le visualizzazioni sono condivise separatamente.

  Per ulteriori informazioni, vedere [Condividi aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

* Tipi di record

   * È possibile condividere i tipi di record con persone all&#39;interno dell&#39;organizzazione.
   * Il livello di autorizzazioni concesse per l&#39;area di lavoro viene visualizzato come Autorizzazioni ereditate per il tipo di record.
   * Non è possibile condividere un tipo di record con un livello di autorizzazione superiore a quello dell&#39;utente nell&#39;area di lavoro.

  Per ulteriori informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).


* Viste

   * È necessario concedere agli utenti, inclusi gli amministratori di sistema, le autorizzazioni per accedere alle visualizzazioni separatamente dalle relative autorizzazioni per accedere alle aree di lavoro.
   * Quando si condivide una visualizzazione, vengono condivisi tutti gli elementi della visualizzazione, inclusi filtri, raggruppamenti, ordinamento o Impostazioni.
   * Quando si condivide una visualizzazione, i record visibili nella visualizzazione non vengono condivisi. I record devono essere condivisi condividendo le aree di lavoro.
   * È possibile condividere una visualizzazione pubblicamente con utenti esterni all&#39;organizzazione quando si genera un collegamento pubblico per una visualizzazione.Gli utenti che accedono alla pagina record da un collegamento pubblico possono visualizzare tutti i record e i relativi campi, inclusi i record e i campi collegati.

  Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

Internamente, è possibile condividere un&#39;area di lavoro, una vista o un tipo di record con le seguenti entità Workfront:

* Utenti
* Gruppi
* Team
* Aziende
* Mansioni

Quando si condividono aree di lavoro e tipi di record con altri utenti, il livello di autorizzazione del tipo di record viene ereditato automaticamente dai record e dai campi ad essi associati.

>[!IMPORTANT]
>
>Se l’istanza di Workfront della tua organizzazione è stata integrata nell’esperienza unificata di Adobe, gli utenti con cui desideri condividere gli oggetti di Planning devono essere aggiunti al Adobe Admin Console. Non è possibile condividere oggetti Planning con utenti di Workfront che non sono stati aggiunti al Adobe Admin Console.


## Considerazioni sulla condivisione di oggetti in Adobe Workfront Planning

* Il tipo di licenza Adobe Workfront funziona insieme alle autorizzazioni di Workfront Planning per consentire l’accesso alla visualizzazione, al contributo o alla gestione delle aree di lavoro e dei relativi oggetti.

  Per informazioni su come i tipi di licenza influiscono sui livelli di autorizzazione per Workfront Planning, vedere [Panoramica sui tipi di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Gli amministratori di sistema possono gestire tutte le aree di lavoro del sistema, incluse quelle che non hanno creato.
* Gli altri utenti, inclusi gli amministratori di sistema, possono accedere solo alle visualizzazioni create o condivise con loro. Gli amministratori di sistema possono disporre delle autorizzazioni necessarie solo per gestire una visualizzazione.
* È possibile condividere con altri utenti un collegamento a un&#39;area di lavoro o a una visualizzazione.

  Esistono i seguenti scenari:
   * Gli utenti che ricevono il collegamento a un’area di lavoro devono essere utenti attivi e accedere a Workfront per poter accedere all’area di lavoro.
   * Gli utenti che ricevono il collegamento a una visualizzazione possono accedervi nei modi seguenti:

      * Se il collegamento alla visualizzazione è stato condiviso internamente, deve trattarsi di utenti attivi e accedere a Workfront.
      * Possono essere utenti esterni di Workfront e accedere alla visualizzazione da un collegamento condiviso pubblicamente, senza effettuare l’accesso a Workfront.

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

|        | Gestisci | Contribuisci | Viste |
|--------|--------|------------|-------|
| Modif | ✓ |            |       |
| Condividi | ✓ |            |       |
| Elimina | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni per i tipi di record

<!-- old access:
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
| Gestisci | Gestisci | Gestisci, Rimuovi autorizzazioni* |
| Contribuisci | Contribuisci | Autorizzazioni Contribute, View, Remove* |
| Visualizza | Visualizza | Visualizza, Rimuovi autorizzazioni* |

>[!NOTE]
>
>*Quando si rimuovono le autorizzazioni da un tipo di record, gli utenti conservano comunque le autorizzazioni di visualizzazione per l&#39;area di lavoro e per tutti i tipi di record, a meno che non si rimuovano le relative autorizzazioni dall&#39;area di lavoro.

### Autorizzazioni per i record

Le autorizzazioni dei record vengono ereditate dal tipo di record quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

Di seguito sono riportati i livelli di autorizzazione per i record:


|        | Gestisci | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ | ✓ |       |
| Elimina | ✓ | ✓ |       |
| Modifica | ✓ | ✓ |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni per registrare i campi

Le autorizzazioni dei campi vengono ereditate dal tipo di record quando si concedono le autorizzazioni all&#39;area di lavoro e al tipo di record.

Le autorizzazioni seguenti fanno riferimento ai campi stessi e non ai valori associati a ciascun campo. Per modificare i valori dei campi è necessario disporre delle autorizzazioni per la modifica dei record.

|        | Gestisci | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |


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
| Visualizza | ✓ | ✓ | ✓ |
| Applica | ✓ | ✓ | ✓ |

| Condivisione pubblica | Visualizza |
|--------|-------|
| Visualizza | ✓ |
| Applica | ✓ |

*Gli utenti devono disporre di autorizzazioni View (Visualizzazione) o superiori per un&#39;area di lavoro per poter accedere a questa visualizzazione.

<!--old view permissions, before sharing View permissions to a view through a workspace:
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

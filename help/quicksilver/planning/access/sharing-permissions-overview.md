---
title: Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning
description: Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. In questo articolo vengono descritte le informazioni generali sulla condivisione o la rimozione delle autorizzazioni per un'area di lavoro o una visualizzazione di Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 6%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning

{{planning-important-intro}}

È possibile condividere o rimuovere le autorizzazioni per un&#39;area di lavoro o una vista di Adobe Workfront Planning.

Questo articolo descrive i livelli di autorizzazione per gli oggetti di Workfront Planning.

Per informazioni su come condividere aree di lavoro o visualizzazioni, vedere i seguenti articoli:

* [Condividere le aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

* [Condividere le visualizzazioni](/help/quicksilver/planning/access/share-views.md)

## Oggetti condivisibili in Adobe Workfront Planning

È possibile condividere i seguenti oggetti:

* Aree di lavoro

   * È possibile condividere le aree di lavoro con altri utenti all&#39;interno dell&#39;organizzazione.
   * Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro.
   * Quando si condivide un&#39;area di lavoro, le visualizzazioni non vengono condivise. Le visualizzazioni sono condivise separatamente.

* Viste

   * È necessario concedere agli utenti, inclusi gli amministratori di sistema, le autorizzazioni per accedere alle visualizzazioni separatamente dalle relative autorizzazioni per accedere alle aree di lavoro.
   * Quando si condivide una visualizzazione, vengono condivisi tutti gli elementi della visualizzazione, inclusi filtri, raggruppamenti, ordinamento o Impostazioni.
   * Quando si condivide una visualizzazione, i record visibili nella visualizzazione non vengono condivisi. I record devono essere condivisi condividendo le aree di lavoro.
   * È possibile condividere una visualizzazione pubblicamente con utenti esterni all&#39;organizzazione quando si genera un collegamento pubblico per una visualizzazione.Gli utenti che accedono alla pagina record da un collegamento pubblico possono visualizzare tutti i record e i relativi campi, inclusi i record e i campi collegati.

  Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

Internamente, potete condividere un&#39;area di lavoro o una vista con le seguenti entità Workfront:

* Utenti
* Gruppi

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
| Crea | ✓ | ✓ |       |
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
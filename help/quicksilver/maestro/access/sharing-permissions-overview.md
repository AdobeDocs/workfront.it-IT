---
title: Panoramica delle autorizzazioni di condivisione nella pianificazione di Adobe Workfront
description: È possibile condividere o rimuovere le autorizzazioni per un'area di lavoro o una visualizzazione di Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront planning. This article describes the levels of access that users could have to Adobe Workfront planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Panoramica delle autorizzazioni di condivisione nella pianificazione di Adobe Workfront

{{maestro-important-intro}}

È possibile condividere o rimuovere le autorizzazioni per un&#39;area di lavoro o una visualizzazione in Adobe Workfront Planning.

In questo articolo vengono descritti i livelli di autorizzazione per gli oggetti di pianificazione di Workfront.

Per informazioni su come condividere aree di lavoro o visualizzazioni, vedere i seguenti articoli:

* [Condividere le aree di lavoro](/help/quicksilver/maestro/access/share-workspaces.md)

* [Condividere le visualizzazioni](/help/quicksilver/maestro/access/share-views.md)

## Oggetti condivisibili nella pianificazione di Adobe Workfront

È possibile condividere i seguenti oggetti:

* Aree di lavoro

  Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro. Le visualizzazioni non sono condivise.

* Viste

## Considerazioni sulla condivisione di oggetti nella pianificazione di Adobe Workfront

* Il tipo di licenza Adobe Workfront funziona in combinazione con le autorizzazioni di pianificazione di Workfront per consentire l’accesso alla visualizzazione, al contributo o alla gestione degli oggetti quando si utilizza la pianificazione di Workfront.

  Per informazioni sull&#39;effetto dei tipi di licenza sui livelli di autorizzazione per la pianificazione di Workfront, vedere [Panoramica del tipo di licenza quando si utilizza la pianificazione di Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).
* Gli amministratori di sistema possono gestire e condividere le aree di lavoro create da altri utenti.
* Se non sei un amministratore di sistema, puoi contribuire alle aree di lavoro create da altri utenti se sono condivise con te.
* Non è possibile condividere le aree di lavoro in blocco.
* Potete condividere un workspace o una vista con le seguenti entità:
   * Utenti
   * Gruppi
* Gli altri utenti, inclusi gli amministratori di sistema, possono accedere solo alle visualizzazioni create o condivise con loro. Agli amministratori di sistema possono essere assegnate solo le autorizzazioni per gestire una visualizzazione.
* È possibile condividere con altri utenti un collegamento a un&#39;area di lavoro o a una visualizzazione da una pagina del tipo di record. Per poter accedere all&#39;area di lavoro o alla pagina del tipo di record visualizzata nella vista selezionata, gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront.

## Condivisione delle autorizzazioni per gli oggetti di pianificazione di Adobe Workfront

Le tabelle delle sezioni seguenti illustrano il livello di autorizzazioni che è possibile selezionare quando si condivide un&#39;area di lavoro o una visualizzazione e le funzionalità consentite da ogni livello.

>[!IMPORTANT]
>
>Non tutti gli utenti possono disporre dei livelli di autorizzazione descritti di seguito. La licenza individuale degli utenti determina il livello di autorizzazioni che possono ricevere per gli oggetti di pianificazione di Workfront.
>
>Per informazioni, consulta [Panoramica del tipo di licenza quando si utilizza la pianificazione di Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


### Autorizzazioni di Workspace

|        | Gestire | Contribuisci | Viste |
|--------|--------|------------|-------|
| Modif | ✓ |            |       |
| Condividi | ✓ |            |       |
| Elimina | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni del tipo di record

Le autorizzazioni del tipo di record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

|        | Gestire | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni record

Le autorizzazioni dei record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

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

|        | Gestire | Viste |
|--------|--------|-------|
| Modif | ✓ |       |
| Elimina | ✓ |       |
| Visualizza | ✓ | ✓ |
| Applica | ✓ | ✓ |

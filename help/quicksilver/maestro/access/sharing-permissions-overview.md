---
title: Panoramica delle autorizzazioni di condivisione in Adobe Maestro
description: Puoi condividere o rimuovere le autorizzazioni per un’area di lavoro o una visualizzazione Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 72d044541f8e061c51c4483672a89ce20e4f30d9
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Panoramica delle autorizzazioni di condivisione in Adobe Maestro

{{maestro-important-intro}}

Puoi condividere o rimuovere le autorizzazioni per un’area di lavoro o una visualizzazione Adobe Maestro.

Questo articolo descrive i livelli di autorizzazione per gli oggetti Maestro.

Per informazioni su come condividere aree di lavoro o visualizzazioni, vedere i seguenti articoli:

* [Condividere le aree di lavoro](/help/quicksilver/maestro/access/share-workspaces.md)

* [Condividere le visualizzazioni](/help/quicksilver/maestro/access/share-views.md)

## Oggetti che puoi condividere in Adobe Maestro

In Maestro puoi condividere i seguenti oggetti:

* Aree di lavoro

  Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro. Le visualizzazioni non sono condivise.

* Viste

## Considerazioni sulla condivisione di oggetti in Maestro

* Per creare aree di lavoro in Maestro è necessario disporre della seguente licenza:

   * Nuovo modello di prezzo: Licenza standard
   * Modello di determinazione prezzi corrente: licenza Pianificazione.

  Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Gli amministratori di sistema possono gestire e condividere le aree di lavoro create da altri utenti.
* Se non sei un amministratore di sistema, puoi contribuire alle aree di lavoro create da altri utenti se sono condivise con te.
* Non è possibile condividere le aree di lavoro in blocco.
* Potete condividere un&#39;area di lavoro con le seguenti entità:
   * Utenti
   * Gruppi
* Gli altri utenti, inclusi gli amministratori di sistema, possono accedere solo alle visualizzazioni create o condivise con loro.
* È possibile condividere con altri utenti un collegamento a un&#39;area di lavoro o una visualizzazione da una pagina di tipo record. Per poter accedere all&#39;area di lavoro o alla pagina del tipo di record visualizzata nella vista selezionata, gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront.

## Condivisione delle autorizzazioni per gli oggetti Maestro

Le tabelle delle sezioni seguenti illustrano il livello di autorizzazioni che è possibile selezionare quando si condivide un&#39;area di lavoro o una visualizzazione Maestro e le funzionalità consentite da ogni livello.

### Autorizzazioni di Workspace

|        | Gestisci | Contribuisci | Viste |
|--------|--------|------------|-------|
| Modif | ✓ |            |       |
| Condividi | ✓ |            |       |
| Elimina | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni del tipo di record

Le autorizzazioni del tipo di record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

|        | Gestisci | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni record

Le autorizzazioni dei record vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.

|        | Gestisci | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ | ✓ |       |
| Modifica | ✓ | ✓ |       |
| Visualizza | ✓ | ✓ | ✓ |

### Autorizzazioni campo

Le autorizzazioni per i campi vengono ereditate quando si concedono le autorizzazioni all&#39;area di lavoro.
Le autorizzazioni seguenti fanno riferimento ai campi stessi e non ai valori associati a ciascun campo. Per modificare i valori dei campi è necessario disporre delle autorizzazioni per la modifica dei record.

|        | Gestisci | Contribuisci | Visualizza |
|--------|--------|------------|-------|
| Crea | ✓ |            |       |
| Elimina | ✓ |            |       |
| Modifica | ✓ |            |       |
| Visualizza | ✓ | ✓ | ✓ |


### Visualizza autorizzazioni

È necessario concedere autorizzazioni separate alle visualizzazioni record. La concessione delle autorizzazioni all&#39;area di lavoro non consente di concedere le autorizzazioni alle visualizzazioni record nell&#39;area di lavoro.

|        | Gestisci | Viste |
|--------|--------|-------|
| Modif | ✓ |       |
| Elimina | ✓ |       |
| Visualizza | ✓ | ✓ |
| Applica | ✓ | ✓ |







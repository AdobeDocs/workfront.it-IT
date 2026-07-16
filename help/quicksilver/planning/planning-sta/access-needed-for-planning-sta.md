---
title: Accesso necessario per Adobe Workfront Planning as a prodotto standalone
description: Questo articolo descrive le licenze, i livelli di accesso e le funzionalità utente per Adobe Workfront Planning come prodotto standalone.
last-update: 2026-04-01T18:02:40Z
git-commit-file: 8cc175490a6aa1db68b238edbdf9da9da7fbb258
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 2%

---

<!--

Update metadata with this at release:
---
title: Access Required for Planning Standalone
description: This article describes how you can benefit from using the standalone version of Adobe Workfront Planning.
feature: Workfront Planning (******************ask Bob for a new feature???***********)
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

# Accesso necessario per Adobe Workfront Planning come prodotto standalone

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning, se acquistato come prodotto standalone. Fare riferimento a questo articolo quando la società ha acquistato un pacchetto solo Adobe Workfront Planning e non ha acquistato un pacchetto flusso di lavoro Workfront.
>
>Per informazioni su Adobe Workfront Planning quando viene acquistato insieme a un pacchetto di Workfront Workflow, vedere [Introduzione a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Questo articolo descrive le licenze, i livelli di accesso e le funzionalità utente per Adobe Workfront Planning come prodotto standalone.

## Pacchetti Workfront Planning

L&#39;organizzazione può acquistare uno dei seguenti pacchetti Workfront Planning autonomi:

* Prime
* Seleziona
* Ultimate

La tabella seguente descrive gli elementi inclusi in ciascun pacchetto:

| Capacità di pianificazione | Seleziona | Prime | Ultimate |
|---|---|---|---|
| Pianificazione, orchestrazione, gestione delle campagne | ✓ | ✓ | ✓ |
| Aree di lavoro illimitate | ✓ | ✓ | ✓ |
| Record per area di lavoro | 25,000 | 500,000 | 1,000,000 |
| Record totali (tutte le aree di lavoro) | 500,000 | 2,000,000 | Senza limiti |
| Tipi di record globali e connessioni tra aree di lavoro diverse | — | ✓ | ✓ |
| Accesso alle funzioni future al momento del rilascio | Alcuni | Alcuni | Più |

## Disponibilità del pacchetto Workfront Planning

<!--
the bullets repeat in the "Planning overview" article
-->

Workfront Planning è accessibile quando l&#39;organizzazione acquista uno dei seguenti pacchetti Workfront:

* Workfront Workflow e Workfront Planning acquistati insieme. Ogni utente dell’organizzazione dispone di un flusso di lavoro e di una licenza Planning. In questo modo tutti gli utenti hanno pieno accesso a tutte le funzioni di Workfront per entrambi i moduli.

* Flusso di lavoro di Workfront per tutti gli utenti dell&#39;organizzazione e pianificazione di Workfront solo per alcuni utenti dell&#39;organizzazione. In questo modo gli utenti avranno pieno accesso a tutte le funzioni di Workflow e avranno un accesso più limitato alle funzioni di Planning per gli utenti ai quali è stata assegnata una licenza Planning.

* Workfront Planning come prodotto autonomo per gli utenti dell&#39;organizzazione. In questo modo gli utenti non potranno accedere alle funzioni di Workfront Workflow né alle funzioni di Planning.

Per informazioni sulle funzionalità incluse in Planning come prodotto standalone, vedere la sezione &quot;Funzionalità incluse in Workfront Planning come prodotto standalone&quot; nell&#39;articolo [Introduzione ad Adobe Workfront Planning come prodotto standalone](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

## Licenza utente e livelli di accesso

<!-- should this be moved to the Manage users in Planning article??-->

Le licenze Planning fanno parte del livello di accesso assegnato agli utenti.

Per Planning come prodotto standalone, non è possibile assegnare licenze ai livelli di accesso, in quanto sono già codificate per essere incluse nei livelli di accesso assegnati agli utenti.

A seconda della combinazione di pacchetti Workfront Planning acquistata dall&#39;organizzazione, è possibile che si disponga di uno dei seguenti livelli di accesso per gli utenti:

* **Amministratore Planning**: disponibile per i pacchetti Workfront Planning. Gli amministratori di Planning vengono assegnati automaticamente quando gli utenti vengono aggiunti a Admin Console.
* **Planning Standard**: disponibile per tutti i pacchetti Workfront Planning. Puoi assegnare questi livelli di accesso agli utenti quando li crei.

<!--
this is not available for Planning STA: 
* **Planning Contributor**: Available for the following customers: 

    * Customers that purchase equal amounts of Workflow and Planning packages together. In this case, Planning Contributors have limited access to Planning objects.
    * Customer that purchase unequal amounts of Workflow and Planning packages. In this case, Planning Contributors have read-only access to Planning objects.

-->

Ogni licenza Planning indipendente è associata a un ruolo nel sistema e controlla quali aree del prodotto sono accessibili.

Nella tabella seguente vengono illustrati i tipi di licenza di Planning e le relative funzionalità in Workfront Planning, se acquistati come prodotto standalone:

| Funzionalità/tipo di licenza | Amministratore pianificazione | Standard di pianificazione |
|---|---|---|
| Descrizione del livello di accesso | Accesso completo al sistema | Può gestire aree di lavoro e contenuti |
| Area Pianificazione nel menu principale | ✔ | ✔ |
| Area Utenti nel menu principale | ✔ | Solo visualizzazione |
| Area Richieste nel menu principale | ✔ | ✔ |
| Area di configurazione nel menu principale | ✔ |   |
| Gestire le aree di lavoro e il relativo contenuto | ✔ | ✔ |
| Condividere i dati di Planning con i team | ✔ | ✔ |
| Inviano richieste | ✔ | ✔ |
| Creare o modificare utenti | ✔ |   |
| Visualizza elenco utenti | ✔ | Solo visualizzazione |
| Configurazione > Team | ✔ |   |
| Configurazione > Accedi come | ✔ |   |
| Configurazione > Trimestri personalizzati | ✔ |   |
| Configurazione > Sistema > Informazioni cliente | ✔ |   |
| Configurazione > Sistema > Preferenze | ✔ |   |

Per informazioni sull&#39;assegnazione dei livelli di accesso agli utenti, vedere [Gestire gli utenti in Adobe Workfront Planning come prodotto standalone](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md).

## Aree di navigazione e dipendenze dei livelli di accesso

A seconda della licenza Planning, gli utenti possono avere diverse aree disponibili nella navigazione globale.

<!--
>[!NOTE]
>
>Workfront-specific toolbar actions (Search, Recents, Favorites, Notifications) are not available in the Workfront header for any Standalone user.
-->

### Panoramica sulla navigazione dell&#39;amministratore di Planning

<!--
Managing your Adobe Workfront Planning instance is similar to managing an Adobe Workfront with Planning instance, but there are some differences.
-->

Un utente con un livello di accesso Amministratore di Planning dispone delle seguenti funzionalità:

* Dispone dell&#39;accesso completo al sistema.
* Può creare e modificare utenti, gestire team, configurare trimestri personalizzati e accedere a tutte le sottopagine Configurazione.

  Per informazioni, consulta:

   * [Gestione degli utenti in Adobe Workfront Planning come prodotto standalone](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)
   * [Gestione dei team in Adobe Workfront Planning come prodotto standalone](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)
* Può inviare e gestire le richieste.

  Per informazioni, vedere [Richieste Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/requests/requests-article-index.md).
* Include le seguenti aree nel menu principale:

   * **Planning**: dispone di funzionalità complete per gli oggetti Planning, per crearli, eliminarli, condividerli e connetterli.
   * **Utenti**: puoi aggiungere utenti e modificarne i profili.
   * **Richieste**
   * **Configura**
* Contiene le seguenti sezioni nell’area Configurazione:

   * **Team**: è possibile aggiungere, rimuovere o modificare i team. La modifica è limitata al nome del team, alla descrizione e ai membri. Non sono disponibili controlli di filtro, visualizzazione, raggruppamento o esportazione.
   * **Accedi come**: rappresenta un altro utente a scopo di risoluzione dei problemi.
   * **Trimestri personalizzati**: configurare i trimestri fiscali personalizzati visualizzati nelle visualizzazioni della sequenza temporale di Planning.
   * Sistema

* Include le seguenti sezioni nell’area Sistema:

   * **Informazioni cliente**: visualizza dettagli cliente e organizzazione.
   * **Preferenze**: rivedi e configura le preferenze a livello di sistema.

### Panoramica sulla navigazione di Planning Standard

Un utente con un livello di accesso Planning Standard dispone delle seguenti funzionalità:

* Può gestire le aree di lavoro e il relativo contenuto.
* Può inviare e gestire le richieste.

  Per informazioni, vedere [Richieste Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/requests/requests-article-index.md).
* Gli utenti di Planning Standard possono accedere alle seguenti aree nel menu Principale:

   * **Pianificazione**
   * **Utenti**: dispongono dell&#39;accesso in sola visualizzazione agli utenti. Non possono creare o modificare utenti. <!--not sure if this is still true-->
   * **Richieste**

* Non hanno accesso a Configurazione o a nessuna delle sue sezioni.

## Configurare i livelli di accesso per Planning come prodotto standalone

I livelli di accesso sono incorporati quando si acquista Planning come prodotto standalone e non è possibile configurarli per gli utenti di Planning.

Per assegnare i livelli di accesso agli utenti, come amministratore di Planning:

* Crea utenti nella console Adobe.

  Esistono i seguenti scenari:

   * Gli utenti aggiunti alla console Adobe come amministratori ricevono un livello di accesso Amministratore di Planning in Workfront Planning.
   * Agli utenti aggiunti alla console Adobe in qualità di utenti può essere assegnato un livello di accesso Planning Standard in Workfront Planning. Questo è l&#39;unico accesso disponibile per l&#39;assegnazione ai nuovi utenti in Workfront Planning come prodotto standalone.

Per ulteriori informazioni, vedere [Gestione utenti](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md).

## Concedere le autorizzazioni in Workfront Planning come prodotto standalone

In Workfront Planning è possibile condividere i seguenti oggetti come prodotto autonomo:

* Aree di lavoro
* Tipi di record
* Record
* Viste

La condivisione di oggetti in Planning come prodotto standalone è identica alla condivisione in Planning quando vengono acquistati insieme a un pacchetto Workflow.

Per ulteriori informazioni, vedere [Informazioni di accesso ad Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/access/access-information.md).

<!--

I took this out because there is NO Contributor for true STA: 

### Planning Contributor user experience

>[!IMPORTANT]
>
>Planning Contributor access level is only available for customers that purchase both Workfront Planning and a Workfront Workflow package together. 
>
>If they purchase unequal numbers of packages for the two modules, the Planning Contributor license is read-only. 

When standalone Workfront Planning users purchase a Workflow package, they receive a read-only Planning Contributor license by default. 

For more information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

A user with a Planning Standard access level has the following capabilities: 

* View-only access to Planning data, equivalent to the Contributor license in Workfront.
* Can access the following areas in the Main menu:
    * **Planning**
    * **Requests**
* Can submit requests.
* No access to the Users list.
* No access to Setup or any of its sub-pages.

-->

<!-- 
this was moved from the STA general article - some information is already above - take out here what is not needed or add above: 

## Package overview

The following packages are available for Workfront Planning as a standalone product:

* Select
* Prime
* Ultimate

The following table describes what is included in each package:  

| Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Licensing overview

Consider the following about Workfront Planning licenses:

* Your organization can purchase Workfront Planning licenses without requiring Workfront or Workflow licenses.
* You can add users to Workfront Planning using the Adobe Experience Platform.

    For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 
* Workfront Planning users are limited to Planning-only capabilities and do not receive access to any Workfront areas or capabilities.

The following access levels are hard-coded in Workfront Planning and cannot be modified: 

* Planning Administrator
* Planning Standard 

>[!IMPORTANT]
>
>In a Workfront Planning context, a user must hold a **Planning Standard** license to access the product. 

For more information, see [Access needed for Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md). 

## How licensing works for customers with a Planning and Workfront combined package

Consider the following if you have both the Workfront Workflow and Planning packages:

* A Planning Contributor read-only license is available for users in Planning. 
* Any Workfront access level (including Light or Contributor) can be paired with either a Planning Standard or Planning Contributor access level, regardless of the Workfront Workflow license type.

    For example, a user with a Workfront Contributor license can still hold a Planning Standard license and have full Planning management capabilities.

### Mixed License access matrix

When a customer has both Planning and Workfront packages, access levels are determined by the combination below:

| Access Type | Planning License | Workflow License | License Origin |
|---|---|---|---|
| Default | Read Only | Workfront Light | Workfront |
| Default | Read Only | Workfront Standard | Workfront |
| Default | Read Only | Workfront Contributor | Workfront |
| Default | Read Only | Workfront External | Workfront |
| Default | Planning Standard | Workfront Contributor | Planning |
| — | Planning Standard | Workfront Light | Either Planning or Workfront |
| — | Planning Standard | Workfront Standard | Either Planning or Workfront |

Consider the following if your organization has purchased Workfront with Planning:

* Adding a new user to Planning or Workfront automatically creates default (read-only) access in the other product.
* You can upgrade the access in the opposite product. For more information, contact your account representative.

### Upgrading from standalone Planning to a Planning with a Workflow package

#### Workfront Planning with a Workfront Workflow package

When you add a Workfront Planning Standalone package to an existing Workflow license, the following changes take effect automatically:

* Planning Administrators are promoted to System Administrators.
* Non-admin Planning users (Standard and Contributor) receive Workflow Contributor licenses.
* All existing Planning data is preserved.
* All newly provisioned Workfront users are auto-assigned Planning Contributor (read-only) licenses.

#### License mapping when you upgrade to a Planning with Workflow package

| Before (Planning Standalone) | After (Workfront + Planning) |
|---|---|
| Planning Administrator | System Administrator |
| Planning Standard | Workflow Contributor |
| Planning Contributor | Workflow Contributor |

Planning and Workflow licenses remain separate after the upgrade. A Planning Standard user can hold a Workflow Contributor license, and a Planning Contributor user can hold a Workflow Standard license — these are assigned independently based on need.

All users receive an email notification when they gain access to the additional Workflow capabilities in Workfront.

-->

<!--
I took out the last column on this table and added above:

| Feature / Access | Planning Administrator | Planning Standard | Planning Contributor |
|---|---|---|---|
| Access level description | Full system access | Can manage workspaces and content | View-only access to Planning data when Planning packages are in unequal numbers to Workflow licenses. This license is not available for Planning as a standalone product.|
| Planning area in the Main Menu | ✔ | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |   |
| Requests area in the Main Menu | ✔ | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |   |
| Manage Workspaces and their content | ✔ | ✔ |   |
| Submit requests | ✔ | ✔ | ✔ |
| Create or edit users | ✔ |   |   |
| View users list | ✔ | View only |   |
| Setup > Teams | ✔ |   |   |
| Setup > Log In As | ✔ |   |   |
| Setup > Custom Quarters | ✔ |   |   |
| Setup > System > Customer info | ✔ |   |   |
| Setup > System > Preferences | ✔ |   |   |

-->

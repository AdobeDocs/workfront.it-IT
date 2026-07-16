---
title: Panoramica Del Tipo Di Licenza Quando Si Utilizza Adobe Workfront Planning
description: L’accesso a Adobe Workfront Planning dipende dal tipo di licenza, oltre che dalle autorizzazioni per gli oggetti. Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. In questo articolo vengono descritti i livelli di accesso che gli utenti potrebbero avere a Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/2V2i9ZZOyQ6gShXK-QUKDeCZCxcrbYwb8-mn-9kQbc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: ab0d036ea3bbcdad2daaed6b09864272fd1beb11
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 1%

---

# Panoramica del tipo di licenza durante l’utilizzo di Pianficazione di Adobe Workfront

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

<!--{{planning-important-intro}}-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning. Workfront Planning è un prodotto standalone o una funzionalità acquistata in più da Adobe Workfront.
>
>
>Questo articolo contiene informazioni generali su Workfront Planning quando i clienti acquistano anche un pacchetto Workfront o Workflow.
>
>Per l&#39;elenco completo degli articoli che contengono la documentazione per Workfront Planning, vedere [Informazioni generali e indice degli articoli per Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Per informazioni su Workfront Planning come prodotto autonomo, vedere [Introduzione ad Adobe Workfront Planning come prodotto autonomo](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Il tipo di licenza di Adobe Workfront Workflow funziona in combinazione con il tipo di licenza di Adobe Workfront Planning e con le autorizzazioni di Planning per concedere il seguente accesso:

* Visualizzare, contribuire o gestire aree di lavoro, tipi di record e record.
* Visualizzare o gestire le visualizzazioni.

Per informazioni sulle autorizzazioni per gli oggetti in Workfront Planning, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Per informazioni sull&#39;accesso a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Relazione tra i tipi di licenze Workflow e Planning

I livelli di accesso degli utenti possono essere associati ai seguenti tipi di licenza:

* Tipo di licenza del flusso di lavoro
* Tipo di licenza pianificazione

Per informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Il tipo di licenze Planning disponibili per assegnare gli utenti varia a seconda del pacchetto Workfront acquistato dall&#39;organizzazione.

<!--

This list also exists here: \help\quicksilver\planning\planning-sta\planning-sta-overview.md
-->

La tua organizzazione può acquistare Workfront Planning in diversi modi:

* Insieme a un pacchetto Workfront Workflow, con lo stesso numero di licenze per Workflow e Planning. Gli utenti possono accedere a tutte le funzionalità di Adobe Workfront Workflow e Planning.
* Insieme a un pacchetto Workfront Workflow, con un numero diverso di licenze per Workflow e Planning. Gli utenti possono accedere a tutte le funzionalità di Adobe Workfront Workflow e a un accesso limitato a Workfront Planning.
* Workfront Planning da solo, come prodotto autonomo. Gli utenti non ricevono l&#39;accesso alle funzioni di Workfront Workflow e hanno accesso completo alle funzionalità di Workfront Planning. Per informazioni, vedere [Introduzione ad Adobe Workfront Planning come prodotto autonomo](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

La tabella seguente descrive la relazione tra il flusso di lavoro e i tipi di licenza Planning e le funzionalità degli utenti basate su queste licenze:

| Pacchetto Workfront | Tipi di licenze Planning | Tipi di licenze flusso di lavoro | Funzionalità di gestione licenze |
|---|---|---|---|
| Pianificazione e flusso di lavoro: numero di licenze uguale | Standard, Collaboratore, Nessun accesso | Standard, Light, Collaboratore | - I tipi di licenza di Planning e Workflow sono impostazioni separate nei livelli di accesso<br>- Il tipo di licenza di Planning consente le opzioni Standard, Collaboratore e Vuoto<br>- Il tipo di licenza di Planning può essere lasciato vuoto in qualsiasi livello di accesso - gli utenti con questo livello di accesso non hanno accesso a Planning<br>- Il tipo di licenza del flusso di lavoro non può essere lasciato vuoto<br>- La combinazione di Planning Standard con la licenza di Workflow Contributor non è consentita<br>- Planning Standard può essere selezionato solo con le licenze Workflow Light e Standard |
| Pianificazione e flusso di lavoro - Numero di licenze non uniforme | Standard, nessun accesso | Standard, Light, Collaboratore | - I tipi di licenza di Planning e Workflow sono impostazioni separate nei livelli di accesso<br>- Il tipo di licenza di Planning consente solo le opzioni Standard o Nessun accesso<br> - Planning Standard può essere selezionato con qualsiasi tipo di licenza Workflow<br> - Il tipo di licenza di Planning può essere Nessuno - Gli utenti con questo livello di accesso non potranno accedere ai dati di Planning in alcun modo<br>- Il tipo di licenza del flusso di lavoro non può essere lasciato vuoto in alcun livello di accesso<br>- Gli utenti con la licenza di Planning Contributor possono visualizzare gli oggetti del flusso di lavoro connessi in Planning, ma non possono connettersi o disconnettersi |

Per ulteriori informazioni sulle licenze in Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

<!--
not sure if we need this anymore, this is before STA launched:

| Adobe Workfront license type                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | <p>Users can manage workspaces, record types, records, and views. They can create, edit, or delete workspaces, record types, records, fields, and views.</p><br><p>System administrators have Manage permissions to all workspaces, including the ones they did not create.</p>                                                                                                                     |
| Light or Contributor  | <p>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</p> <br> <p>Users can view the views shared with them, but they cannot create their own. </p><br> <p>Users cannot create, edit, or delete workspaces, record types, records, or fields.</p>|
-->

<!--
Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->


## Tipi di licenza e autorizzazioni per aree di lavoro e tipi di record

La concessione di autorizzazioni utente a un&#39;area di lavoro consente inoltre di concedere autorizzazioni ai tipi di record, ai record e ai campi.

Per poter accedere alle viste e gestirle, è necessario concedere agli utenti autorizzazioni distinte per le viste, oltre a quelle di cui dispongono per le aree di lavoro.

Quando si utilizzano le autorizzazioni per il tipo di record, tenere presente quanto segue:

* Gli utenti ereditano automaticamente le autorizzazioni del tipo di record dalle aree di lavoro.
* Quando un utente dispone delle autorizzazioni di gestione per un’area di lavoro, non può avere un accesso inferiore a un tipo di record.
* Gli utenti non possono disporre di autorizzazioni maggiori per un tipo di record rispetto a quelle disponibili per l’area di lavoro a cui appartiene il tipo di record.
* Se si rimuovono le autorizzazioni degli utenti per un tipo di record, non viene rimosso il loro accesso di visualizzazione a tutti i tipi di record nell’area di lavoro, in quanto questo non rimuove le loro autorizzazioni per l’area di lavoro.

Solo gli utenti con una licenza di Planning Standard possono disporre delle autorizzazioni Contribute o Manage per le aree di lavoro e i tipi di record. Per impostazione predefinita, anche le autorizzazioni Contribute (Contribuisci) e Manage (Gestisci) per le aree di lavoro e i tipi di record vengono trasferite a record e campi.

Gli amministratori possono visualizzare tutte le aree di lavoro del sistema, incluse quelle che non hanno creato.

<!--
Lilit asked for this to be removed as there is no Planning Admin license/ access for combos: 
>[!TIP]
>
>Planning Administrator access is automatically assigned to users that you create as Administrators in the Adobe Admin Console. 
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Users with all other license types can have View permissions to workspaces and record types  shared with them, as well as to their records and fields. 
-->

>[!INFO]
>
>**ESEMPIO:**
>
>Gli utenti di Planning Contributor o Workflow Light non possono contribuire o gestire le aree di lavoro e i relativi oggetti.
>
>Nella casella Condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per contribuire a o gestire un’area di lavoro quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disabilitati.
>
>![Autorizzazioni disattivate per l&#39;utente collaboratore nell&#39;area di lavoro](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


## Tipi di licenza e autorizzazioni per le visualizzazioni

Solo gli utenti con una licenza Planning Standard possono disporre delle autorizzazioni di gestione per le visualizzazioni.

Gli amministratori non possono accedere alle viste che non hanno creato. Devono essere condivisi con loro.

Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le visualizzazioni condivise con loro.

>[!INFO]
>
>**ESEMPIO:**
>
>Gli utenti di Planning Contributor o Workflow Light-license non possono gestire le viste. Possono applicare filtri, ordinamenti o raggruppamenti temporanei alle visualizzazioni a cui possono accedere.
>
>Nella casella di condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per gestire una visualizzazione quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disattivati.
>
>![Autorizzazioni disattivate per l&#39;utente leggero nella condivisione di visualizzazione](assets/permissions-grayed-out-for-light-user.png)

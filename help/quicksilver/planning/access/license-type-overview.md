---
title: Panoramica Del Tipo Di Licenza Quando Si Utilizza Adobe Workfront Planning
description: L’accesso a Adobe Workfront Planning dipende dal tipo di licenza, oltre che dalle autorizzazioni per gli oggetti. Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. In questo articolo vengono descritti i livelli di accesso che gli utenti potrebbero avere a Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---


# Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Il tipo di licenza di Adobe Workfront funziona in combinazione con le autorizzazioni di Adobe Workfront Planning per concedere i seguenti accessi:

* Visualizzare, contribuire o gestire aree di lavoro o tipi di record
* Visualizzare o gestire le visualizzazioni.

Per informazioni sulle autorizzazioni per gli oggetti in Workfront Planning, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Per informazioni sull&#39;accesso a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Relazione tra i tipi di licenza di Workfront e le autorizzazioni di Workfront Planning

La tabella seguente descrive la relazione tra il tipo di licenza di un utente in Adobe Workfront e il livello di autorizzazioni che è possibile concedere agli oggetti di Adobe Workfront Planning in base a tale licenza.

La concessione di autorizzazioni utente a un&#39;area di lavoro consente inoltre di concedere autorizzazioni ai tipi di record, ai record e ai campi.

Per poter accedere alle viste e gestirle, è necessario concedere agli utenti autorizzazioni distinte per le viste, oltre a quelle di cui dispongono per le aree di lavoro.

Quando si utilizzano le autorizzazioni per il tipo di record, tenere presente quanto segue:

* Gli utenti ereditano automaticamente le autorizzazioni del tipo di record dalle aree di lavoro.
* Quando un utente dispone delle autorizzazioni di gestione per un’area di lavoro, non può avere un accesso inferiore a un tipo di record.
* Gli utenti non possono disporre di autorizzazioni maggiori per un tipo di record rispetto a quelle disponibili per l’area di lavoro a cui appartiene il tipo di record.
* Se si rimuovono le autorizzazioni degli utenti per un tipo di record, non viene rimosso il loro accesso di visualizzazione a tutti i tipi di record nell’area di lavoro, in quanto questo non rimuove le loro autorizzazioni per l’area di lavoro.

| Tipo di licenza Adobe Workfront | Autorizzazioni massime consentite in Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Gli utenti possono gestire aree di lavoro, tipi di record e visualizzazioni. Possono creare, modificare o eliminare aree di lavoro, tipi di record, record, campi e visualizzazioni.</p> <br> <p>Gli amministratori di sistema dispongono delle autorizzazioni di gestione per tutte le aree di lavoro, incluse quelle che non hanno creato.</p> |
| Light o Collaboratore | <p>Gli utenti possono visualizzare le aree di lavoro condivise, nonché i tipi di record, i record e i campi di tali aree di lavoro.</p> <br> <p>Gli utenti possono visualizzare le visualizzazioni condivise con loro, ma non possono crearne di proprie. </p><br> <p>Gli utenti non possono creare, modificare o eliminare aree di lavoro, tipi di record, record o campi.</p> |

<!--Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


### Tipi di licenza e autorizzazioni per aree di lavoro e tipi di record

Solo gli utenti con una licenza Standard possono disporre delle autorizzazioni Contribute o Manage per aree di lavoro e tipi di record. Anche le autorizzazioni Contribute e Manage per le aree di lavoro e i tipi di record vengono trasferite a record e campi.

Gli amministratori di sistema possono visualizzare tutte le aree di lavoro del sistema, incluse quelle che non hanno creato.

Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le aree di lavoro e i tipi di record condivisi con loro, nonché per i relativi record e campi.


>[!INFO]
>
>**ESEMPIO:**
>
>I collaboratori o gli utenti con licenza Light non possono contribuire o gestire le aree di lavoro e i relativi oggetti.
>
>Nella casella Condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per contribuire a o gestire un’area di lavoro quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disabilitati.
>
>![Autorizzazioni disattivate per l&#39;utente collaboratore nell&#39;area di lavoro](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Tipi di licenza e autorizzazioni per le visualizzazioni

Solo gli utenti con una licenza Standard possono disporre delle autorizzazioni di gestione per le visualizzazioni.

Gli amministratori di sistema non possono accedere alle viste che non hanno creato. Devono essere condivisi con loro.

Gli utenti con tutti gli altri tipi di licenza possono disporre delle autorizzazioni di visualizzazione per le visualizzazioni condivise con loro.

>[!INFO]
>
>**ESEMPIO:**
>
>I collaboratori o gli utenti con licenza Light non possono gestire le visualizzazioni. Possono applicare filtri, ordinamenti o raggruppamenti temporanei alle visualizzazioni a cui possono accedere.
>
>Nella casella di condivisione è indicato che non è possibile concedere agli utenti le autorizzazioni per gestire una visualizzazione quando dispongono di una licenza di livello inferiore, poiché tali livelli di autorizzazione sono disattivati.
>
>![Autorizzazioni disattivate per l&#39;utente leggero nella condivisione di visualizzazione](assets/permissions-grayed-out-for-light-user.png)

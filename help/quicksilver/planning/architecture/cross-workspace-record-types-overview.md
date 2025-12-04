---
title: Panoramica del tipo di record in più aree di lavoro
description: È possibile abilitare i tipi di record affinché siano globali o collegabili. I tipi di record globali possono essere aggiunti a più aree di lavoro da un'area di lavoro centrale o principale in Adobe Workfront Planning, mentre i tipi di record collegabili possono essere collegati a da altre aree di lavoro diverse dalla propria.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 0c890cc535c61c5402a334e43ed45b3ec3f9f748
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 0%

---


# Panoramica del tipo di record in più aree di lavoro

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedi [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

In Adobe Workfront Planning è possibile abilitare le funzionalità tra aree di lavoro diverse per un tipo di record. È possibile fare riferimento a un tipo di record di più aree di lavoro oppure accedervi da più aree di lavoro.

>[!IMPORTANT]
>
>Sono stati migliorati i requisiti dei pacchetti Workfront per poter abilitare le funzionalità tra aree di lavoro diverse per i tipi di record presenti nel sistema. Per informazioni, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).


Di seguito sono riportate le funzionalità dei tipi di record in più aree di lavoro:

* <span class="preview">**Tipi di record globali**: gli utenti possono aggiungere tipi di record globali ad altre aree di lavoro che gestiscono.</span>

* **Tipi di record collegabili**: gli utenti possono connettersi a questo tipo di record da altre aree di lavoro.

Questo articolo offre una panoramica dei tipi di record tra aree di lavoro diverse. Per informazioni sulla definizione delle funzionalità tra aree di lavoro di un tipo di record, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

<div class="preview">

## Panoramica dei tipi di record globali

I tipi di record globali possono essere aggiunti a più aree di lavoro da un&#39;area di lavoro centrale o principale in Workfront Planning.

Quando si implementa Workfront Planning per un’organizzazione con più team e flussi di lavoro comuni, potrebbe essere necessario definire una struttura coesa e i metadati per i tipi di record chiave (come Campagne o Deliverable) che possono essere aggiunti alle aree di lavoro di ciascun team per acquisire e gestire il proprio lavoro.

Inoltre, potrebbe essere necessario il lavoro di ogni team per raggiungere un livello centrale.

In un flusso di lavoro di questo tipo, puoi fare in modo che i team acquisiscano il proprio lavoro in modo coerente sbloccando la visibilità tra i team, senza dover aggiungere tutto a un’area di lavoro o tutti gli utenti dell’organizzazione a ogni area di lavoro. A tale scopo, è possibile utilizzare i tipi di record globali.

Per utilizzare i tipi di record globali, eseguire le operazioni seguenti:

1. Da un&#39;area di lavoro gestita, configurare un tipo di record come globale.

   Un manager dell&#39;area di lavoro può concedere autorizzazioni agli utenti con una licenza Standard oppure ai team, ai gruppi, ai ruoli e alle società per aggiungere un tipo di record scelto alle aree di lavoro che gestiscono.

   Il tipo di record originale sarà presente nell&#39;area di lavoro originale ma sarà reso visibile in altre aree di lavoro.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Aggiungere un tipo di record a un&#39;area di lavoro secondaria da una esistente configurata come tipo di record globale.

   Il tipo di record esiste nelle aree di lavoro seguenti:

   * Area di lavoro originale in cui è stato designato come tipo di record globale.
   * Un workspace secondario.

   Per informazioni, vedere [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Nelle sezioni seguenti vengono descritte considerazioni sui tipi di record globali e sul loro funzionamento nelle aree di lavoro originali o secondarie.

### Considerazioni sui tipi di record globali nell&#39;area di lavoro originale

Il tipo di record configurato come globale presenta le seguenti proprietà:

* Tutte le relative informazioni (aspetto, campi originali) possono essere modificate solo nell&#39;area di lavoro originale.

* Nel tipo di record globale è possibile eseguire le azioni seguenti dall&#39;area di lavoro originale:

   * Modifica

     La modifica di un tipo di record globale include la modifica dell&#39;aspetto, delle funzionalità per più aree di lavoro e di tutti i campi creati nell&#39;area di lavoro originale.
   * Creare e gestire i moduli di richiesta
   * Creare e gestire le automazioni

* È possibile eliminare un tipo di record globale solo se non è stato aggiunto a un&#39;area di lavoro secondaria. Prima di eliminarlo dall&#39;area di lavoro originale, è necessario rimuoverlo dalle aree di lavoro secondarie.

  Per ulteriori informazioni, vedere [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).
* I record aggiunti a un tipo di record globale sono visibili solo agli utenti che dispongono delle autorizzazioni di visualizzazione per l&#39;area di lavoro in cui sono stati aggiunti.
* I record aggiunti da un workspace secondario vengono aggregati e visualizzati nel workspace originale. Tutti i membri dell&#39;area di lavoro originale ottengono le relative autorizzazioni di visualizzazione.
* Quando il tipo di record globale originale viene aggiunto a più aree di lavoro secondarie, esistono i seguenti scenari:

   * I membri dell&#39;area di lavoro originale ottengono automaticamente le autorizzazioni di visualizzazione per tutti i record aggiunti da qualsiasi area di lavoro, anche se non sono membri di tali aree di lavoro.
   * I membri dell&#39;area di lavoro secondaria possono visualizzare solo i record delle aree di lavoro in cui sono membri.
* I tipi di record connessi di un tipo di record globale saranno disponibili per la connessione dalle aree di lavoro in cui viene aggiunto il tipo di record.

  Ad esempio, se disponi di un tipo di record globale Campaign con una connessione a un tipo di record Aree geografiche e aggiungi il tipo di record Campaign a un’area di lavoro secondaria, le aree diventeranno collegabili tra aree di lavoro diverse dall’area di lavoro secondaria. I membri dell’area di lavoro secondaria possono ora creare campagne e collegarle alle aree geografiche.

* I campi creati per un tipo di record globale dall&#39;area di lavoro originale sono visibili da tutte le aree di lavoro in cui viene aggiunto il tipo di record. È possibile modificare le impostazioni dei campi solo dall&#39;area di lavoro originale. Le impostazioni dei campi creati nell&#39;area di lavoro originale sono di sola lettura nelle aree di lavoro secondarie per tutti i membri, indipendentemente dalle relative autorizzazioni nell&#39;area di lavoro secondaria. I responsabili dell&#39;area di lavoro secondaria non possono modificare le impostazioni dei campi configurati nell&#39;area di lavoro originale. Solo i responsabili dell&#39;area di lavoro dell&#39;area di lavoro originale possono modificare le impostazioni dei campi nell&#39;area di lavoro originale.

### Considerazioni sui tipi di record globali in un workspace secondario

* I collaboratori dell&#39;area di lavoro secondaria ottengono l&#39;autorizzazione Contribute per il tipo di record globale nell&#39;area di lavoro del proprio team. Possono aggiungere e gestire i record in esso contenuti dall’area di lavoro secondaria.

* I visualizzatori dell&#39;area di lavoro secondaria ottengono l&#39;autorizzazione di visualizzazione per il tipo di record globale nell&#39;area di lavoro del team. Non possono aggiungere e gestire record al suo interno.

* I responsabili dell&#39;area di lavoro secondaria possono eseguire le azioni aggiuntive seguenti sul tipo di record aggiunto da un tipo di record globale in un&#39;area di lavoro secondaria:

   * Eliminalo.

     Se si elimina il tipo di record da un workspace secondario, questo viene rimosso solo dal workspace secondario. Verranno eliminati anche i record e i campi aggiunti a esso dall’area di lavoro secondaria. Il tipo di record non viene eliminato dall&#39;area di lavoro originale o da altre aree di lavoro secondarie in cui è stato aggiunto.

     Per ulteriori informazioni, vedere [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Condividere le visualizzazioni dei tipi di record.

     Non è possibile condividere una visualizzazione pubblicamente da un tipo di record globale in un&#39;area di lavoro secondaria. È possibile condividere le viste solo internamente da un workspace secondario. È possibile condividere una visualizzazione internamente e pubblicamente per un tipo di record globale nell&#39;area di lavoro originale.

     Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).


     <!-- when they will be able to add fields to the secondary space, this bullet will need this extra information: 
         After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added. -->

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* Nessun utente può eseguire le azioni seguenti su un tipo di record globale in un&#39;area di lavoro secondaria:

   * Modifica

     Non è possibile modificarne l’aspetto, le funzionalità tra aree di lavoro diverse o i campi aggiunti dall’area di lavoro originale.
   * Condividi
   * Creare e gestire i moduli di richiesta
   * Creare e gestire le automazioni

* I record aggiunti in un&#39;area di lavoro secondaria sono visibili dalle aree di lavoro seguenti solo se si dispone delle autorizzazioni di visualizzazione o di livello superiore per tali aree di lavoro:

   * L’area di lavoro secondaria in cui vengono aggiunti.
   * Area di lavoro originale del tipo di record globale.
   * Tutte le altre aree di lavoro in cui viene aggiunto il workspace globale.

* Esistono i seguenti scenari per i record creati nelle aree di lavoro secondarie:

   * Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro originale e non si dispone delle autorizzazioni per le aree di lavoro secondarie, è possibile visualizzare i record aggiunti dalle aree di lavoro secondarie nell&#39;area di lavoro originale, ma non è possibile gestirli dall&#39;area di lavoro originale.
   * Se si dispone delle autorizzazioni Gestione nell&#39;area di lavoro secondaria, è possibile gestire i record sia dall&#39;area di lavoro originale del tipo di record globale che dall&#39;area di lavoro secondaria in cui sono stati aggiunti.
   * È possibile visualizzare i record in aree di lavoro secondarie aggiuntive in cui il tipo di record globale viene aggiunto solo se si dispone delle autorizzazioni di visualizzazione per tali aree di lavoro.

### Accesso alle connessioni di un tipo di record globale

I tipi di record connessi al tipo di record globale nell&#39;area di lavoro originale diventano visibili da altre aree di lavoro in cui viene aggiunto il tipo di record globale e sono disponibili per le connessioni dalle aree di lavoro secondarie in cui viene aggiunto il tipo di record globale.

### Accesso API di un tipo di record globale

Quando si aggiungono record a un tipo di record globale da un&#39;area di lavoro secondaria utilizzando l&#39;API di Workfront Planning, il sistema controlla se l&#39;utente ha accesso alla creazione di record nell&#39;area di lavoro originale del tipo di record globale.

Esistono i seguenti casi:

* Se l&#39;utente dispone dell&#39;accesso, il record viene creato nell&#39;area di lavoro originale dei tipi di record globali.

* Se l&#39;utente non dispone dell&#39;accesso, riceve un errore che indica che non ha accesso all&#39;area di lavoro originale del tipo di record globale e che deve fornire l&#39;ID dell&#39;area di lavoro a cui ha accesso per creare i record.

</div>

## Panoramica dei tipi di record collegabili

È possibile connettersi a un tipo di record definito come collegabile da qualsiasi area di lavoro gestita.

È possibile che i team necessitino di record collegati a tipi di record di altre aree di lavoro o di visualizzare informazioni acquisite su record appartenenti a record di altre aree di lavoro. È possibile ottenere questa configurazione designando un tipo di record come collegabile.

Per utilizzare i tipi di record collegabili, effettuare le seguenti operazioni:

1. Configurare un tipo di record in modo che sia collegabile in un&#39;area di lavoro specifica.

   Un workspace manager può selezionare le aree di lavoro a cui è disponibile un determinato tipo di record.

   Il tipo di record originale sarà presente nell&#39;area di lavoro originale e potrà essere accessibile da un&#39;altra area di lavoro.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Connettersi a un tipo di record designato come collegabile da un&#39;altra area di lavoro gestita.

   Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

---
title: Panoramica dei tipi di record in più aree di lavoro
description: I tipi di record centralizzati possono essere aggiunti a più aree di lavoro da un'area di lavoro centrale o principale in Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Panoramica sui tipi di record in più aree di lavoro

In Adobe Workfront Planning è possibile abilitare le funzionalità tra aree di lavoro per un tipo di record che consente di fare riferimento a un tipo di record in più aree di lavoro.

Di seguito sono riportate le funzionalità dei tipi di record in più aree di lavoro:

* È possibile designare un tipo di record come centralizzato. Gli utenti possono aggiungere tipi di record centralizzati ad altre aree di lavoro che possono gestire.
* È possibile designare un tipo di record come collegabile. Gli utenti possono connettersi a questo tipo di record da altre aree di lavoro.

Questo articolo offre una panoramica dei tipi di record tra aree di lavoro diverse. Per informazioni sulla definizione delle funzionalità tra aree di lavoro di un tipo di record, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Panoramica dei tipi di record centralizzati

I tipi di record centralizzati possono essere aggiunti a più aree di lavoro da un&#39;area di lavoro centrale o principale in Adobe Workfront Planning.

Quando si implementa Workfront Planning per un’organizzazione con più team e flussi di lavoro comuni, potrebbe essere necessario definire una struttura coesa e i metadati per i tipi di record chiave (come Campagne o Deliverable) che possono essere aggiunti alle aree di lavoro di ciascun team per acquisire e gestire il proprio lavoro.

Inoltre, potrebbe essere necessario il lavoro di ogni team per raggiungere un livello centrale.

In un flusso di lavoro di questo tipo, puoi fare in modo che i team acquisiscano il proprio lavoro in modo coerente sbloccando la visibilità tra i team, senza dover aggiungere tutto a un’area di lavoro o tutti gli utenti dell’organizzazione a ogni area di lavoro. A tale scopo è possibile utilizzare tipi di record centralizzati.

Per utilizzare i tipi di record centralizzati, eseguire le operazioni seguenti:

1. Configurare un tipo di record da centralizzare in un workspace specifico.

   Un responsabile dell&#39;area di lavoro può selezionare gli utenti con una licenza Standard, i team, i gruppi, i ruoli o le società per aggiungere un tipo di record scelto alle aree di lavoro che gestisce.

   Il tipo di record originale sarà presente nell&#39;area di lavoro originale ma sarà reso visibile da tutte le altre aree di lavoro.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Aggiungere a un&#39;area di lavoro secondaria un tipo di record esistente configurato come tipo di record centralizzato.

   Il tipo di record esiste nelle aree di lavoro seguenti:

   * Area di lavoro originale in cui è stato designato come tipo di record centralizzato.
   * Un workspace secondario.

   Per informazioni, vedere [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Nelle sezioni seguenti vengono descritte considerazioni sui tipi di record centralizzati e sul loro funzionamento nelle aree di lavoro originali o secondarie.

### Considerazioni sui tipi di record centralizzati nell&#39;area di lavoro originale

Il tipo di record configurato per essere centralizzato ha le seguenti proprietà:

* Tutte le relative informazioni possono essere modificate solo nell&#39;area di lavoro originale.

* È possibile eseguire le azioni seguenti sul tipo di record centralizzato dall&#39;area di lavoro originale di un tipo di record centralizzato:

   * Modifica

     La modifica di un tipo di record centralizzato include la modifica dell&#39;aspetto, delle funzionalità per più aree di lavoro e di tutti i campi creati nell&#39;area di lavoro originale.
   * Creare moduli di richiesta
   * Gestisci i moduli di richiesta

* È possibile eliminare un tipo di record centralizzato solo se non è stato aggiunto a un&#39;area di lavoro secondaria. Dopo essere stato aggiunto a un’altra area di lavoro, se provi a eliminarla dall’area di lavoro originale viene generato un errore.

  In questo modo il tipo di record centralizzato può rimanere nelle aree di lavoro in cui è già stato aggiunto.
* I record aggiunti a un tipo di record centralizzato sono visibili solo agli utenti che dispongono delle autorizzazioni di visualizzazione per l&#39;area di lavoro in cui sono stati aggiunti.
* I record aggiunti da un workspace secondario vengono aggregati e visualizzati nel workspace originale. Tutti i membri dell&#39;area di lavoro originale ottengono le autorizzazioni di visualizzazione.

* I tipi di record connessi di un tipo di record centralizzato saranno disponibili per la connessione dalle aree di lavoro in cui viene aggiunto questo tipo di record.

  Ad esempio, se disponi di un tipo di record Campaign con una connessione con il tipo di record Aree geografiche e aggiungi il tipo di record Campaign a un’area di lavoro secondaria, Aree geografiche diventeranno collegabili tra aree di lavoro diverse per l’area di lavoro secondaria. I membri dell’area di lavoro secondaria possono ora creare campagne e collegarle alle aree geografiche.

* I campi creati per un tipo di record centralizzato dall&#39;area di lavoro originale sono visibili da tutte le aree di lavoro in cui viene aggiunto il tipo di record. I campi di un workspace originale sono di sola lettura nelle aree di lavoro secondarie.

### Considerazioni sui tipi di record centralizzati dopo averli aggiunti a un workspace secondario

* I collaboratori dell&#39;area di lavoro secondaria ottengono l&#39;autorizzazione Contribute per il tipo di record centralizzato nell&#39;area di lavoro del proprio team. Possono aggiungere e gestire i record al suo interno.

* I visualizzatori dell&#39;area di lavoro secondaria ottengono l&#39;autorizzazione di visualizzazione per il tipo di record centralizzato nell&#39;area di lavoro del team. Non possono aggiungere e gestire record in.

* I responsabili dell&#39;area di lavoro secondaria possono eseguire le azioni seguenti sul tipo di record aggiunto da un tipo di record centralizzato in un&#39;area di lavoro secondaria:

   * Eliminalo.

     Se si elimina il tipo di record da un workspace secondario, questo viene rimosso solo dal workspace secondario. Verranno eliminati anche i record aggiunti dall&#39;area di lavoro secondaria. Il tipo di record non viene eliminato dall&#39;area di lavoro originale o da altre aree di lavoro secondarie in cui è stato aggiunto.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Non è possibile eseguire le azioni seguenti sul tipo di record aggiunto da un tipo di record centralizzato in un&#39;area di lavoro secondaria:

   * Modifica

     Non è possibile modificarne l’aspetto, le funzionalità tra aree di lavoro diverse o i campi aggiunti dall’area di lavoro originale.
   * Creare e gestire i moduli di richiesta
   * Creare e gestire i moduli di richiesta

* I record aggiunti in un&#39;area di lavoro secondaria sono visibili dalle aree di lavoro seguenti, se si dispone delle autorizzazioni di visualizzazione o di livello superiore per tali aree di lavoro:

   * L’area di lavoro secondaria in cui vengono aggiunti.
   * Area di lavoro originale del tipo di record centralizzato.
   * Tutte le altre aree di lavoro in cui viene aggiunto il workspace centralizzato.

* Esistono i seguenti scenari per i record creati nelle aree di lavoro dei team:

   * Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro originale e non si dispone delle autorizzazioni per le aree di lavoro secondarie, è possibile visualizzare i record aggiunti dalle aree di lavoro secondarie nell&#39;area di lavoro originale, ma non è possibile gestirli dall&#39;area di lavoro originale.
   * Se si dispone delle autorizzazioni Gestione nell&#39;area di lavoro secondaria, è possibile gestire i record nell&#39;area di lavoro originale del tipo di record centralizzato o dall&#39;area di lavoro in cui sono stati aggiunti.

     È possibile visualizzare i record in aree di lavoro secondarie aggiuntive in cui il tipo di record centralizzato viene aggiunto solo se si dispone delle autorizzazioni di visualizzazione per tali aree di lavoro.

### Accesso alle connessioni di un record centralizzato

I tipi di record connessi al tipo di record centralizzato nell&#39;area di lavoro originale diventano visibili da altre aree di lavoro in cui viene aggiunto il tipo di record centralizzato.

### Accesso API di tipo record centralizzato

Quando si aggiungono record a un tipo di record centralizzato da un&#39;area di lavoro secondaria utilizzando l&#39;API di Workfront Planning, il sistema controlla se l&#39;utente ha accesso alla creazione di record nell&#39;area di lavoro originale del tipo di record centralizzato.

Esistono i seguenti casi:

* Se l&#39;utente dispone dell&#39;accesso, il record viene creato nell&#39;area di lavoro originale dei tipi di record centralizzati.

* Se l&#39;utente non dispone dell&#39;accesso, riceve un errore che indica che non ha accesso all&#39;area di lavoro originale del tipo di record centralizzato e che deve fornire l&#39;ID area di lavoro in cui ha accesso per creare i record.

## Panoramica dei tipi di record collegabili

È possibile connettersi a un tipo di record definito come collegabile da qualsiasi area di lavoro gestita.

È possibile che i team necessitino di record collegati a tipi di record di altre aree di lavoro o di visualizzare informazioni acquisite su record appartenenti a record di altre aree di lavoro. È possibile ottenere questa configurazione designando un tipo di record come collegabile.

Per utilizzare i tipi di record collegabili, effettuare le seguenti operazioni:

1. Configurare un tipo di record in modo che sia collegabile in un&#39;area di lavoro specifica.

   Un workspace manager può selezionare le aree di lavoro a cui è disponibile un determinato tipo di record.

   Il tipo di record originale sarà presente nell&#39;area di lavoro originale e verrà aggiunto come tipo di record connesso a un&#39;altra area di lavoro.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Connettersi a un tipo di record designato come collegabile da un&#39;altra area di lavoro gestita.

   Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

   Nelle sezioni seguenti vengono descritte considerazioni sui tipi di record centralizzati e sul loro funzionamento nelle aree di lavoro originali o secondarie.
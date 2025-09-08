---
title: Panoramica dei tipi di record centralizzati
description: I tipi di record centralizzati possono essere aggiunti a più aree di lavoro da un'area di lavoro centrale o principale in Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Panoramica sui tipi di record centralizzati

I tipi di record centralizzati possono essere aggiunti a più aree di lavoro da un&#39;area di lavoro centrale o principale in Adobe Workfront Planning.

## Panoramica dei tipi di record centralizzati

Quando si implementa Workfront Planning per un’organizzazione con più team e flussi di lavoro comuni, potrebbe essere necessario definire una struttura coesa e i metadati per i tipi di record chiave (come Campagne o Deliverable) che possono essere aggiunti alle aree di lavoro di ciascun team per acquisire e gestire il proprio lavoro.

Inoltre, potrebbe essere necessario il lavoro di ogni team per raggiungere un livello centrale.

In un flusso di lavoro di questo tipo, puoi fare in modo che i team acquisiscano il proprio lavoro in modo coerente sbloccando la visibilità tra i team, senza dover aggiungere tutto a un’area di lavoro o tutti gli utenti dell’organizzazione a ogni area di lavoro. A tale scopo è possibile utilizzare tipi di record centralizzati.

Per utilizzare i tipi di record centralizzati, eseguire le operazioni seguenti:

1. Configurare un tipo di record da centralizzare in un workspace specifico.

   Un responsabile dell&#39;area di lavoro può selezionare gli utenti con una licenza Standard, i team, i gruppi, i ruoli o le società per aggiungere un tipo di record scelto alle aree di lavoro che gestisce.

   Il tipo di record originale sarà presente nell&#39;area di lavoro originale ma sarà reso visibile da tutte le altre aree di lavoro.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Aggiungere all&#39;area di lavoro di un team un tipo di record esistente configurato come record centralizzato.

   Il tipo di record esiste nelle aree di lavoro seguenti:

   * Area di lavoro originale in cui è stato designato come tipo di record centralizzato.
   * Area di lavoro del team.

   Per informazioni, vedere [Aggiungere tipi di record esistenti](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   Nelle sezioni seguenti vengono descritte considerazioni sui tipi di record centralizzati nelle aree di lavoro originali o dopo che sono stati aggiunti alle aree di lavoro di un team.

## Considerazioni sui tipi di record centralizzati nell&#39;area di lavoro originale

Il tipo di record configurato per essere centralizzato ha le seguenti proprietà:

* Tutte le relative informazioni possono essere modificate solo nell&#39;area di lavoro originale.

* È possibile eseguire le azioni seguenti sul tipo di record centralizzato dall&#39;area di lavoro originale di un tipo di record centralizzato:

   * Modifica

     La modifica di un tipo di record centralizzato include la modifica dell&#39;aspetto, delle funzionalità per più aree di lavoro e di tutti i campi creati nell&#39;area di lavoro originale.
   * Creare moduli di richiesta
   * Gestisci i moduli di richiesta

* È possibile eliminare un tipo di record centralizzato solo se non è stato aggiunto a un&#39;area di lavoro del team. Dopo essere stato aggiunto all’area di lavoro di un team, se provi a eliminarlo dall’area di lavoro originale viene generato un errore.

  In questo modo il tipo di record centralizzato può rimanere nelle aree di lavoro in cui è già stato aggiunto.
* I record aggiunti a un tipo di record centralizzato sono visibili solo agli utenti che dispongono delle autorizzazioni di visualizzazione per l&#39;area di lavoro originale.
* I record aggiunti dall&#39;area di lavoro del team vengono visualizzati nell&#39;area di lavoro originale. Tutti i membri dell&#39;area di lavoro originale ottengono le autorizzazioni di visualizzazione.

* I tipi di record connessi di un tipo di record centralizzato saranno disponibili per la connessione dalle aree di lavoro in cui viene aggiunto questo tipo di record.

* I campi creati per un tipo di record centralizzato dall&#39;area di lavoro originale sono visibili da tutte le aree di lavoro in cui viene aggiunto il tipo di record.

## Considerazioni sui tipi di record centralizzati dopo averli aggiunti all&#39;area di lavoro di un team

* I collaboratori dell&#39;area di lavoro del team ottengono l&#39;autorizzazione Contribute per il tipo di record centralizzato nell&#39;area di lavoro del team. Possono aggiungere e gestire i record al suo interno.

* I visualizzatori dell&#39;area di lavoro del team ottengono l&#39;autorizzazione di visualizzazione per il tipo di record centralizzato nell&#39;area di lavoro del team. Non possono aggiungere e gestire record in.

* I responsabili dell&#39;area di lavoro del team possono eseguire le azioni seguenti sul tipo di record aggiunto da un tipo di record centralizzato nell&#39;area di lavoro di un team:

   * Aggiungi nuovi campi

     I campi aggiunti a un record centralizzato da un&#39;area di lavoro del team sono visibili solo dall&#39;area di lavoro del team.
   * Condividi
   * Eliminalo.

     Se si elimina il tipo di record dall&#39;area di lavoro di un team, questo viene rimosso solo dall&#39;area di lavoro del team. Vengono eliminati anche i record aggiunti al gruppo dall&#39;area di lavoro del team. Il tipo di record non viene eliminato dall&#39;area di lavoro originale o da altre aree di lavoro del team in cui è stato aggiunto.

     Questa operazione consente di mantenere il tipo di record centralizzato già aggiunto nelle aree di lavoro che lo utilizzano già.

* Non è possibile eseguire le azioni seguenti sul tipo di record aggiunto da un tipo di record centralizzato nell&#39;area di lavoro di un team:

   * Modifica

     Non è possibile modificarne l&#39;aspetto, le funzionalità tra aree di lavoro o i campi importati dall&#39;area di lavoro originale.
   * Creare moduli di richiesta
   * Gestisci i moduli di richiesta

* I record aggiunti nelle aree di lavoro di un team sono visibili dalle aree di lavoro seguenti, se si dispone delle autorizzazioni di visualizzazione o di livello superiore per tali aree di lavoro:

   * L’area di lavoro del team in cui vengono aggiunti.
   * Area di lavoro originale del tipo di record centralizzato.
   * Tutte le altre aree di lavoro in cui viene aggiunto il workspace centralizzato.

* Esistono i seguenti scenari per i record creati nelle aree di lavoro dei team:

   * Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro originale e non si dispone delle autorizzazioni per le aree di lavoro dei team, è possibile visualizzare i record aggiunti dalle aree di lavoro del team nell&#39;area di lavoro originale, ma non è possibile gestirli dall&#39;area di lavoro originale.
   * Se si dispone delle autorizzazioni Gestione nell&#39;area di lavoro del team, è possibile gestire i record nell&#39;area di lavoro originale del tipo di record centralizzato o dall&#39;area di lavoro in cui sono stati aggiunti.

     È possibile visualizzare i record in altre aree di lavoro del team in cui il tipo di record centralizzato viene aggiunto solo se si dispone delle autorizzazioni di visualizzazione per tali aree di lavoro.

## Accesso alle connessioni

I tipi di record connessi al tipo di record centralizzato nell&#39;area di lavoro originale diventano visibili per le aree di lavoro del team in cui viene aggiunto il tipo di record centralizzato.

## Comportamento API

Quando si aggiungono record a un tipo di record centralizzato da un&#39;area di lavoro del team utilizzando l&#39;API di Workfront Planning, il sistema controlla se l&#39;utente ha accesso alla creazione di record nell&#39;area di lavoro originale del tipo di record centralizzato.

Esistono i seguenti casi:

* Se l&#39;utente dispone dell&#39;accesso, il record viene creato nell&#39;area di lavoro originale dei tipi di record centralizzati.

* Se l&#39;utente non dispone dell&#39;accesso, riceve un errore che indica che non ha accesso all&#39;area di lavoro originale del tipo di record centralizzato e che deve fornire l&#39;ID area di lavoro in cui ha accesso per creare i record.
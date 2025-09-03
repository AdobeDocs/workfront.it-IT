---
title: Panoramica dei tipi di record centralizzati
description: I tipi di record centralizzati possono essere aggiunti a più aree di lavoro da un'area di lavoro centrale o principale in Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
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

Inoltre, potrebbe essere necessario il lavoro di ogni team per passare a un livello centrale e più globale.

In questo flusso di lavoro, puoi fare in modo che i team acquisiscano il proprio lavoro in modo coerente sbloccando la visibilità tra i team, senza la necessità di aggiungere tutti gli utenti dell’organizzazione a un’unica area di lavoro.

Per utilizzare i tipi di record centralizzati, eseguire le operazioni seguenti:

1. Configurare un tipo di record da centralizzare.

   Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Aggiungere un tipo di record esistente da uno centralizzato.

   Per informazioni, vedere [Aggiungere tipi di record esistenti](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




· In Impostazioni avanzate per i tipi di record è disponibile la nuova impostazione &quot;Consenti l’aggiunta del tipo di record in altre aree di lavoro&quot;.

· Se questa opzione è abilitata, il manager dell&#39;area di lavoro può selezionare gli utenti con licenza Standard, i team, i gruppi, i ruoli o le aziende che possono aggiungere il tipo di record nelle aree di lavoro che gestiscono.

· Per impostazione predefinita, il manager dell&#39;area di lavoro che sta modificando l&#39;impostazione viene aggiunto automaticamente all&#39;elenco degli utenti selezionati

o Il manager dell&#39;area di lavoro può rimuovere il proprio nome dopo aver aggiunto almeno un&#39;altra entità

o Per salvare l&#39;impostazione è necessario selezionare almeno un utente/team/...

o Una volta aggiunto il tipo di record in almeno un&#39;altra area di lavoro, è possibile rimuovere tutti gli utenti selezionati

§ Questa operazione consente di impedire l&#39;aggiunta del tipo di record globale in nuove aree di lavoro, ma di mantenerlo in quelle già in uso.

· Nella fase 1, tutti i record dei tipi di record collegati vengono condivisi automaticamente con qualsiasi area di lavoro in cui è stato aggiunto il tipo di record.

· Una volta abilitato il tipo di record come cross-workspace, al tipo di record viene aggiunto un campo &quot;Workspace&quot; generato dal sistema

o Visualizza l&#39;area di lavoro da cui è stato creato ogni record.

o Questo campo è di sola lettura e non può essere eliminato.

o Può essere nascosto nei campi di visualizzazione.

o Il campo dell&#39;area di lavoro può essere utilizzato per filtrare, raggruppare e ordinare, nonché in qualsiasi impostazione di visualizzazione, come in altri campi.


Tipi di record cross-Workspace nelle aree di lavoro locali

· Quando si tenta di aggiungere un nuovo tipo di record all&#39;area di lavoro, i responsabili dell&#39;area di lavoro locale visualizzano un&#39;opzione per selezionare dall&#39;elenco dei tipi di record globali disponibili

· Quando viene selezionato uno dei tipi di record globali, questo viene aggiunto immediatamente all&#39;area di lavoro

· È possibile spostare il tipo di record globale in qualsiasi sezione e posizione all&#39;interno dell&#39;area di lavoro locale


Autorizzazioni per il tipo di record globale nelle aree di lavoro locali

All&#39;interno delle aree di lavoro locali, i membri possono accedere al tipo di record globale nel modo seguente:

· Nella fase 1, i responsabili locali dell&#39;area di lavoro ottengono l&#39;autorizzazione Contribute. Ciò significa che:

o I responsabili dell&#39;area di lavoro locale possono:

§ Aggiungere il tipo di record globale

§ Aggiungere, modificare o eliminare record nel tipo di record globale, indipendentemente dall&#39;area di lavoro da cui è stato aggiunto il record.

§ Eliminare il tipo di record globale dall&#39;area di lavoro locale

o I responsabili dell&#39;area di lavoro locale non possono:

§ Aggiungere, modificare, eliminare campi

§ Aggiornare l&#39;aspetto e l&#39;etichetta del tipo di record

§ Vedere impostazioni avanzate per il tipo di record

Automazioni di § Manage

§ Gestire i moduli di richiesta

§ Regolare la condivisione del tipo di record per l&#39;ambito dell&#39;area di lavoro

§ Disattivare l&#39;impostazione del tipo di record globale nelle impostazioni avanzate.

· I collaboratori dell&#39;area di lavoro locale ottengono l&#39;autorizzazione Contribute per il tipo di record globale e possono aggiungere e gestire record al suo interno

· I visualizzatori dell&#39;area di lavoro locale ottengono l&#39;autorizzazione di visualizzazione per il tipo di record globale

· Non appena un record viene aggiunto al tipo di record globale da una delle aree di lavoro locali, il campo Workspace mostra tale nome dell’area di lavoro

o Per il momento non è possibile modificare il campo dell&#39;area di lavoro

· I record aggiunti alle aree di lavoro locali vengono tutti aggregati e visualizzati nell&#39;area di lavoro principale e tutti i membri dell&#39;area di lavoro principale vi accedono.

· I record aggiunti nelle aree di lavoro locali non vengono visualizzati in altre aree di lavoro locali che utilizzano lo stesso tipo di record globale e i relativi membri non hanno accesso ai record.



Accesso alle connessioni:

· Ambito MVP

o I tipi di record connessi al tipo di record globale diventeranno visibili per le aree di lavoro locali in cui viene aggiunto il tipo di record globale, in modo che possano utilizzare i campi di connessione per assegnare tag


Comportamento API

Se l’utente tenta di creare record in un tipo di record globale tramite API senza fornire l’ID dell’area di lavoro, il sistema controlla se l’utente ha accesso alla creazione di record nell’area di lavoro principale (dove viene creato il tipo di record globale)

· In caso affermativo, il record viene creato nell&#39;area di lavoro principale

· In caso contrario, l’utente riceve un errore di convalida a causa del quale non ha accesso all’area di lavoro principale e deve fornire l’ID dell’area di lavoro in cui può creare.
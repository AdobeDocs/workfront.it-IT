---
title: Panoramica dei record collegati
description: Dopo aver creato connessioni tra tipi di record, è possibile collegare tra loro singoli record. In questo articolo vengono descritte le considerazioni da tenere in considerazione per la connessione dei record in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Panoramica sui record collegati

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

È possibile collegare tra loro record di Adobe Workfront Planning o a oggetti di altre applicazioni.

In questo articolo vengono descritte le considerazioni da tenere in considerazione per la connessione dei record in Workfront Planning.

Per informazioni su come connettere i record tra loro o a un altro oggetto, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## Prerequisiti

Prima di poter connettere i record in Workfront Planning, è necessario connettere quanto segue:

* Due tipi di record
* Un tipo di record con un oggetto di un&#39;altra applicazione

Per ulteriori informazioni, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).


## Considerazioni sulla connessione dei record

* Dopo aver connesso i tipi di record, i tipi di record connessi vengono visualizzati come campi di connessione nella tabella dei tipi di record da cui sono collegati e nelle pagine dei record.
* È possibile sfogliare e aggiungere record e oggetti dei tipi di record e oggetti collegati dai campi dei record collegati.
* È possibile aggiungere campi (campi di ricerca) dei tipi di record collegati nella tabella del tipo di record da cui si sta effettuando il collegamento.

  È inoltre possibile aggiungere campi (campi di ricerca) dei tipi di record da cui si sta effettuando il collegamento nella tabella del tipo di record a cui si sta effettuando il collegamento.

  Ad esempio, se colleghi il tipo di record Prodotto dal tipo di record Campagna, puoi visualizzare i campi prodotto per le campagne e i campi campagna per i prodotti.
* Non è possibile aggiornare manualmente i valori dei campi di ricerca nei record da cui si sta effettuando il collegamento.

  I valori dei campi di ricerca vengono inseriti automaticamente nel record di Workfront Planning da cui si sta eseguendo il collegamento dopo l&#39;aggiornamento nel record o nell&#39;oggetto originale.

* Tutti coloro che dispongono dell&#39;accesso a Workfront Planning and View o di autorizzazioni superiori per l&#39;area di lavoro e un tipo di record possono visualizzare le connessioni che si creano tra record o tra record e oggetti di altre applicazioni. Possono visualizzare i record e gli oggetti connessi indipendentemente dalle autorizzazioni di cui dispongono nelle applicazioni a cui ci si connette.
* È possibile visualizzare e modificare le connessioni di tutti gli altri utenti se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro e il tipo di record in cui si trovano i record connessi.
* È possibile connettere un record a uno o più oggetti di un&#39;altra applicazione, a seconda del tipo di connessione selezionata durante la connessione dei tipi di record. Per ulteriori informazioni, vedere la sezione &quot;Tipi di connessione&quot; nell&#39;articolo [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* Quando i tipi di record connessi fanno parte di gerarchie, è possibile accedere a qualsiasi tipo di oggetto all&#39;interno della gerarchia dalle pagine dei record. Per informazioni, vedere [Panoramica della gerarchia e delle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
* Quando i tipi di record connessi fanno parte di gerarchie, è possibile collegare un record da un tipo di record figlio a un massimo di 10 record da un tipo di record padre. Per informazioni, vedere [Panoramica della gerarchia e delle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Aree in cui è possibile collegare i record

È possibile collegare i record manualmente o automaticamente in Workfront.

### Connetti record manualmente

È possibile connettere manualmente i record ad altri record o a oggetti di un&#39;altra applicazione nelle seguenti aree:

* È possibile collegare record da Workfront Planning a oggetti Workfront, oggetti Experience Manager Assets o Marchi GenStudio nelle seguenti aree di un record Planning:

   * Campi record collegati nella vista tabella di un tipo di record in Planning.
   * Campi record collegati nella pagina di anteprima o dei dettagli di un record.
   * L&#39;anteprima o la pagina dei dettagli del record nella pagina Record collegati di un record.

* È possibile collegare oggetti Workfront ai record di Workfront Planning nelle seguenti aree di Workfront:

   * La sezione Planning di un oggetto Workfront.
   * Campo di connessione Planning nel modulo personalizzato di un oggetto Workfront.

  Per informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

### Connetti automaticamente i record

Dopo aver collegato tipi di record a un altro o un tipo di record a un tipo di oggetto di un&#39;altra applicazione, è possibile connettere automaticamente record e oggetti nei modi seguenti:

* Utilizzo delle automazioni

  È possibile creare record o oggetti Workfront da un record di Planning in cui è possibile configurare le automazioni.

  Quando viene soddisfatta una condizione definita, viene creato un record o un oggetto che viene automaticamente connesso al record da cui si attiva l&#39;automazione.

  Per informazioni, vedere [Configurare le automazioni di Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

* Utilizzo dei moduli di richiesta per creare record

  È possibile creare record quando si sottomette una richiesta Planning. La richiesta e il record vengono collegati automaticamente.

  >[!NOTE]
  >
  >Impossibile disconnettere un record dalla richiesta originale.

  Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

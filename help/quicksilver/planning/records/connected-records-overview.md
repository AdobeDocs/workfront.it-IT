---
title: Panoramica dei record collegati
description: Dopo aver creato connessioni tra tipi di record, è possibile collegare tra loro singoli record. In questo articolo vengono descritte le considerazioni da tenere in considerazione per la connessione dei record in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Panoramica sui record collegati

<!--for the Planning connection field, see commented out below; also add preview tags-->

{{planning-important-intro}}

È possibile collegare tra loro record di Adobe Workfront Planning o a oggetti di altre applicazioni.

In questo articolo vengono descritte le considerazioni da tenere in considerazione per la connessione dei record in Adobe Workfront Planning.

Per informazioni su come connettere i record tra loro o a un altro oggetto, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).


## Considerazioni sulla connessione dei record

* Dopo aver connesso i tipi di record, i tipi di record collegati vengono visualizzati come campi di record collegati nella tabella dei tipi di record da cui sono collegati e nelle pagine dei record.
* È possibile sfogliare e aggiungere record e oggetti dei tipi di record e oggetti collegati dai campi dei record collegati.
* È possibile aggiungere campi (campi di ricerca) dei tipi di record collegati nella tabella del tipo di record da cui si sta effettuando il collegamento.

  È inoltre possibile aggiungere campi (campi di ricerca) dei tipi di record da cui si sta effettuando il collegamento nella tabella del tipo di record a cui si sta effettuando il collegamento.

  Ad esempio, se colleghi il tipo di record Prodotto dal tipo di record Campagna, puoi visualizzare i campi prodotto per le campagne e i campi campagna per i prodotti.
* Non è possibile aggiornare manualmente i valori dei campi di ricerca nei record da cui si sta effettuando il collegamento.

  I valori dei campi di ricerca vengono inseriti automaticamente nel record di Workfront Planning da cui si sta eseguendo il collegamento dopo l&#39;aggiornamento nel record o nell&#39;oggetto originale.

* Tutti coloro che dispongono dell&#39;accesso a Workfront Planning and View o delle autorizzazioni di livello superiore per l&#39;area di lavoro possono visualizzare le connessioni tra record o tra record e oggetti di altre applicazioni. Possono visualizzare i record e gli oggetti connessi indipendentemente dalle autorizzazioni di cui dispongono nelle applicazioni a cui ci si connette.
* Se si dispone delle autorizzazioni di gestione per l&#39;area di lavoro in cui si trovano i record connessi, è possibile visualizzare e modificare le connessioni di tutti gli altri utenti.
* È possibile connettere un record a uno o più oggetti di un&#39;altra applicazione. Per ulteriori informazioni, vedere la sezione &quot;Tipi di connessione&quot; nell&#39;articolo [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Aree in cui è possibile collegare i record

È possibile collegare record ad altri record o a oggetti di un&#39;altra applicazione nelle aree seguenti:

* È possibile collegare record da Workfront Planning a oggetti Workfront o Experience Manager Assets nelle seguenti aree di un record Planning:

   * Campi record collegati nella vista tabella di un tipo di record in Planning.
   * L&#39;anteprima o la pagina del record nei campi del record collegato nella scheda Dettagli.
   * L&#39;anteprima o la pagina del record nella scheda Connessioni.

* È possibile collegare oggetti Workfront ai record di Workfront Planning nelle aree seguenti:

   * Dalla sezione Planning di un oggetto Workfront.
  <!--* From a Planning connection field on a Workfront object's custom form. -->

  Per informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md)
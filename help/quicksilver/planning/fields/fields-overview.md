---
title: Panoramica campo
description: In Adobe Workfront Planning è possibile aggiungere nuovi campi che riflettono il ciclo di vita dell'organizzazione. I campi sono attributi dei tipi di record.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 2%

---


# Panoramica campo

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

In Adobe Workfront Planning è possibile aggiungere nuovi campi che riflettono il ciclo di vita dell&#39;organizzazione. I campi sono attributi dei tipi di record.


## Considerazioni sui campi di Adobe Workfront Planning

* È possibile creare campi solo dalla vista tabella di una pagina del tipo di record. I campi vengono visualizzati come colonne nella vista tabella. Nella pagina del record vengono visualizzati anche tutti i campi associati a un tipo di record.

  Per informazioni sulla gestione delle colonne di tabella (o dei campi record), vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

  Per informazioni sulla gestione dei campi, vedi anche i seguenti articoli:

   * [Modifica impostazioni campo](/help/quicksilver/planning/fields/edit-fields.md)
   * [Elimina campi](/help/quicksilver/planning/fields/delete-fields.md)

* I campi associati a un tipo di record sono disponibili per essere associati a tutti i record di quel tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Impossibile aggiungere campi associati a un tipo di record a un altro tipo di record. <!-- this will change when they open the Field library tab when creating a field-->

* Puoi creare i campi manualmente o automaticamente nei seguenti modi:

   * Manualmente:

      * Quando si aggiungono colonne nella visualizzazione tabella di una pagina del tipo di record. Le colonne della tabella sono i campi associati al tipo di record. Sono gli stessi campi visualizzati nella pagina di un record.

        Impossibile creare campi dalla pagina del record.

      * Quando si collegano tipi di record. È possibile creare campi record collegati quando si aggiunge una nuova connessione tra due tipi di record o un tipo di record e un tipo di oggetto di altre applicazioni.

        Per ulteriori informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Quando importi campi esistenti da Workfront.

        Per informazioni, vedere [Importare campi da Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automaticamente:

      * Quando si crea un tipo di record:

         * Nome
         * Descrizione
         * Data di inizio
         * Data di fine
         * Stato. I valori predefiniti per gli stati dei record sono:
            * Sviluppo
            * Pianificato
            * Attiva
            * Completato
            * In sospeso

        Puoi aggiungere altri valori o rinominare quelli esistenti.

      * Quando crei un’area di lavoro da un modello.

        Per informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Quando si importano tipi di record utilizzando un file Excel o CSV.

        Per ulteriori informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

* I campi di Workfront Planning non sono accessibili da Workfront.

* I campi di Workfront sono accessibili da Workfront Planning solo quando si collegano tipi di record a tipi di oggetti di Workfront e si aggiungono campi collegati o di ricerca da oggetti di Workfront. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

* Se disponi delle autorizzazioni di gestione per l’area di lavoro e il tipo di record a cui appartiene il campo, puoi visualizzare e aggiornare le impostazioni per i campi creati da te o da qualsiasi altro utente.

* È possibile avere fino a 500 campi per un tipo di record.

* I nomi dei campi possono contenere fino a 250 caratteri.

* Durante l’eliminazione di un tipo di record o di un’area di lavoro, vengono eliminati anche tutti i campi ad essi associati e i relativi valori, che non possono essere recuperati. <!-- this might change with a possible recycle bin solution?!-->

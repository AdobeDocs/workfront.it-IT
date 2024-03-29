---
title: Panoramica campo
description: Nella pianificazione di Adobe Workfront puoi aggiungere nuovi campi che riflettono il ciclo di vita della tua organizzazione. I campi sono attributi dei tipi di record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 2%

---

# Panoramica campo

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Nella pianificazione di Adobe Workfront puoi aggiungere nuovi campi che riflettono il ciclo di vita della tua organizzazione. I campi sono attributi dei tipi di record.


## Considerazioni sui campi di pianificazione di Adobe Workfront

* È possibile creare campi solo dalla vista tabella di una pagina del tipo di record. I campi vengono visualizzati come colonne nella vista tabella. Tutti i campi associati a un tipo di record vengono visualizzati anche nella pagina Dettagli di ciascun record di quel tipo.

  Per informazioni sulla gestione delle colonne di tabella (o dei campi record), vedere [Gestire la vista tabella](../views/manage-the-table-view.md).

  Per informazioni sulla gestione dei campi, vedi anche i seguenti articoli:

   * [Modifica campi](../fields/edit-fields.md)
   * [Elimina campi](../fields/delete-fields.md)

* I campi associati a un tipo di record sono disponibili per essere associati a tutti i record di quel tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Impossibile aggiungere campi associati a un tipo di record a un altro tipo di record. <!-- this will change when they open the Field library tab when creating a field-->

* Puoi creare i campi manualmente o automaticamente nei seguenti modi:

   * Manualmente:

      * Aggiungendo colonne nella visualizzazione tabella di una pagina di tipo record. Le colonne della tabella sono i campi associati al tipo di record. Sono gli stessi campi visualizzati nella pagina Dettagli di un record.

        Impossibile creare campi dalla pagina Dettagli di un record.

        Questo articolo descrive come creare manualmente i campi.

      * Collegando i tipi di record. È possibile creare campi record collegati quando si aggiunge una nuova connessione tra due tipi di record o un tipo di record e un tipo di oggetto di altre applicazioni.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Per ulteriori informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](../architecture/connect-record-types.md).

      * Importando i tipi di record utilizzando un file Excel o CSV. Per ulteriori informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

   * Automaticamente:

     Di seguito sono riportati i campi standard creati per impostazione predefinita per ogni nuovo tipo di record:

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

     Quando si crea un&#39;area di lavoro da un modello, in Workfront planning vengono creati campi per i tipi di record. Per informazioni, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

* I campi di pianificazione di Workfront non sono accessibili da Workfront.

* I campi di Workfront sono accessibili da Workfront Planning solo quando si collegano tipi di record a tipi di oggetti di Workfront e si aggiungono campi collegati o di ricerca da oggetti di Workfront. Per informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).

* Se disponi delle autorizzazioni di gestione per l’area di lavoro a cui appartiene il campo, puoi visualizzare e aggiornare le impostazioni per i campi creati da te o da qualsiasi altro utente.

* È possibile avere fino a 500 campi per un tipo di record.

* I nomi dei campi possono contenere fino a 250 caratteri.

* Durante l’eliminazione di un tipo di record o di un’area di lavoro, vengono eliminati anche tutti i campi ad essi associati e i relativi valori, che non possono essere recuperati. <!-- this might change with a possible recycle bin solution?!-->

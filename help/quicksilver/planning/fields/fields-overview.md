---
title: Panoramica campo
description: In Adobe Workfront Planning è possibile aggiungere nuovi campi che riflettono il ciclo di vita dell'organizzazione. I campi sono attributi dei tipi di record.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 8d5006532e93dc687beb79e817b725f18b0c65d3
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 2%

---


# Panoramica campo

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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

      * Aggiungendo colonne nella visualizzazione tabella di una pagina di tipo record. Le colonne della tabella sono i campi associati al tipo di record. Sono gli stessi campi visualizzati nella pagina di un record.

        Impossibile creare campi dalla pagina del record.

      * Collegando i tipi di record. È possibile creare campi record collegati quando si aggiunge una nuova connessione tra due tipi di record o un tipo di record e un tipo di oggetto di altre applicazioni.

        Per ulteriori informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

      * <span class="preview">Importazione di campi esistenti da Workfront. </span>
        <span class="preview">Per informazioni, vedere [Importare campi da Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).</span>

      * <span class="preview">Importando i tipi di record utilizzando un file Excel o CSV. </span>

        <span class="preview">Per ulteriori informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).</span>

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

     Workfront Planning crea campi per i tipi di record quando si crea un&#39;area di lavoro da un modello. Per informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

* I campi di Workfront Planning non sono accessibili da Workfront.

* I campi di Workfront sono accessibili da Workfront Planning solo quando si collegano tipi di record a tipi di oggetti di Workfront e si aggiungono campi collegati o di ricerca da oggetti di Workfront. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

* Se disponi delle autorizzazioni di gestione per l’area di lavoro a cui appartiene il campo, puoi visualizzare e aggiornare le impostazioni per i campi creati da te o da qualsiasi altro utente.

* È possibile avere fino a 500 campi per un tipo di record.

* I nomi dei campi possono contenere fino a 250 caratteri.

* Durante l’eliminazione di un tipo di record o di un’area di lavoro, vengono eliminati anche tutti i campi ad essi associati e i relativi valori, che non possono essere recuperati. <!-- this might change with a possible recycle bin solution?!-->

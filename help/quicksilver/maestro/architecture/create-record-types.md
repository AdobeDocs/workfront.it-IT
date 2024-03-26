---
title: Crea tipi di record
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell'organizzazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '1245'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Crea tipi di record

{{maestro-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi relativi al lavoro necessari per il ciclo di vita dell&#39;organizzazione.
I tipi di record possono essere uno dei seguenti:

Per ulteriori informazioni sui tipi di record, vedere [Panoramica dei tipi di record](../architecture/overview-of-record-types-and-taxonomies.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L’organizzazione deve essere iscritta al programma beta chiuso di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Corrente: Piano</p>
   Oppure
   <p>Nuovo: Standard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per la pianificazione di Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni sulla creazione di tipi di record

* È possibile creare tipi di record in un&#39;area di lavoro nei modi seguenti:

   * Automaticamente:
      * Quando crei un’area di lavoro utilizzando un modello.

        Per informazioni, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

      * Quando vengono importati utilizzando un file Excel o CSV.

        >[!IMPORTANT]
        >
        >Questa funzionalità è stata temporaneamente disabilitata dal 21 marzo 2024. Verrà attivato in un secondo momento.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * Manualmente:

      * Da zero.

        Questo articolo descrive come creare tipi di record generici da zero in un&#39;area di lavoro creata da zero.

* È possibile spostare tipi di record all&#39;interno di una sezione e da una sezione di un&#39;area di lavoro a un&#39;altra. Non è possibile spostare tipi di record da un&#39;area di lavoro a un&#39;altra.

## Creare tipi di record utilizzando un modello di area di lavoro

È possibile creare automaticamente i tipi di record quando si crea un&#39;area di lavoro utilizzando un modello di pianificazione di Workfront. Ogni modello contiene tipi di record di esempio.

Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono raggruppati nelle sezioni seguenti:

* Tipi di record operativi
* Tassonomie

È possibile aggiungere manualmente tipi di record nelle sezioni Tipi di record operativi e Tassonomie.

Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

Per informazioni sui tipi di record inclusi in ogni modello, vedere [Elenco dei modelli di Workspace](../architecture/workspace-templates.md).

## Creare un tipo di record da zero

Questo articolo descrive come creare tipi di record da zero.

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace per il quale si desidera creare i tipi di record.
1. Clic **Aggiungi tipo di record**.
1. (Condizionale) Se si sta creando un tipo di record operativo, fare clic su **Da zero**.

   Viene visualizzata la casella Aggiungi tipo di record.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aggiorna le seguenti informazioni:

   * **Nome tipo di record**: sostituisci &quot;Tipo di record operativo senza titolo&quot; con il nome del tipo di record futuro.
   * **Aspetto**: definisci il colore e la forma dell’icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il nuovo tipo di record. Colore dell&#39;icona del tipo di record. Il grigio è selezionato per impostazione predefinita.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. Fai clic all’esterno del **Aggiungi tipo di record** per salvare il tipo di record.

   La scheda del tipo di record viene aggiunta all&#39;area di lavoro selezionata.
Sulla scheda viene visualizzato il numero di campi contenuti nel tipo di record.
1. (Facoltativo) Fare clic sulla scheda tipo di record per aprire la pagina tipo di record.

   ![](assets/operational-record-type-blank.png)

   Per impostazione predefinita, la pagina del tipo di record viene visualizzata nella vista Tabella. Le colonne della tabella sono campi associati al nuovo tipo di record. Ogni riga è un record univoco da aggiungere.

   Per impostazione predefinita, i campi seguenti vengono visualizzati nelle colonne della vista tabella di un tipo di record operativo:

   * Nome
   * Descrizione
   * Data di inizio
   * Data di fine
   * Stato

1. (Facoltativo) Aggiorna il nome del tipo di record nell’intestazione della pagina

   Oppure

   Fai clic su **Altro** icona ![](assets/more-menu.png) a destra del nome del tipo di record e fare clic su **Rinomina** per rinominarlo.

1. (Facoltativo) Fai clic su **+ Nuovo record** per aggiungere record del tipo di record selezionato. Per ulteriori informazioni, consulta [Crea record](../records/create-records.md).
1. (Facoltativo) Fai clic su **+** nell&#39;angolo superiore destro della tabella per aggiungere altri campi al tipo di record.

   Per ulteriori informazioni sulla creazione dei campi, consulta [Crea campi](../fields/create-fields.md).

1. (Facoltativo) Fare clic sulla freccia rivolta a sinistra a sinistra del nome del tipo di record per tornare all&#39;area di lavoro selezionata.

   Nella scheda del tipo di record viene visualizzato il numero di campi e connessioni contenuti nel tipo di record.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Per ulteriori informazioni sull&#39;aggiunta di record, l&#39;eliminazione o la modifica di tipi di record o l&#39;aggiornamento della visualizzazione nella pagina del tipo di record, vedere gli articoli seguenti:

   * [Crea record](../records/create-records.md)
   * [Elimina tipi di record](../architecture/delete-record-types.md)
   * [Modifica tipi di record](../architecture/edit-record-types.md)
   * [Gestire le visualizzazioni record](../views/manage-record-views.md)

1. (Facoltativo) Dall&#39;area di lavoro, fare clic su per trascinare un tipo di record in un punto desiderato o per spostarlo in un&#39;altra sezione.

   Le modifiche vengono salvate automaticamente dopo che la scheda del tipo di record selezionato è stata eliminata.

## Creare tipi di record importando un file Excel o CSV

>[!IMPORTANT]
>
>Questa funzionalità è stata temporaneamente disabilitata dal 21 marzo 2024. Verrà attivato in un secondo momento.


Quando si importano tipi di record utilizzando un file Excel o CSV, tenere presente quanto segue:

* Ogni foglio del file Excel diventa un tipo di record.
* Le colonne di ciascun foglio diventano i campi associati a ciascun tipo di record.
* I campi sono univoci per i rispettivi tipi di record.
* Ogni riga di ogni foglio diventa un record univoco associato al rispettivo tipo di record.
* Ogni foglio del file Excel non deve superare i seguenti:
   * 50.000 righe
   * 500 colonne
* Il file Excel non deve superare i 5 MB.
* I fogli vuoti non sono supportati.

Per importare i tipi di record utilizzando un file di Excel:

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace per il quale si desidera creare i tipi di record.
1. Clic **Aggiungi tipo di record**.
1. Clic **Excel/CSV**.
1. Trascina e rilascia un file Excel o CSV salvato in precedenza sul computer, oppure fai clic su **Seleziona un file CSV o Excel** per sfogliarne uno.
1. Clic **Verifica i dati**.

   Viene visualizzata la casella Anteprima e modifica con le seguenti informazioni:

   * I nomi dei fogli o dei tipi di record futuri vengono visualizzati nel pannello sinistro. Per impostazione predefinita, Workfront planning seleziona un&#39;icona e un colore per ogni nuovo tipo di record.
   * Il primo foglio o il tipo di record viene selezionato e i nomi dei campi associati vengono visualizzati come intestazioni di colonna. Il tipo di ogni campo è selezionato per impostazione predefinita.
   * Ogni riga rappresenta un nuovo record. Nella casella Anteprima e modifica vengono visualizzati solo i primi 10 record.

   ![](assets/preview-and-edit-box.png)

1. (Facoltativo) Fate clic sul nome di ciascun foglio nel pannello a sinistra per esaminare le informazioni in esso contenute.

   >[!NOTE]
   >
   >    I fogli vuoti non sono supportati e sono oscurati.


1. (Facoltativo) Fai clic su **Seleziona i fogli da importare** e deselezionare i fogli da non importare.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   I fogli deselezionati vengono visualizzati con uno sfondo grigio.

1. Clic **Importa** quando sei pronto per importare il file.

   Le informazioni seguenti vengono importate in Workfront Planning:

   * Nuovi tipi di record
   * Nuovi campi associati a ciascun tipo di record
   * Nuovi record associati a ciascun tipo di record

   È possibile iniziare a gestire campi e record nelle pagine dei tipi di record.

   Tutti coloro che hanno accesso alla pianificazione di Workfront ora possono visualizzare e modificare i tipi di record importati e le relative informazioni. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->
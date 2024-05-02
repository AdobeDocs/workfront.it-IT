---
title: Crea record
description: Quando si utilizza Adobe Workfront Planning, un record è un'istanza di un tipo di record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Crea record

{{maestro-important-intro}}

In Adobe Workfront Planning, un record è un&#39;istanza di un tipo di record.

È possibile creare record eseguendo una delle operazioni seguenti:

* Crearli manualmente per i tipi di record
* Creare record copiando e incollando informazioni da un elenco esterno.

In questo articolo viene descritto come creare record. Per informazioni sulla gestione dei record nelle viste tabella o sequenza temporale, vedere gli articoli seguenti:

* [Gestire la vista tabella](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Gestire la visualizzazione della timeline](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Creare record aggiungendoli manualmente a un tipo di record <!--in a record type table (I don't think you can create them elsewhere right now)-->

È possibile creare record nella vista tabella di una pagina del tipo di record.

Per informazioni sulla modifica delle informazioni sui record, vedere [Modifica record](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso. Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.
Tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. (Condizionale) Se la pagina del tipo di record non si apre nella visualizzazione tabella, fare clic sulla scheda di una visualizzazione tabella oppure fare clic su **+ Visualizza** per creare una vista tabella.

1. Per aggiungere nuovi record, fare clic su **Nuovo record** nell’ultima riga della tabella

   Oppure

   Clic **Maiusc + Invio** sulla tastiera da qualsiasi colonna o riga della tabella. Viene aggiunta una riga vuota.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Iniziare a digitare informazioni sul nuovo record nella nuova riga.

   >[!NOTE]
   >
   >  * Non esistono campi obbligatori per i record. È tuttavia consigliabile aggiungere un nome per il record, in quanto è utile identificare i record quando si collegano tra loro record.
   >
   >  * I campi che fanno riferimento ad altri tipi di record o campi calcolati sono campi di sola lettura.

1. Continua ad aggiungere informazioni su ogni riga, quindi fai clic su **Invio** sulla tastiera per salvare le modifiche.

   Oppure

   Fare clic sul nome del nuovo record o sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome del record. Nella tabella viene visualizzata un&#39;anteprima con le informazioni dettagliate del record.

   >[!TIP]
   >
   >È possibile accedere a **Apri dettagli** solo dal campo del nome del record quando il campo del nome è un campo primario.

1. Iniziare a modificare le informazioni del record nell&#39;anteprima del record. Workfront salva automaticamente le modifiche.
1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda. Continuare a modificare il record nella pagina record.


1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere l&#39;aggiunta di nuovi record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Creare record copiando e incollando informazioni da un elenco esterno

1. Iniziare a creare record nella vista Tabella, come descritto nella sezione [Creare record aggiungendoli manualmente a un tipo di record](#create-records-by-manually-adding-them-to-a-record-type) in questo articolo.

   Verificare che nella vista tabella siano presenti le colonne o i campi che si desidera compilare con le nuove informazioni del record.

1. Clic **Nuovo &lt; Nome tipo di record >** nell&#39;ultima riga della tabella per aggiungere alla tabella tutte le nuove righe che si desidera aggiungere ai nuovi record.

   Aggiungere ad esempio 10 righe alla vista tabella se si desidera incollare le informazioni relative a 10 nuovi record da un&#39;altra applicazione.

1. In un&#39;altra applicazione creare un elenco di record che si desidera importare.

   Ad esempio, puoi utilizzare un foglio di calcolo Excel per creare l’elenco.

   L’elenco deve contenere informazioni in formato tabulare.

   >[!TIP]
   >
   > Le colonne dell’elenco devono contenere informazioni relative ai campi esistenti in Workfront.
   >
   > Assicurati di avere già creato i campi desiderati in Workfront e che le informazioni nel foglio siano visualizzate nel formato corretto che corrisponde a quello di ciascun campo in Workfront.

1. In un&#39;altra applicazione, selezionare più righe e colonne, quindi incollare le informazioni nella vista tabella del tipo di record, a partire dal primo nuovo record.

   Nell&#39;area Workfront Planning vengono importate le seguenti informazioni:

   * Le righe contengono i nuovi record
   * Nelle colonne vengono inserite le informazioni relative ai campi dei record.

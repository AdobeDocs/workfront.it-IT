---
title: Crea record
description: In Adobe Maestro, un record è un'istanza di un tipo di record. È necessario creare tipi di record prima di creare singoli record. La creazione di record di tassonomia è identica alla creazione di record operativi.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1105'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Crea record

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

In Adobe Maestro, un record è un&#39;istanza di un tipo di record.

È possibile disporre dei seguenti tipi di record:

* **Record operativi**: rappresentano oggetti correlati al lavoro. Ad esempio, per un record operativo denominato &quot;Campaign&quot;, è possibile denominare record come &quot;Monthly Newsletter&quot; o &quot;Summer Sale&quot;.
* **Record di tassonomia**: rappresentano attributi che possono essere associati a record operativi. Ad esempio, per un tipo di record di tassonomia denominato &quot;Canale&quot;, è possibile denominare tassonomie come &quot;E-mail&quot;, &quot;Social Media&quot; o &quot;Advertising&quot;.

La creazione di record operativi è identica alla creazione di record di tassonomia.

È possibile creare record in Maestro eseguendo una delle operazioni seguenti:

* Creali manualmente per i tipi di record Maestro
* Collegali ai record Maestro da applicazioni di terze parti.
* Creare record copiando e incollando informazioni da un elenco esterno.

Questo articolo descrive come creare i record Maestro. Per informazioni sulla gestione dei record nelle viste tabella o sequenza temporale, vedere gli articoli seguenti:

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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td> <p>Non ci sono controlli di accesso per Maestro </p>  
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
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
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

1. (Condizionale) Se la pagina del tipo di record non si apre nella vista a tabella, fare clic sul pulsante **Visualizza** e selezionare un menu a discesa esistente **Vista tabella** ![](assets/table-view-icon.png) o fai clic su **Crea vista > Tabella** per creare una vista tabella.

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

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere l&#39;aggiunta di nuovi record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica

## Creare record collegandoli da un&#39;altra applicazione

Puoi importare record da altre applicazioni collegandoli a record collegati Maestro. In questo modo viene creato un tipo di record Maestro per l&#39;oggetto connesso dell&#39;applicazione di terze parti. I record collegati ai record Maestro originali vengono visualizzati nella vista della tabella del tipo di record Maestro dell&#39;oggetto collegato a un&#39;applicazione di terze parti.

1. Creare un tipo di record Maestro, come descritto in [Crea tipi di record](../architecture/create-record-types.md).

1. Crea record Maestro per il tipo di record creato nel passaggio precedente. Per informazioni, consulta la sezione [Creare record aggiungendoli manualmente a un tipo di record](#create-records-by-manually-adding-them-to-a-record-type) in questo articolo.

1. Creare una connessione a un tipo di oggetto da un&#39;applicazione di terze parti per il tipo di record Maestro creato. Per informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).

1. Aggiungi i record dell&#39;applicazione di terze parti ai record Maestro creati in precedenza utilizzando il campo record collegato creato nel passaggio precedente. Per informazioni, consulta [Collega record](../records/connect-records.md).

   I seguenti elementi sono creati in Maestro:

   * Tipo di record Maestro di sola lettura che fa riferimento al tipo di record di terze parti a cui è stato effettuato il collegamento nel campo record connesso.

     Ad esempio, se si collega un tipo di record Maestro a progetti Workfront, nella stessa area di lavoro viene creato un tipo di record di sola lettura denominato &quot;progetti Workfront&quot;.
   * Record di sola lettura nella pagina del tipo di record di terze parti. I record importati dall&#39;applicazione di terze parti rimangono di sola lettura e possono essere aggiornati solo nell&#39;applicazione originale.

## Creare record copiando e incollando informazioni da un elenco esterno

1. In Maestro, inizia a creare record nella vista Tabella, come descritto nella sezione [Creare record aggiungendoli manualmente a un tipo di record](#create-records-by-manually-adding-them-to-a-record-type) in questo articolo.

   Assicurarsi che la vista tabella Maestro contenga le colonne (o i campi) che si desidera compilare con le nuove informazioni del record.

1. Clic **Nuovo &lt; Nome tipo di record >** nell&#39;ultima riga della tabella per aggiungere alla tabella tutte le nuove righe che si desidera aggiungere ai nuovi record.

   Aggiungere ad esempio 10 righe alla vista tabella se si desidera incollare le informazioni relative a 10 nuovi record da un&#39;altra applicazione.

1. In un&#39;altra applicazione, creare un elenco di record che si desidera importare in Maestro.

   Ad esempio, puoi utilizzare un foglio di calcolo Excel per creare l’elenco.

   L’elenco deve contenere informazioni in formato tabulare.

   >[!TIP]
   >
   > Le colonne dell’elenco devono contenere informazioni relative ai campi esistenti in Maestro.
   >
   > Assicurati di avere già creato i campi desiderati in Maestro e che le informazioni nel tuo foglio siano visualizzate nel formato corretto che corrisponde a quello di ciascun campo in Maestro.

1. Dall&#39;applicazione di terze parti selezionare più righe e colonne, quindi incollare le informazioni nella vista tabella del tipo di record, a partire dal primo nuovo record.

   Le seguenti informazioni sono importate in Maestro:

   * Le righe contengono i nuovi record
   * Nelle colonne vengono inserite le informazioni relative ai campi dei record.

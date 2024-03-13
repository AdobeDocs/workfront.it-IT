---
title: Modifica record
description: È possibile modificare le informazioni del record nelle funzionalità di pianificazione di Adobe Workfront. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifica record

{{maestro-important-intro}}

È possibile modificare le informazioni sui record nelle funzionalità di pianificazione di Adobe Workfront modificando i valori dei campi associati ai record.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

Per informazioni sulla creazione di record, vedere [Crea record](/help/quicksilver/maestro/records/create-records.md).

&lt;!— menziona qui che i campi nella visualizzazione Dettagli sono gli stessi di quelli nella visualizzazione tabella — questo articolo è collegato da Gestisci visualizzazioni record uno per fare riferimento a queste informazioni—>

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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso delle funzionalità di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Chiaro o superiore</p>
   Oppure
   <p>Corrente: Lavoro o versione successiva</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Non sono presenti controlli di accesso per le funzionalità di pianificazione di Adobe Workfront </p>  
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

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerazioni sulla modifica dei record

* Se si dispone delle autorizzazioni necessarie per l&#39;area di lavoro, è possibile modificare i record creati o quelli creati da altri utenti.
* È possibile modificare i campi record dalla pagina Dettagli di un record o dalla visualizzazione tabella di un tipo di record.
* Non è possibile modificare le informazioni del record dalla vista timeline.
* I seguenti tipi di campi vengono aggiornati automaticamente e non è possibile modificarne i valori manualmente:
   * Campi collegati da altri record
   * Campi di tipo formula
   * Campi di sistema (Creato da, Data di creazione, Autore ultima modifica, Data ultima modifica)
* Se i record visualizzati sono collegati ad altri record, le nuove informazioni dei record che si sta modificando verranno applicate ai record collegati.
* Non è possibile modificare i record in blocco. <!--this will probably change-->
* Gli URL vengono riconosciuti come collegamenti nei tipi di campi di testo a riga singola solo quando iniziano con: http://, https://, ftp:// o www. .

## Modifica record

È possibile modificare un record dalle seguenti aree:

* [Dalla vista tabella di un tipo di record](#edit-a-record-from-the-table-view-of-a-record-type)
* [Dalla pagina Dettagli di un record](#edit-a-record-from-the-records-details-page)

### Modificare un record dalla vista tabella di un tipo di record

{#step1-to-maestro}

Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Da **Visualizza** menu a discesa nell&#39;angolo superiore sinistro della tabella, selezionare un **Tabella** visualizzazione. Questa dovrebbe essere la visualizzazione predefinita, a meno che il tipo di record non sia stato visualizzato in un altro tipo di visualizzazione al momento dell&#39;ultimo accesso.

<!--replace above with this when we release view redesign: (Conditional) Click the tab of a table view or click **+ View** to create a table view. The table view should be the default view, unless you viewed the record type in another type of view when you accessed it last. -->

    I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic all&#39;interno della riga di un record per iniziare a modificare le informazioni sul record in linea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo e condizionale) Quando si modifica un campo di tipo Paragrafo, utilizzare quanto segue **Rich Text** opzioni di formattazione:

   * Bold
   * Italic
   * Sottolinea
   * Aggiungi un collegamento
   * Aggiungere un elenco puntato
   * Aggiungere un elenco numerato

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Facoltativo) Fare doppio clic su un campo record connesso per aggiungere record o oggetti connessi a un altro record. Per ulteriori informazioni, consulta [Collega record](/help/quicksilver/maestro/records/connect-records.md).
1. Premi **Invio** sulla tastiera o fare clic all&#39;esterno di una riga per salvare le modifiche. Le modifiche vengono salvate automaticamente. A **Salvato** viene visualizzato brevemente nell&#39;angolo superiore destro della vista tabella per indicare che le modifiche sono state salvate.


   <!--
    1. (Optional) Click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of a record name, or click a record name. The **Details** box opens in the table. 
        >[!TIP]
        >
        >    You can view the Open details icon to the left of the Name field of a record only when the Name field is a primary field. 
    1. Start editing the field information in the Details box. Workfront automatically saves your changes. 
    1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) (*********check the icon; they are changing it***********) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record as described in [Edit a record from the record's Details page](#edit-a-record-from-the-records-details-page) section in this article. 
    -->

1. (Facoltativo) Per copiare e incollare informazioni da un campo all&#39;altro, effettuare una delle seguenti operazioni:

   * Copiare uno o più valori esistenti di un campo, quindi incollarli in un campo dello stesso tipo in un altro record
   * Fare clic sull&#39;intestazione di una colonna per selezionarla e copiarla, quindi fare clic sull&#39;intestazione di un&#39;altra colonna e incollare il contenuto della colonna copiata. Le colonne devono contenere tipi di campo simili.
   * Con il tasto Maiusc premuto, fai clic su per selezionare più righe in una tabella, copia le informazioni nelle righe selezionate, quindi fai clic su una riga diversa e incolla le informazioni selezionate nella nuova riga e nelle righe successive.

   >[!NOTE]
   >
   >Considera quanto segue:
   >
   >* Utilizza le seguenti scelte rapide da tastiera per copiare e incollare le informazioni:
   >   * Copia: CTRL + C (⌘ + C per Mac)
   >   * Incolla: CTRL + V (⌘ + V per Mac)
   >* Non è possibile copiare informazioni da un&#39;altra origine, ad eccezione di un campo record dello stesso tipo del campo in cui si incollano le informazioni.
   >
   >* Non è possibile copiare e incollare i valori dei campi nell&#39;area Dettagli di un record. Questa funzionalità è supportata solo nella vista tabella di un tipo di record.
   >* Non è possibile copiare e incollare valori di campo per i tipi di campo seguenti:
   >
   >
   >    * Campi collegati creati mediante la connessione di tipi di record. È possibile copiare e incollare campi record collegati. Per ulteriori informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).
   >    * Campi dei seguenti tipi: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere la modifica o la copia e l&#39;incollamento delle informazioni del record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica

   >[!TIP]
   >
   >    È possibile utilizzare più volte le scelte rapide da tastiera in una riga per annullare più modifiche.

1. (Facoltativo) Aggiungi una miniatura a un record. Per informazioni, consulta [Aggiungere una miniatura a un record](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).


### Modificare un record dalla pagina Dettagli del record

<!--You can edit a record from the Details box in a table view, or from the Details page. For information about editing records in the Details box, see the [Edit a record from the table view of a record type](#edit-a-record-from-the-table-view-of-a-record-type) section in this article.-->

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Esegui una delle operazioni seguenti:

   * Da un **Tabella** visualizzazione, fare clic sul nome di un record.
   * Dalla sezione **Tabella** , passa il puntatore sul nome di un record, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Il record **Dettagli** viene visualizzata la pagina.

1. Fai clic su **Altro** menu ![](assets/more-menu.png) a destra del nome del record, quindi fare clic su **Modifica**

   Oppure

   Fare clic all&#39;interno di un campo modificabile nella pagina Dettagli per modificare le informazioni. <!--Your changes are saved automatically.-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clic **Salva modifiche**. <!--Eliminate this step when we release the new Details box in the table with the Details page. Add above that the saves are automatic-->
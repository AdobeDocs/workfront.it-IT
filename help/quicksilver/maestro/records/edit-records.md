---
title: Modifica record
description: Puoi modificare le informazioni dei record in Adobe Maestro. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifica record

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Puoi modificare le informazioni dei record in Adobe Maestro. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

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

## Considerazioni sulla modifica dei record

* È possibile modificare i record creati dall&#39;utente corrente o da un altro utente. <!--will change with access levels-->
* Non è possibile modificare i campi collegati da altri record o campi che contengono calcoli.
* Se i record visualizzati sono collegati ad altri record, le nuove informazioni dei record che si sta modificando verranno applicate ai record collegati.
* Non è possibile modificare i record in blocco. <!--this will probably change-->
* Gli URL vengono riconosciuti come collegamenti nei tipi di campi di testo a riga singola solo quando iniziano con: http://, https://, ftp:// o www. .
* Durante la modifica di un campo di tipo Paragrafo, è possibile utilizzare le seguenti opzioni di formattazione Rich Text:

   * Bold
   * Italic
   * Sottolinea
   * Aggiungi un collegamento
   * Aggiungere un elenco puntato
   * Aggiungere un elenco numerato

## Modifica record

È possibile modificare un record dalle seguenti aree:

* [Dalla pagina Dettagli di un record](#edit-a-record-from-the-records-details-page)
* [Dalla vista tabella di un tipo di record](#edit-a-record-from-the-record-type-table-view)

### Modificare un record dalla pagina Dettagli del record

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Esegui una delle operazioni seguenti:

   * In una visualizzazione Tabella fare clic sul nome di un record.
   * Nella visualizzazione Tabella, posizionare il puntatore del mouse sul nome di un record, quindi fare clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Il record **Dettagli** viene visualizzata la pagina.

1. Fai clic su **Altro** menu ![](assets/more-menu.png) a destra del nome del record, quindi fare clic su **Modifica**

   Oppure

   Fare clic all&#39;interno di un campo modificabile nella pagina Dettagli per modificare le informazioni.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clic **Salva modifiche**. <!--logged a bug for this - this needs to be "Save"-->

### Modificare un record dalla vista tabella di un tipo di record

{#step1-to-maestro}

Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Da **Visualizza** menu a discesa nell&#39;angolo superiore destro della tabella, selezionare un **Tabella** visualizzazione. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic all&#39;interno della riga di un record per iniziare a modificare le informazioni sul record in linea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Premi **Invio** sulla tastiera o fare clic all&#39;esterno di una riga per salvare le modifiche. Le modifiche vengono salvate automaticamente. Un indicatore Saved (Salvato) viene visualizzato brevemente nell&#39;angolo superiore destro della vista tabella per indicare che le modifiche sono state salvate.

   >[!NOTE]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).
   >  * Campi dei seguenti tipi: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica


1. (Facoltativo) Copiare uno o più valori esistenti di un campo, quindi incollarli in un campo dello stesso tipo in un altro record, quindi fare clic su **Invio** sulla tastiera per salvare le modifiche.

   >[!NOTE]
   >
   >Considera quanto segue:
   >
   >* Non è possibile copiare informazioni da un&#39;altra origine, ad eccezione di un campo Maestro dello stesso tipo del campo in cui si incollano le informazioni.
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
---
title: Modifica record
description: Puoi modificare le informazioni dei record in Adobe Maestro. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

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
 <tbody>
<td>
   <p> prodotto Adobe</p> </td>
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
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

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

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o **Menu principale** ![](assets/main-menu-shell.png) nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro** ![](assets/maestro-icon.png).

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


   <!--take People out of the list above when they release this - this might be coming later-->

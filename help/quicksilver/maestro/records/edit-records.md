---
title: Modifica record
description: Puoi modificare le informazioni dei record in Adobe Maestro. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifica record

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Puoi modificare le informazioni dei record in Adobe Maestro. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
Per informazioni, consulta [Crea tipi di record](../architecture-and-fields/create-record-types.md).

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
* Se i record modificati sono collegati ad altri record, le nuove informazioni dei record che si sta modificando verranno applicate ai record collegati.
* Non è possibile modificare i record in blocco. <!--this will probably change-->
* Non è possibile modificare i campi collegati da altri record.

## Modifica record

È possibile modificare un record dalle seguenti aree:

* [Dalla pagina Dettagli di un record](#edit-a-record-from-the-records-details-page)
* [Dalla vista tabella di un tipo di record](#edit-a-record-from-the-record-type-table-view)

### Modificare un record dalla pagina Dettagli del record

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o **Menu principale** ![](assets/main-menu-shell.png) nell’angolo in alto a sinistra, se è disponibile, fai clic su Maestro.

   Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.
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

   >[!NOTE]
   >
   >    I campi collegati o che contengono calcoli o sono generati dal sistema non sono modificabili.


1. Clic **Salva modifiche**. <!--logged a bug for this - this needs to be "Save"-->

### Modificare un record dalla vista tabella del tipo di record

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) in alto a destra, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> quindi fai clic su **Maestro** ![](assets/maestro-icon.png).

   Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Da **Visualizza** nell&#39;angolo superiore destro della tabella, selezionare una vista Tabella. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic all&#39;interno della riga di un record per iniziare a modificare le informazioni sul record in linea, quindi premere **Invio** sulla tastiera per salvare le modifiche. Le modifiche vengono salvate automaticamente.

   >[!TIP]
   >
   >* I campi collegati non sono modificabili. Le informazioni per questi campi vengono compilate automaticamente dai record collegati. Per informazioni, consulta [Connetti tipi di record](../architecture-and-fields/connect-record-types.md).
   >
   >* Gli URL vengono riconosciuti come collegamenti nei tipi di campi di testo a riga singola solo quando iniziano con: http://, https://, ftp:// o www. .
<!--for rich text formatting - when released:

1. (Conditional) When you edit a Paragraph-type field, use the following Rich Text formatting capabilities: 

    * Bold
    * Italic
    * Underline (*****anything else?? insert a screen shot?***********)
-->
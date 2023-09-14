---
title: Elimina record
description: È possibile eliminare i record creati dall'utente corrente o da un altro utente. Non è possibile recuperare i record eliminati.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Elimina record

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Puoi eliminare i record che non sono più rilevanti in Adobe Maestro.

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

## Considerazioni sull&#39;eliminazione di record

* È possibile eliminare i record creati dall&#39;utente corrente o da un altro utente.
* Non è possibile recuperare i record eliminati. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Se i record eliminati sono collegati ad altri record, i record collegati non vengono eliminati, ma vengono eliminate anche le informazioni del record eliminato.
* Non è possibile eliminare i record in blocco. <!--this will probably change-->
* Non è possibile eliminare record dalla visualizzazione timeline.

## Elimina record

È possibile eliminare un record dalle seguenti aree:

* [Dalla pagina Dettagli di un record](#delete-a-record-from-the-records-details-page)
* [Dalla vista tabella di un tipo di record](#delete-a-record-from-the-record-type-table-view)

### Eliminare un record dalla pagina Dettagli del record

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o **Menu principale** ![](assets/main-menu-shell.png) nell’angolo in alto a sinistra, se è disponibile, fai clic su Maestro.

   Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.
1. Selezionare un tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. Esegui una delle operazioni seguenti:

   * In una visualizzazione Tabella fare clic sul nome di un record.
   * Nella visualizzazione Tabella, posizionare il puntatore del mouse sul nome di un record, quindi fare clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Il record **Dettagli** viene visualizzata la pagina.

1. Fai clic su **Altro** menu ![](assets/more-menu.png) a destra del nome del record, quindi fare clic su **Elimina**, quindi **Elimina** di nuovo per confermare.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Il record viene eliminato e non può essere recuperato.

### Eliminare un record dalla vista tabella del tipo di record

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o **Menu principale** ![](assets/main-menu-shell.png) nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro**.

   Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.
1. Selezionare un tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Da **Visualizza** nell&#39;angolo superiore destro della tabella, selezionare una vista Tabella. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic con il pulsante destro del mouse su una riga di record, quindi scegliere **Elimina**.

   ![](assets/contextual-menu-for-record-row.png)

   Il record viene eliminato e non può essere recuperato.

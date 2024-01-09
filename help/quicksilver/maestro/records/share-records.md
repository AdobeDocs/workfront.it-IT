---
title: Condividere i record
description: È possibile condividere i record con altri utenti per aumentare la collaborazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Condividere i record

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Per collaborare con altri utenti, è possibile condividere i record con altri utenti.

Puoi condividere un record Maestro nei seguenti modi:

* Copiare il collegamento della pagina Dettagli di un record dal browser quando la pagina è aperta.

* Copiare un collegamento nella pagina Dettagli del record quando si visualizzano i record nella visualizzazione tabella del tipo di record.

<!-- Update with this when we release permissions: 

* You can share all records in a workspace with other users by sharing the workspace. For more information, see [Grant access to Adobe Maestro](../access/grant-access.md).
-->

In questo articolo viene descritto come copiare un collegamento alla pagina Dettagli di un record dalla vista tabella di un tipo di record.

<!-- add information about permissions, like:
- in the table below, you must have at least View permissions to the record
- the user you're sharing with must have at least View permissions to the record to view it
- etc - others???-->

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
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with - below
****AND - see more above, another bullet point to update when permissions are released****

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
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
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

## Condividere i collegamenti ai record dalla vista tabella del tipo di record

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o **Menu principale** ![](assets/main-menu-shell.png) nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro**.

   Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Da **Visualizza** nell&#39;angolo superiore destro della tabella, selezionare una vista tabella. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic con il pulsante destro del mouse su una riga di record

   Oppure

   Passa il puntatore del mouse sul nome di un record e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Copia collegamento**.

   ![](assets/contextual-menu-for-record-row.png)

   Il collegamento viene copiato negli Appunti.

1. Incolla il collegamento in un’e-mail o in una finestra di chat per condividerlo con altri utenti. Quando gli utenti ricevono il collegamento, viene aperta la pagina Dettagli del record.

   >[!TIP]
   >
   >I campi del record nella pagina Dettagli sono gli stessi campi disponibili nella visualizzazione Tabella del record.


   <!--add there when it will be available: if they have access to this record-->

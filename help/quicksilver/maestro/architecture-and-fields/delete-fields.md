---
title: Elimina campi
description: Ad Adobe, Maestro, puoi eliminare i campi personalizzati che non sono più rilevanti.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Elimina campi

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro che è una nuova offerta di Adobe.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Ad Adobe, Maestro, puoi creare campi personalizzati per memorizzare informazioni sui record.

Per informazioni sulla creazione di campi personalizzati in Maestro, consulta [Crea campi](../architecture-and-fields/create-fields.md).

Puoi eliminare i campi Maestro che non sono più rilevanti.

## Considerazioni sull’eliminazione dei campi Maestro:

* Puoi eliminare i campi creati o quelli creati da altri utenti. <!--this will change with access levels/ permissions-->
* È possibile eliminare un campo solo nella tabella del tipo di record.
* Tutte le informazioni memorizzate nel campo vengono eliminate e non possono essere recuperate.
* Quando si elimina un campo record collegato, vengono eliminati anche tutti i campi di ricerca collegati dal tipo di record da cui si esegue il collegamento. I campi record collegati dei tipi di record a cui si effettua il collegamento non vengono eliminati.

  Per ulteriori informazioni, consulta [Connetti tipi di record](../architecture-and-fields/connect-record-types.md).
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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

## Elimina campi

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Fai clic su **Menu principale** icona ![](assets/main-menu-workfront.png) nell’angolo superiore destro di Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> quindi fai clic su **Maestro** ![](assets/maestro-icon.png).

   Si apre l’ultimo spazio di lavoro a cui si è avuto accesso in Maestro.
1. Fare clic sulla scheda di un tipo di record di cui si desidera eliminare i campi.
1. (Condizionale) Seleziona un **Vista tabella** dal **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.
1. Individuare il campo da eliminare nelle intestazioni di colonna, posizionare il puntatore del mouse sull&#39;intestazione di colonna e fare clic sulla freccia rivolta verso il basso dopo il nome del campo.
1. Clic **Elimina**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clic **Elimina** per confermare.

   Il campo viene eliminato, non può essere recuperato e non può più essere associato ad alcun record.

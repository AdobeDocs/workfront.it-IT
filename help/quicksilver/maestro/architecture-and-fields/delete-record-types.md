---
title: Elimina tipi di record
description: È possibile eliminare i tipi di record operativi o i tipi di record della tassonomia quando non sono più rilevanti.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Elimina tipi di record

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta chiuso aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

È possibile eliminare i tipi di record operativi o i tipi di record della tassonomia quando non sono più rilevanti.

Per informazioni sui tipi di record e sulle tassonomie, vedere [Panoramica dei tipi di record e delle tassonomie](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

È consigliabile ricreare i campi e i record associati al tipo di record o alla tassonomia che si desidera eliminare in un altro tipo di record prima di eliminarli.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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

## Considerazioni durante l’eliminazione dei tipi di record

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* È possibile eliminare qualsiasi tipo di record o tassonomia creata dall&#39;utente o da altri utenti dell&#39;organizzazione. <!--this will change with access levels and permissions-->
* L&#39;eliminazione dei tipi di record comporta la rimozione di tutte le informazioni ad essi associate, inclusi i campi e i record di quel tipo.
* Non è possibile recuperare i tipi di record eliminati o le relative informazioni.

## Elimina tipi di record

L&#39;eliminazione dei tipi di record della tassonomia è identica all&#39;eliminazione dei tipi di record operativi.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-workfront.png) nell’angolo superiore destro di Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> quindi fai clic su **Maestro** ![](assets/maestro-icon.png).

   Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace per il quale si desidera eliminare i tipi di record.

   Verrà aperto il workspace e verranno visualizzati i tipi di record e le tassonomie ad esso associati.
1. Fare clic sulla scheda relativa al tipo di record o alla tassonomia che si desidera eliminare.

   Verrà aperta la pagina del tipo di record.
1. Fai clic su **Altro** menu ![](assets/more-menu.png) a destra del nome del tipo di record, quindi fare clic su **Elimina**.
1. Clic **Elimina** per confermare.

   Il tipo di record o la tassonomia selezionati, insieme ai relativi campi e record associati, vengono eliminati.
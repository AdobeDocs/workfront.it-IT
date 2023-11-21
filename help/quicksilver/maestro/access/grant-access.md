---
title: Concedere l’accesso a Adobe Maestro
description: Scopri come concedere l’accesso e condividere le informazioni in Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Concedere l’accesso a Adobe Maestro

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per poter accedere a Maestro devi essere un cliente Workfront
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Tutti gli utenti dell’organizzazione possono accedere a Maestro se sono presenti i seguenti prerequisiti:

<!--the first requisite will be removed when we go to GA-->

* La tua organizzazione è iscritta al programma beta chiuso Adobe Maestro.
* In qualità di amministratore di sistema, devi aggiungere l’area Maestro al menu principale utilizzando un modello di layout.

  Maestro non viene visualizzato nel menu principale per impostazione predefinita per qualsiasi utente, inclusi gli amministratori di sistema.

  Per informazioni, consulta [Personalizzare il menu principale utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Non ci sono livelli di accesso o autorizzazioni associati agli utenti o alle informazioni in Maestro. Tutti gli utenti che hanno Maestro abilitato nel loro ambiente possono visualizzare, modificare ed eliminare tutte le informazioni che qualsiasi altro utente aggiunge a Maestro.

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
   <td role="rowheader"><p>Livello di accesso</p></td>
   <td> <p>Qualsiasi da utilizzare Maestro</p>
   <p>Amministratore di sistema o piano per condividere l’area Maestro in un modello di layout</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro al modello di layout. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

## Condividi l’area Maestro nel menu principale con altri

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Dopo che la tua organizzazione è stata iscritta al programma beta Maestro, puoi aggiungere l’area Maestro al menu principale di tutti gli utenti utilizzando un modello di layout.

1. Accedi a **Workfront** come amministratore di Workfront.

1. Aggiungi il **Maestro** icona ![](assets/maestro-icon.png) al **Menu principale** utilizzando un **Modello di layout**.

   Per informazioni, consulta [Personalizzare il menu principale utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Assegna il modello di layout agli utenti che desideri possano accedere a Maestro.

   Per informazioni, consulta [Assegnare utenti a un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Tutti gli utenti assegnati al modello ora possono accedere a Maestro nel loro menu principale.

   Gli utenti possono iniziare a creare workspace, tipi di record, record e campi.

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->
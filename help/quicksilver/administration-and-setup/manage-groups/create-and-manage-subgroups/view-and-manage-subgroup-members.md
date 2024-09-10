---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visualizzare e gestire i membri del sottogruppo
description: Quando visualizzi un gruppo che gestisci, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Visualizzare e gestire i membri del sottogruppo

Quando visualizzi un gruppo che gestisci, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. </li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-settings.png">. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e gestire i membri dei sottogruppi in un gruppo

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo per il quale si desidera visualizzare o gestire i membri del sottogruppo.
1. Nel pannello a sinistra, fai clic su **Membri del sottogruppo**.

   Questo elemento del pannello a sinistra è disponibile solo se il gruppo ha dei sottogruppi.

1. Effettua una delle seguenti operazioni:

   * Selezionare un membro nell&#39;elenco, quindi fare clic su Modifica ![](assets/edit-icon.png) per modificare il profilo utente di tale persona.

     Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) o [Modificare i profili utente in blocco](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Selezionare un numero qualsiasi di membri nell&#39;elenco, quindi fare clic su Aggiorna ![](assets/comment-icon.png) per aggiungere un commento ai profili utente.

     L’utente o gli utenti ricevono una notifica in-app e una notifica e-mail con il commento. Il commento viene visualizzato nell’area Aggiornamenti del profilo dell’utente.

   * Selezionare un numero qualsiasi di membri nell&#39;elenco, quindi fare clic su Disattiva ![](assets/deactivate-user.png) o Attiva ![](assets/activate-user.png).

     Per ulteriori informazioni, vedere [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Esporta ![](assets/export.png) l&#39;elenco dei membri.

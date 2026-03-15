---
user-type: administrator
product-area: system-administration
keywords: modifica,e-mail,notifica,impostazioni,in blocco,modifica in blocco,configura,multipli,utenti
navigation-topic: emails-administration
title: Modifica delle impostazioni di notifica e-mail per più utenti
description: Questo articolo fornisce informazioni agli amministratori di Workfront o di gruppi su come aggiornare le notifiche e-mail di altri utenti.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 6%

---

# Modificare le impostazioni delle notifiche e-mail di più utenti

<!-- Audited: 12/2023 -->

Se sei un amministratore di Adobe Workfront o disponi di un livello di accesso Planner che ti consente di modificare le impostazioni di altri utenti, puoi configurare le impostazioni di notifica per più utenti alla volta. Ciò include l&#39;indicazione se gli utenti ricevono le notifiche quando si verificano eventi o in un&#39;e-mail di riepilogo giornaliera, come descritto nelle [notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Per informazioni sul livello di accesso necessario per modificare gli utenti, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Puoi anche configurare le notifiche e-mail per un utente alla volta, incluso il tuo profilo. Per ulteriori informazioni, vedere [Modifica delle notifiche e-mail personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
    <p>Standard</p>
    <p>Piano</p>
   </td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare le impostazioni delle notifiche e-mail per più utenti

Quando si configurano le impostazioni di notifica in blocco, è possibile modificare solo le impostazioni comuni agli utenti selezionati.

Quando si modifica un&#39;impostazione di notifica, viene visualizzata l&#39;etichetta **Modificato** per tale impostazione di notifica, per segnalare che l&#39;impostazione di notifica è stata modificata.

Per modificare le impostazioni delle notifiche e-mail per più utenti:

{{step-1-to-users}}

1. Seleziona gli utenti, quindi fai clic su **Modifica**.
1. Nella casella **Modifica persona** visualizzata, fai clic su **Notifiche**.

1. Espandere una categoria per visualizzare le impostazioni di notifica relative a tale categoria.

   Se è selezionato almeno un utente per il quale le notifiche non corrispondono alle notifiche degli altri utenti selezionati, la casella di controllo categoria per tale notifica contiene una riga orizzontale ![Riga anziché un segno di spunta](assets/straight-line-instead-of-checkmark.jpg).


1. Fai clic sulle notifiche che desideri che gli utenti ricevano quotidianamente o istantaneamente o deseleziona quelle che desideri che gli utenti interrompano la ricezione.

   >[!NOTE]
   >
   >   Per la categoria **Comunicazione**, è possibile selezionare singole notifiche solo per la consegna immediata. È necessario selezionare tutte le notifiche da inviare in un riepilogo giornaliero.


1. If you selected notifications to be sent as a daily digest, select the time of the day you want the digest delivered at the top of the **Notifications** section in the **Email Daily Digest after** menu.

   ![Ora riepilogo giornaliera](assets/daily-digest-time.png)

   Il riepilogo giornaliero include gli eventi che soddisfano i criteri delle notifiche 24 ore prima dell&#39;ora selezionata. Gli utenti ricevono un messaggio e-mail di riepilogo giornaliero per ogni tipo di notifica.

   Il riepilogo giornaliero potrebbe arrivare dopo il momento selezionato, a seconda di quante e-mail sono in coda per la consegna nel sistema. L&#39;ora elencata corrisponde all&#39;ora locale specificata nelle impostazioni del browser.

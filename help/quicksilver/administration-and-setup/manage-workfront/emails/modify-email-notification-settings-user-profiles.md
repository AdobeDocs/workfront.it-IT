---
user-type: administrator
product-area: system-administration
keywords: modificare,e-mail,notifica,impostazioni,bulk,modifica in serie,configurare,più,utenti
navigation-topic: emails-administration
title: Modificare le impostazioni di notifica e-mail nei profili degli utenti
description: Se sei un amministratore di Adobe Workfront o disponi di un livello di accesso Planner che consente di modificare le impostazioni di altri utenti, puoi configurare le impostazioni di notifica per più utenti contemporaneamente. Ciò include specificare se gli utenti ricevono notifiche mentre si verificano eventi o in un’e-mail digest giornaliera, come descritto nelle notifiche di Adobe Workfront. Per informazioni sul livello di accesso necessario per modificare gli utenti, consulta Concedere l’accesso agli utenti.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Modificare le impostazioni di notifica e-mail nei profili degli utenti

Se sei un amministratore di Adobe Workfront o disponi di un livello di accesso Planner che consente di modificare le impostazioni di altri utenti, puoi configurare le impostazioni di notifica per più utenti contemporaneamente. Ciò include specificare se gli utenti ricevono notifiche mentre si verificano eventi, o in un’e-mail digest giornaliera, come descritto in [Notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Per informazioni sul livello di accesso necessario per modificare gli utenti, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Quando configuri le impostazioni di notifica in blocco, puoi modificare solo le impostazioni comuni agli utenti selezionati.

Puoi anche configurare le notifiche e-mail per un utente alla volta. Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Modificare le impostazioni di notifica e-mail di più utenti in blocco

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png). Seleziona gli utenti, quindi fai clic su **Modifica**.
1. In **Modifica persona** casella visualizzata, fai clic su **Notifiche**.

1. Espandi una categoria per visualizzare le impostazioni di notifica relative a tale categoria.

   Se è selezionato almeno un utente in cui le notifiche non corrispondono alle notifiche degli altri utenti selezionati, la casella di controllo della categoria relativa a tale notifica contiene una riga orizzontale ![](assets/straight-line-instead-of-checkmark.jpg) invece di un segno di spunta.

1. Fai clic su tutte le notifiche che desideri che gli utenti ricevano quotidianamente o istantaneamente, oppure cancella tutte le notifiche che desideri che smettano di ricevere.

   Per **Comunicazione** categoria , puoi selezionare singole notifiche solo per la consegna istantanea. Devi selezionare tutte le notifiche da consegnare in un riepilogo giornaliero.

   Quando modifichi un’impostazione di notifica, l’etichetta **Modificato** viene visualizzata per tale impostazione di notifica, per informarti che l’impostazione di notifica è stata modificata.

1. Se hai selezionato le notifiche da inviare come riepilogo giornaliero, seleziona l’ora del giorno in cui desideri che il digest venga consegnato nella parte superiore della **Notifiche** nella sezione **Digest giornaliero e-mail dopo** menu.

   Dopo aver selezionato un orario di consegna, la **Digest giornaliero e-mail dopo** viene visualizzata con una cornice arancione per indicare che è stata modificata l’ora della consegna.

   Il riepilogo giornaliero include eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Gli utenti ricevono un’e-mail digest giornaliera per ogni tipo di notifica.

   Il riepilogo giornaliero potrebbe arrivare dopo il tempo selezionato, a seconda del numero di e-mail che vengono messe in coda per la consegna nel sistema. L&#39;ora indicata è l&#39;ora locale specificata nelle impostazioni del browser.

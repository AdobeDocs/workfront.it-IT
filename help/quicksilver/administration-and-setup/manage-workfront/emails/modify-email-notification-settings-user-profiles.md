---
user-type: administrator
product-area: system-administration
keywords: modifica,e-mail,notifica,impostazioni,in blocco,modifica in blocco,configura,più,utenti
navigation-topic: emails-administration
title: Modifica impostazioni di notifica e-mail per più utenti
description: Questo articolo fornisce informazioni agli amministratori di Workfront o di gruppi su come aggiornare le notifiche e-mail di altri utenti.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Modificare le impostazioni delle notifiche e-mail per più utenti

<!-- Audited: 12/2023 -->

Se sei un amministratore di Adobe Workfront o hai un livello di accesso alla Pianificazione che ti consente di modificare le impostazioni di altri utenti, puoi configurare le impostazioni di notifica per più utenti contemporaneamente. Ciò include la specifica se gli utenti ricevono le notifiche quando gli eventi si verificano, oppure in un messaggio e-mail di riepilogo giornaliero, come descritto in [Notifiche di Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Per informazioni sul livello di accesso necessario per modificare gli utenti, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Puoi anche configurare le notifiche e-mail per un utente alla volta, incluso il tuo profilo. Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
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

Quando modifichi un&#39;impostazione di notifica, viene visualizzata l&#39;etichetta **Modificato** per tale impostazione di notifica, per informarti che l&#39;impostazione di notifica è stata modificata.

Per modificare le impostazioni delle notifiche e-mail per più utenti:

{{step-1-to-users}}

1. Seleziona gli utenti, quindi fai clic su **Modifica**.
1. Nella casella **Modifica persona** visualizzata, fare clic su **Notifiche**.

1. Espandere una categoria per visualizzare le impostazioni di notifica relative a tale categoria.

   Se è selezionato almeno un utente le cui notifiche non corrispondono a quelle degli altri utenti selezionati, la casella di controllo categoria per la notifica contiene una riga orizzontale ![Riga invece del segno di spunta](assets/straight-line-instead-of-checkmark.jpg).


1. Fai clic sulle notifiche che desideri che gli utenti ricevano quotidianamente o istantaneamente, oppure cancella le notifiche che desideri che gli utenti smettano di ricevere.

   >[!NOTE]
   >
   >   Per la categoria **Comunicazione**, è possibile selezionare singole notifiche solo per la consegna immediata. Devi selezionare tutte le notifiche da consegnare in un riepilogo giornaliero.


1. Se hai selezionato le notifiche da inviare come riepilogo giornaliero, seleziona l&#39;ora del giorno in cui desideri che il riepilogo venga consegnato nella parte superiore della sezione **Notifiche** nel menu **Invia riepilogo giornaliero tramite posta elettronica dopo**.

   ![Ora riepilogo giornaliera](assets/daily-digest-time.png)

   Il riepilogo giornaliero include gli eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Gli utenti ricevono un’e-mail di riepilogo giornaliero per ogni tipo di notifica.

   Il riepilogo giornaliero può arrivare dopo l’orario selezionato, a seconda di quante e-mail sono in coda per la consegna nel sistema. L’ora indicata corrisponde all’ora locale specificata nelle impostazioni del browser.

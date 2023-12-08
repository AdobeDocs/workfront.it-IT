---
user-type: administrator
product-area: system-administration
keywords: modifica,e-mail,notifica,impostazioni,in blocco,modifica in blocco,configura,più,utenti
navigation-topic: emails-administration
title: Modificare le impostazioni delle notifiche e-mail per più utenti
description: Questo articolo fornisce informazioni agli amministratori di Workfront o di gruppi su come aggiornare le notifiche e-mail di altri utenti.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 7c1115065e4d2f4732b392336aed692c055ba97c
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Modificare le impostazioni delle notifiche e-mail per più utenti

Se sei un amministratore di Adobe Workfront o hai un livello di accesso alla Pianificazione che ti consente di modificare le impostazioni di altri utenti, puoi configurare le impostazioni di notifica per più utenti contemporaneamente. Ciò include specificare se gli utenti ricevono le notifiche quando gli eventi si verificano, oppure in un’e-mail di riepilogo giornaliera, come descritto in [Notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Per informazioni sul livello di accesso necessario per modificare gli utenti, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Puoi anche configurare le notifiche e-mail per un utente alla volta, incluso il tuo profilo. Per ulteriori informazioni, consulta [Modifica le tue notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo piano: Standard </p>
 <p>oppure</p> 
<p>Piano corrente: piano </p> 
</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore Workfront.

## Modificare le impostazioni delle notifiche e-mail per più utenti

Quando si configurano le impostazioni di notifica in blocco, è possibile modificare solo le impostazioni comuni agli utenti selezionati.

Quando modifichi un’impostazione di notifica, l’etichetta **Modificato** per l&#39;impostazione di notifica, per comunicare che l&#39;impostazione di notifica è stata modificata.

Per modificare le impostazioni delle notifiche e-mail per più utenti:

{{step-1-to-users}}

1. Seleziona gli utenti, quindi fai clic su **Modifica**.
1. In **Modifica persona** visualizzata, fare clic su **Notifiche**.

1. Espandere una categoria per visualizzare le impostazioni di notifica relative a tale categoria.

   Se è selezionato almeno un utente le cui notifiche non corrispondono a quelle degli altri utenti selezionati, la casella di controllo Categoria relativa a tale notifica contiene una riga orizzontale ![](assets/straight-line-instead-of-checkmark.jpg) invece di un segno di spunta.


1. Fai clic sulle notifiche che desideri che gli utenti ricevano quotidianamente o istantaneamente, oppure cancella le notifiche che desideri che gli utenti smettano di ricevere.

   >[!NOTE]
   >
   >   Per **Comunicazione** categoria, puoi selezionare singole notifiche solo per la consegna immediata. Devi selezionare tutte le notifiche da consegnare in un riepilogo giornaliero.


1. Se hai selezionato le notifiche da inviare come riepilogo giornaliero, seleziona l’ora del giorno in cui desideri che il riepilogo venga consegnato all’inizio del **Notifiche** sezione nella sezione **Invia digest tramite e-mail ogni giorno dopo** menu.

   ![](assets/daily-digest-time.png)

   Il riepilogo giornaliero include gli eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Gli utenti ricevono un’e-mail di riepilogo giornaliero per ogni tipo di notifica.

   Il riepilogo giornaliero può arrivare dopo l’orario selezionato, a seconda di quante e-mail sono in coda per la consegna nel sistema. L’ora indicata corrisponde all’ora locale specificata nelle impostazioni del browser.

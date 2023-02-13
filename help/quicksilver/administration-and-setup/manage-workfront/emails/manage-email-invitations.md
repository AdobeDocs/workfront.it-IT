---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gestire gli inviti via e-mail a nuovi utenti
description: In qualità di amministratore di Adobe Workfront, puoi aggiungere utenti a Workfront e avvisarli dell’aggiunta tramite inviti e-mail.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# Gestire gli inviti via e-mail a nuovi utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, puoi aggiungere utenti a Workfront e avvisarli dell’aggiunta tramite inviti e-mail.

L’invito e-mail consente ai nuovi utenti di seguire un collegamento in cui possono scegliere una password per il loro account Workfront. Possono quindi finire di configurare il proprio account.

Per garantire la sicurezza dei nuovi account, si consiglia di utilizzare gli inviti e-mail per i nuovi utenti, in modo che possano scegliere la propria password. In alternativa, è possibile selezionare una password per un nuovo utente quando si crea il proprio account. Per ulteriori informazioni sull’aggiunta di nuovi utenti a Workfront, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Puoi configurare le nuove e-mail utente per:

* Qualsiasi nuovo utente aggiunto a Workfront
* Utenti aggiunti a Workfront con una licenza Richiedente

Tutti i nuovi utenti visualizzano la stessa e-mail quando viene inviato un invito e-mail.

Per informazioni sulla ricezione di inviti e-mail, consulta [Ricevi inviti e-mail e crea una password per Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Requisiti di accesso

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Genera inviti e-mail {#generate-email-invitations}

Gli inviti e-mail vengono generati nei seguenti scenari:

* Quando crei un nuovo utente e selezioni la **Invia un messaggio e-mail di invito a questa persona** sulla **Nuovo utente** modulo. Per ulteriori informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Quando importi più nuovi utenti e selezioni la **Invia e-mail di invito a queste persone** opzione . Per ulteriori informazioni sull’importazione di diversi nuovi utenti, consulta [Importare utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Dopo la creazione degli utenti, puoi generare manualmente gli inviti agli utenti che non hanno ancora registrato il loro account con Workfront e che non hanno stabilito una password Workfront.\
   Gli utenti che hanno creato un account ma che non hanno ancora registrato il proprio account sono contrassegnati come **Non registrato** in Workfront.

   >[!NOTE]
   >
   >Se deselezioni la **Invia un invito tramite e-mail a questa persona** quando crei l’utente, l’invito e-mail non può essere generato manualmente. L’invio manuale degli inviti e-mail è possibile solo per gli utenti a cui è stato inviato l’invito e-mail originale al momento della creazione del loro account. Per ulteriori informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Per generare manualmente gli inviti e-mail agli utenti non registrati esistenti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
1. Seleziona l’utente che visualizza la **Non registrato** etichetta dopo il loro nome.

   ![](assets/unreg-user-qs-350x221.png)

1. Fai clic sull’icona Altro ![](assets/more-icon.png), quindi fai clic su **Ricordare all&#39;utente di registrarsi**.

   Viene inviato un invito e-mail al nuovo utente con un nuovo collegamento che può utilizzare per creare la password Workfront.

   >[!NOTE]
   >
   >Se l’organizzazione è stata imbarcata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi scegliere di inviare un invito e-mail a nuovi utenti.
   >
   >All’Admin Console vengono aggiunti nuovi utenti di Adobe e l’Admin Console invia un messaggio e-mail per invitarli a completare il processo di registrazione. Tutti gli utenti devono completare il processo di registrazione per accedere a qualsiasi sistema di Adobe.
   >
   >Per gli utenti esistenti di Adobe, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Si tratta di una preferenza controllata dall’amministratore di Adobe per il prodotto.

## Configurare gli inviti e-mail {#configure-email-invitations}

In qualità di amministratore di Workfront, puoi configurare il messaggio incluso con gli inviti e-mail per i nuovi utenti.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nell&#39;elenco a sinistra, fai clic su **E-mail** > **Inviti**.

1. In **Opzioni generali** effettua una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disattiva i collegamenti di invito dopo ... giorni</strong> </td> 
      <td> <p>Scegli il periodo di tempo dopo il quale gli inviti e-mail non contengono più un collegamento valido a Workfront. Il valore predefinito è 45 giorni.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Includere un messaggio e/o un termine di servizio</strong> </td> 
      <td> <p>Seleziona questa opzione se desideri modificare l’invito e-mail per tutti i nuovi utenti aggiunti a Workfront. Ciò non include gli utenti con una licenza Richiedente.</p> 
       <ul> 
        <li><strong>Messaggio</strong>: Se scegli di modificare l’invito e-mail per tutti i nuovi utenti, specifica il testo da includere negli inviti e-mail come corpo dell’e-mail.</li> 
        <li><strong>Termini e condizioni</strong>: Se selezioni di modificare l’invito e-mail per tutti i nuovi utenti, specifica il testo da includere negli inviti e-mail come termini e condizioni.<br></li> 
        <li><strong>Includere un messaggio e/o una durata del servizio per gli utenti dell'helpdesk</strong>: Seleziona questa opzione se desideri modificare l’invito e-mail per tutti i nuovi utenti aggiunti a Workfront che dispongono di una licenza Richiedente.</li> 
        <li><strong>Messaggio</strong>: Se scegli di modificare l’invito e-mail per tutti i nuovi utenti con una licenza Richiedente, specifica il testo da includere negli inviti e-mail come corpo dell’e-mail.</li> 
        <li><strong>Termini e condizioni</strong>: Se selezioni di modificare l’invito e-mail per tutti i nuovi utenti con una licenza Richiedente, specifica il testo da includere negli inviti e-mail come termini e condizioni.<br></li> 
        <li> <p>In <strong>Anteprima invito</strong> Puoi visualizzare un’anteprima del tuo invito e-mail. Se hai selezionato di includere un messaggio personalizzato nell’invito e-mail, il messaggio personalizzato viene visualizzato in quest’area.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

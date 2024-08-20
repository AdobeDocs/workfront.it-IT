---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gestire gli inviti e-mail ai nuovi utenti
description: In qualità di amministratore di Adobe Workfront, puoi aggiungere utenti a Workfront e avvisarli che sono stati aggiunti, utilizzando inviti e-mail.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Gestire gli inviti e-mail per i nuovi utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, puoi aggiungere utenti a Workfront e avvisarli che sono stati aggiunti, utilizzando inviti e-mail.

L’invito e-mail consente ai nuovi utenti di seguire un collegamento tramite il quale è possibile scegliere una password per il proprio account Workfront. Potranno quindi completare l’impostazione dell’account.

Per garantire la sicurezza dei nuovi account, si consiglia di utilizzare gli inviti e-mail per i nuovi utenti, in modo che possano scegliere la propria password. In alternativa, è possibile selezionare una password per un nuovo utente al momento della creazione dell&#39;account. Per ulteriori informazioni sull&#39;aggiunta di nuovi utenti a Workfront, vedere [Aggiungere utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Puoi configurare le e-mail del nuovo utente per:

* Qualsiasi nuovo utente aggiunto a Workfront
* Utenti aggiunti a Workfront con una licenza Requestor

Tutti i nuovi utenti visualizzano la stessa e-mail quando viene inviato un invito e-mail.

Per informazioni sulla ricezione di inviti e-mail, vedere [Ricevere inviti e-mail e creare una password per Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Genera inviti e-mail {#generate-email-invitations}

Gli inviti e-mail vengono generati nei seguenti scenari:

* Quando crei un nuovo utente e selezioni **Invia un&#39;e-mail di invito a questa persona** nel modulo **Nuovo utente**. Per ulteriori informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Quando importi più nuovi utenti e selezioni l&#39;opzione **Invia e-mail di invito a queste persone**. Per ulteriori informazioni sull&#39;importazione di diversi nuovi utenti, vedere [Importa utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Dopo la creazione degli utenti, è possibile generare manualmente gli inviti agli utenti che non hanno ancora registrato il proprio account con Workfront e che non hanno stabilito una password Workfront.\
  Gli utenti che hanno creato un account ma non lo hanno ancora registrato sono contrassegnati come **Non registrati** in Workfront.

  >[!NOTE]
  >
  >Se deselezioni la casella **Invia un invito e-mail a questa persona** al momento della creazione dell&#39;utente, l&#39;invito e-mail non può essere generato manualmente. È possibile inviare manualmente gli inviti e-mail solo agli utenti a cui è stato inviato l’invito e-mail originale al momento della creazione del loro account. Per ulteriori informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Per generare manualmente inviti e-mail per utenti esistenti non registrati:

{{step-1-to-users}}

1. Seleziona l&#39;utente che mostra l&#39;etichetta **Non registrato** dopo il nome.

   ![](assets/unreg-user-qs-350x221.png)

1. Fai clic sull&#39;icona Altro ![](assets/more-icon.png), quindi fai clic su **Ricorda all&#39;utente di registrarsi**.

   Al nuovo utente viene inviato un invito e-mail con un nuovo collegamento da utilizzare per creare la password Workfront.

   >[!NOTE]
   >
   >Se la tua organizzazione è stata integrata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi inviare un invito e-mail a nuovi utenti.
   >
   >I nuovi utenti dell’Adobe vengono aggiunti all’Admin Console Admin Console, che a sua volta distribuisce un’e-mail per invitarli a completare la procedura di registrazione. Tutti gli utenti devono completare la procedura di registrazione per accedere a qualsiasi Adobe.
   >
   >Per gli Adobi esistenti, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Questa è una preferenza controllata dall’amministratore di Adobe per il prodotto.

## Configurare gli inviti e-mail {#configure-email-invitations}

In qualità di amministratore di Workfront, puoi configurare il messaggio da includere con gli inviti e-mail per i nuovi utenti.

{{step-1-to-setup}}

1. Nell&#39;elenco a sinistra, fare clic su **E-mail** > **Inviti**.

1. Nella sezione **Opzioni generali**, apporta una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disattiva i collegamenti di invito dopo ... giorni</strong> </td> 
      <td> <p>Scegliere il periodo di tempo dopo il quale gli inviti e-mail non contengono più un collegamento valido a Workfront. L'importo predefinito di giorni è 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Includi un messaggio e/o un termine di servizio</strong> </td> 
      <td> <p>Seleziona questa opzione se desideri modificare l’invito e-mail per tutti i nuovi utenti aggiunti a Workfront. Non sono inclusi gli utenti con una licenza Requestor.</p> 
       <ul> 
        <li><strong>Messaggio</strong>: se si sceglie di modificare l'invito e-mail per tutti i nuovi utenti, specificare il testo da includere negli inviti e-mail come corpo dell'e-mail.</li> 
        <li><strong>Termini e condizioni</strong>: se si sceglie di modificare l'invito e-mail per tutti i nuovi utenti, specificare il testo da includere negli inviti e-mail come termini e condizioni.<br></li> 
        <li><strong>Includi un messaggio e/o un termine di servizio per gli utenti dell'helpdesk</strong>: selezionare questa opzione se si desidera modificare l'invito tramite posta elettronica per tutti i nuovi utenti aggiunti a Workfront che dispongono di una licenza Requestor.</li> 
        <li><strong>Messaggio</strong>: se si seleziona di modificare l'invito e-mail per tutti i nuovi utenti con una licenza Requestor, specificare il testo da includere negli inviti e-mail come corpo dell'e-mail.</li> 
        <li><strong>Termini e condizioni</strong>: se si sceglie di modificare l'invito e-mail per tutti i nuovi utenti con una licenza Richiedente, specificare il testo da includere negli inviti e-mail come termini e condizioni.<br></li> 
        <li> <p>Nella sezione <strong>Anteprima invito</strong> è disponibile un'anteprima dell'invito e-mail. Se hai selezionato di includere un messaggio personalizzato nell’invito e-mail, il messaggio personalizzato viene visualizzato in quest’area.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

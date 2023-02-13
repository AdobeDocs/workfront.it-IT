---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Assegnare tag agli utenti per condividere una bozza
description: Quando si commenta una bozza nel visualizzatore di bozze, è possibile assegnare tag ad altri utenti per attirare la loro attenzione sul commento tramite e-mail e aggiungerli al flusso di lavoro della bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Assegnare tag agli utenti per condividere una bozza

Quando si commenta una bozza nel visualizzatore di bozze, è possibile assegnare tag ad altri utenti per attirare la loro attenzione sul commento tramite e-mail e aggiungerli al flusso di lavoro della bozza.

Quando assegni tag agli utenti nei commenti su una bozza, gli utenti a cui puoi assegnare i tag possono variare a seconda di vari fattori, ad esempio le autorizzazioni per i singoli utenti e l’iscrizione nell’organizzazione:

* Se sei l’autore della bozza, il proprietario o disponi di autorizzazioni specifiche abilitate, puoi assegnare tag agli utenti al di fuori del flusso di lavoro della bozza e condividerla con loro.
* Se sei stato aggiunto alla bozza come utente esterno e sei membro di un altro ambiente con un account di prova diverso, puoi assegnare tag solo agli utenti dell’ambiente originale. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Requisiti di accesso {#access-requirements}

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ruolo di prova</td> 
   <td>Autore, Moderatore</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Supervisore o amministratore</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Assegnare tag agli utenti per condividere una bozza

Utenti con il ruolo Profilo di autorizzazione bozza o Proof descritto nel [Requisiti di accesso](#access-requirements) La sezione precedente può assegnare agli utenti un tag per condividere una bozza per impostazione predefinita. Puoi anche assegnare tag agli utenti affinché condividano una bozza indipendentemente dal ruolo Profilo di autorizzazione bozza o Proof , se sei il proprietario o creatore della bozza. Puoi consentire agli utenti con ruoli Profilo di autorizzazione bozza o Proof inferiori di condividere una bozza quando crei una bozza. Per ulteriori informazioni, consulta la sezione [Configurare il flusso di lavoro e aggiungere revisori](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) nella sezione [Creare una bozza avanzata con un flusso di lavoro di base](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) articolo.

>[!NOTE]
>
>Puoi assegnare un tag a un collaboratore esterno utilizzando il suo indirizzo e-mail solo se una delle seguenti affermazioni è vera:>
>* Un utente dell’account Workfront della tua organizzazione ha aggiunto in precedenza l’indirizzo e-mail del collaboratore a una bozza.
>* Il collaboratore ha utilizzato l’indirizzo e-mail per registrarsi a una bozza nell’account Workfront della tua organizzazione in precedenza.
>


Per assegnare tag a qualcuno e condividere una bozza in un commento:

1. Quando si commenta una bozza, digitare un segno di spunta (@) seguito dal nome o dall&#39;indirizzo di posta elettronica della persona. Quando inizi a digitare, i nomi disponibili vengono visualizzati in un elenco a discesa.
1. Selezionare il nome della persona quando la si visualizza nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Se desideri chiudere l’elenco a discesa senza selezionare nessuno, puoi premere il pulsante **Esc** fare clic in un punto qualsiasi all’esterno dell’elenco.

1. Ripeti i passaggi 1-2 per tutti gli altri utenti a cui desideri assegnare un tag nel commento.
1. Termina il commento, quindi fai clic su **Post**.
1. (Condizionale) Se hai applicato tag a persone che non erano già state aggiunte alla bozza, specifica un **Ruolo di prova** e **Avvisi e-mail** per ogni utente elencato nella casella visualizzata, quindi fare clic su **Aggiungi persone e pubblica un commento**.

   ![](assets/add-people-to-proof-350x220.png)

   Per informazioni sui ruoli di bozza, consulta . Per informazioni sugli avvisi e-mail di bozza, consulta la sezione nell’articolo [Configurare le impostazioni di notifica e-mail in Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Se la bozza dispone di un flusso di lavoro automatizzato, gli utenti a cui è stato applicato il tag vengono aggiunti all’area di visualizzazione in cui ci si trova. Per ulteriori informazioni, consulta [Panoramica del flusso di lavoro automatizzato](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Chiunque assegni un tag riceve un messaggio e-mail di notifica relativo al tuo commento di bozza, indipendentemente dalle impostazioni di avviso e-mail di bozza che stanno utilizzando:

   * Se l’utente riceve un’e-mail di riepilogo giornaliero o orario, Workfront invia la notifica separatamente e include informazioni sul commento della bozza nell’e-mail di riepilogo.
   * Se l’utente riceve avvisi relativi a tutte le attività o alle risposte ai propri commenti, la notifica sostituisce le notifiche relative a tali commenti e risposte.

Per informazioni su altri modi per aggiungere utenti a una bozza, vedi [Condividere una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Assegnare tag agli utenti per condividere una bozza
description: Quando inserisci un commento su una bozza nel visualizzatore di bozze, puoi assegnare un tag ad altri utenti per attirare l’attenzione sul commento tramite e-mail e aggiungerli al flusso di lavoro della bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Assegnare tag agli utenti per condividere una bozza

Quando inserisci un commento su una bozza nel visualizzatore di bozze, puoi assegnare un tag ad altri utenti per attirare l’attenzione sul commento tramite e-mail e aggiungerli al flusso di lavoro della bozza.

Quando si assegnano tag agli utenti nei commenti di una bozza, gli utenti a cui è possibile assegnare tag possono variare a seconda di vari fattori, come le autorizzazioni per i singoli utenti e l’appartenenza all’organizzazione:

* Se sei il creatore o il proprietario della bozza oppure disponi di autorizzazioni specifiche abilitate, puoi assegnare tag agli utenti al di fuori del flusso di lavoro della bozza e condividere la bozza con loro.
* Se sei stato aggiunto alla bozza come utente esterno e fai parte di un altro ambiente con un account di bozza diverso, puoi assegnare tag solo a tali utenti dall’ambiente originale. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Requisiti di accesso {#access-requirements}

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ruolo bozza</td> 
   <td>Autore, Moderatore</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Supervisore o amministratore</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Assegnare tag agli utenti per condividere una bozza

Gli utenti con il profilo di autorizzazione di una bozza o il ruolo di bozza descritto nella sezione [Requisiti di accesso](#access-requirements) possono assegnare tag agli utenti per la condivisione di una bozza per impostazione predefinita. Puoi anche assegnare agli utenti dei tag per condividere una bozza, indipendentemente dal profilo di autorizzazione della bozza o dal ruolo Bozza, se sei il proprietario o il creatore della bozza. Puoi consentire agli utenti con un Profilo di autorizzazione di bozza inferiore o Ruoli di bozza di assegnare un tag agli utenti per condividere una bozza durante la sua creazione. Per ulteriori informazioni, consulta la sezione [Configurare il flusso di lavoro e aggiungere i revisori](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) nell&#39;articolo [Creare una bozza avanzata con un flusso di lavoro di base](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Puoi assegnare tag a un collaboratore esterno utilizzando il suo indirizzo e-mail solo se si verifica una delle seguenti condizioni:>
>* Un utente nell’account Workfront della tua organizzazione ha aggiunto in precedenza l’indirizzo e-mail del collaboratore a una bozza.
>* Il collaboratore ha già utilizzato l’indirizzo e-mail per iscriversi a una bozza nell’account Workfront della tua organizzazione.
>

Per assegnare un tag a qualcuno e condividere una bozza in un commento:

1. Quando si commenta una bozza, digitare il simbolo @ seguito dal nome o dall&#39;indirizzo di posta elettronica della persona. Quando si inizia a digitare, i nomi disponibili vengono visualizzati in un elenco a discesa.
1. Seleziona il nome della persona quando la vedi nell’elenco a discesa.

   >[!TIP]
   >
   >Se si desidera chiudere l&#39;elenco a discesa senza selezionare alcun utente, è possibile premere il tasto **Esc** o fare clic in un punto qualsiasi all&#39;esterno dell&#39;elenco.

1. Ripeti i passaggi 1-2 per tutti gli altri utenti a cui desideri assegnare tag nel commento.
1. Termina il commento, quindi fai clic su **Post**.
1. (Condizionale) Se hai assegnato un tag a qualcuno che non è già stato aggiunto alla bozza, specifica un&#39;impostazione per **Ruolo bozza** e **Avvisi e-mail** per ogni utente elencato nella casella visualizzata, quindi fai clic su **Aggiungi persone e pubblica commento**.

   ![](assets/add-people-to-proof-350x220.png)

   Per informazioni sui ruoli delle bozze, consulta . Per informazioni sugli avvisi e-mail relativi alle bozze, vedere la sezione dell&#39;articolo [Configurare le impostazioni delle notifiche e-mail in Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Se la bozza dispone di un flusso di lavoro automatizzato, gli utenti a cui si applicano i tag vengono aggiunti alla fase in cui ci si trova. Per ulteriori informazioni, vedere [Panoramica del flusso di lavoro automatico](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Chiunque assegni un tag riceve un’e-mail di notifica relativa al commento della bozza, indipendentemente dalle impostazioni degli avvisi e-mail per le bozze in uso:

   * Se l’utente riceve un’e-mail di riepilogo giornaliero o orario, Workfront invia la notifica separatamente e include informazioni sul commento della bozza nell’e-mail di riepilogo.
   * Se l’utente riceve avvisi per tutte le attività o per le risposte ai propri commenti, la notifica sostituisce le notifiche relative a tali commenti e risposte.

Per informazioni su altri modi per aggiungere utenti a una bozza, consulta [Condividere una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

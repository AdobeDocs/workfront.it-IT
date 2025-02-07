---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare le impostazioni di bozza predefinite
description: Queste impostazioni consentono di impostare i valori predefiniti applicabili a tutte le nuove bozze create dagli utenti. Tuttavia, gli utenti possono ignorare la maggior parte di queste impostazioni durante la creazione di una bozza.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 7%

---

# Configurare le impostazioni di bozza predefinite

Queste impostazioni consentono di impostare i valori predefiniti applicabili a tutte le nuove bozze create dagli utenti. Tuttavia, gli utenti possono ignorare la maggior parte di queste impostazioni durante la creazione di una bozza.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td>
   <p>Nuovo: Standard</p>
   oppure
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Configurare le nuove impostazioni predefinite della bozza

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Bozze** > **Impostazioni bozza**.
1. Nella sezione **Nuovi valori predefiniti per la bozza** configura le impostazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Destinatari</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesso obbligatorio</td> 
      <td> <p>I revisori devono accedere con la propria e-mail e password prima di poter visualizzare le bozze create nell’account della tua organizzazione. Se questa opzione è abilitata, gli utenti non possono condividere la bozza con i revisori ospiti.</p> <p><b>IMPORTANTE</b>: se abilitata, l'accesso è necessario per tutte le nuove bozze create.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia il proprietario dalla bozza originale per le nuove versioni</td> 
      <td> <p>Il proprietario della prima versione di una bozza è anche il proprietario di tutte le versioni consecutive della bozza, indipendentemente da chi crea queste versioni. Questa impostazione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti agli utenti di eliminare i propri commenti in bozza</td> 
      <td>Gli utenti possono eliminare i propri commenti. Questa impostazione è attivata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni </td> 
      <td> <p>Ai decision maker viene richiesto di inserire le credenziali di accesso a Workfront quando prendono una decisione su una bozza.</p> <p><b>IMPORTANTE</b>: se questa opzione è abilitata, gli utenti non possono condividere la bozza con i revisori guest che non dispongono delle credenziali di accesso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Scadenza</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impostare la scadenza predefinita</td> 
      <td> <p>Il sistema applica questa scadenza a tutte le nuove bozze nel tuo account che non hanno un flusso di lavoro automatico.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifica i destinatari prima che la bozza sia a rischio</td> 
      <td>I destinatari ricevono una notifica via e-mail prima che la bozza venga considerata a rischio a seconda della scadenza specificata in precedenza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Notifiche e-mail</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifica i destinatari quando vengono aggiunti a una bozza</td> 
      <td>I destinatari ricevono una notifica tramite e-mail quando vengono aggiunti a una bozza.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

## Configurare le decisioni relative alle bozze

Gli utenti possono utilizzare le decisioni relative alle bozze per indicare lo stato della bozza dopo la revisione.

>[!NOTE]
>
>La logica alla base delle decisioni relative alle bozze viene utilizzata per calcolare lo stato complessivo di un flusso di lavoro di una bozza in presenza di più decisioni di vari livelli. Le decisioni &quot;Approvato&quot; e &quot;Approvato con modifiche&quot; attivano la fase successiva in un flusso di lavoro automatico.

Per configurare le decisioni relative alle bozze:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Bozze** > **Impostazioni bozza**.
1. Nella sezione **Decisioni** puoi

   1. **Rinomina la decisione**: fare clic sul testo all&#39;interno della casella di decisione e iniziare a digitare la nuova etichetta di decisione.

      >[!TIP]
      >
      >Quando lo rinomini, mantieni la logica per una decisione. Ad esempio, la decisione predefinita Rifiutata potrebbe essere modificata in *Nuova versione richiesta*, ma non dovrebbe essere modificata in *Invia a stampanti*.

      ![Rinomina decisione](assets/rename-decision-350x109.png)

   1. **Ridisponi l&#39;ordine di decisione**: trascina le caselle di decisione nell&#39;ordine in cui desideri che vengano visualizzate nel visualizzatore di bozze.

      ![Sposta decisione](assets/move-decision-350x110.png)

   1. **Nascondi una decisione**: passa il puntatore del mouse sulla casella di decisione e fai clic sull&#39;icona Nascondi nell&#39;angolo superiore destro.

      ![Nascondi decisione](assets/hide-decision-350x109.png)

1. (Facoltativo) Per tornare ai valori predefiniti di Workfront, fare clic su **Ripristina valori predefiniti**.
1. Fai clic su **Salva**.

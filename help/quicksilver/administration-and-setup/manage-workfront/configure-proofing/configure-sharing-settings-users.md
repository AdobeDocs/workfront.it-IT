---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare le impostazioni di condivisione per gli utenti
description: In qualità di amministratore di Adobe Workfront o di Workfront Proof, puoi configurare gli account utente con cui è possibile condividere le bozze, specificare se gli utenti possono visualizzare tutte le versioni di una bozza e i tempi in cui gli utenti possono accedere agli elementi condivisi.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Configurare le impostazioni di condivisione per gli utenti

In qualità di amministratore di Adobe Workfront o di Workfront Proof, puoi configurare gli account utente con cui è possibile condividere le bozze, specificare se gli utenti possono visualizzare tutte le versioni di una bozza e i tempi in cui gli utenti possono accedere agli elementi condivisi.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Nel profilo di autorizzazione bozza deve essere selezionato Amministratore. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurare l'accesso di verifica di un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Configurare la condivisione con altri account

1. Da Workfront, fare clic sul menu principale ![](assets/main-menu-icon.png), quindi fare clic su Bozza ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic sulla scheda **Impostazioni**.

1. Nella sezione **Condivisione**, a destra di **Consenti condivisione con**, fare clic su **Configurazione**.

1. Nell’elenco a discesa visualizzato, seleziona un’opzione per specificare se desideri rendere le bozze disponibili a chiunque, limitare la condivisione delle bozze solo al tuo account personale o limitarla al tuo account personale e a tutti gli account partner con cui stai collaborando.
1. Fai clic su **Salva.**

## Configurare la visibilità per tutte le versioni di una bozza condivisa

1. Da Workfront, fare clic sul menu principale ![](assets/main-menu-icon.png), quindi fare clic su Bozza ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic sulla scheda **Impostazioni**.

1. Nella sezione **Condivisione**, a destra di **I destinatari possono visualizzare tutte le versioni**, selezionare **Abilita** o **Disabilita** per indicare se si desidera consentire ai destinatari di visualizzare tutte le versioni di una bozza nel visualizzatore di bozze quando l&#39;URL della bozza è abilitato.

## Configurare la visibilità delle bozze in base all’attività della fase del flusso di lavoro

È possibile specificare quando le bozze con un flusso di lavoro automatico sono visibili agli utenti associati a una determinata fase.

>[!NOTE]
>
>* Questa opzione è disponibile solo quando si utilizza l&#39;applicazione Workfront Proof standalone; non è disponibile quando si utilizza un&#39;istanza Workfront Proof integrata con Workfront o quando si esegue la verifica in Workfront.
>* Gli utenti ricevono una notifica e-mail relativa alla bozza solo dopo che è entrata nella fase a cui l’utente è associato, indipendentemente da questa impostazione.
>

Per configurare quando le bozze con un flusso di lavoro automatizzato sono visibili agli utenti:

1. Da Workfront, fare clic sul menu principale ![](assets/main-menu-icon.png), quindi fare clic su Bozza ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic sulla scheda **Impostazioni**.

1. Nella sezione **Condivisione**, abilita o disabilita **Visibilità bozza in base all&#39;attivazione della fase**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disabilitato</strong> (impostazione predefinita)</td> 
      <td>Le bozze sono visibili agli utenti al momento della creazione della bozza.<br><p>Qualsiasi utente associato a una fase del flusso di lavoro per la bozza può visualizzarla nei risultati di ricerca subito dopo la creazione della bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abilitato</strong> </td> 
      <td> <p>Le bozze sono visibili agli utenti solo dopo che la fase a cui sono associate diventa <strong>attiva.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Dopo aver abilitato questa opzione, le bozze esistenti saranno ancora visibili agli utenti che potrebbero visualizzarle al momento della creazione.</em> </li> 
         <li>Quando un utente ottiene l’accesso a una versione di una bozza (perché la fase a cui è associato l’utente diventa attiva), può visualizzare solo la versione in cui è attivata. Se una versione precedente non ha mai raggiunto la fase a cui l’utente è associato, l’utente non può visualizzare tale versione della bozza.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

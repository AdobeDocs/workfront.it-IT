---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare le impostazioni di condivisione per gli utenti
description: In qualità di amministratore di Adobe Workfront o amministratore di Workfront Proof, puoi configurare gli account utente con cui è possibile condividere le bozze, se gli utenti possono visualizzare tutte le versioni di una bozza e la data e l’ora in cui gli utenti possono accedere agli elementi condivisi.
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

In qualità di amministratore di Adobe Workfront o amministratore di Workfront Proof, puoi configurare gli account utente con cui è possibile condividere le bozze, se gli utenti possono visualizzare tutte le versioni di una bozza e la data e l’ora in cui gli utenti possono accedere agli elementi condivisi.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario che l’amministratore sia selezionato nel profilo delle autorizzazioni di prova. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurare l’accesso per la correzione di un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare la condivisione con altri account

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic su **Impostazioni** scheda .

1. In **Condivisione** a destra di **Consenti condivisione con**, fai clic su **Configurazione**.

1. Nell’elenco a discesa visualizzato, seleziona un’opzione per specificare se desideri rendere disponibili le bozze a chiunque, limitare la condivisione delle bozze solo sul tuo account o limitarla al tuo account e a qualsiasi account partner con cui stai collaborando.
1. Fai clic su **Salva.**

## Configurare la visibilità di tutte le versioni di una bozza condivisa

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic su **Impostazioni** scheda .

1. In **Condivisione** a destra di **I destinatari possono visualizzare tutte le versioni**, seleziona **Abilita** o **Disattiva** per indicare se si desidera consentire ai destinatari di visualizzare tutte le versioni di una bozza all’interno del visualizzatore di correzione quando l’URL di prova è abilitato.

## Configurare la visibilità della bozza in base all’attività della fase del flusso di lavoro

Puoi specificare quando le bozze con un flusso di lavoro automatizzato sono visibili agli utenti associati a un determinato passaggio.

>[!NOTE]
>
>* Questa opzione è disponibile solo quando si utilizza l’applicazione Workfront Proof autonoma; non è disponibile quando si utilizza un’istanza di Workfront Proof integrata con Workfront o durante la correzione all’interno di Workfront.
>* Gli utenti ricevono una notifica e-mail sulla bozza solo dopo essere entrati nell’area di visualizzazione a cui è associato l’utente, indipendentemente da questa impostazione.
>


Per configurare quando le bozze con un flusso di lavoro automatizzato sono visibili agli utenti:

1. In Workfront, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su Proofing ![](assets/proofing-in-main-menu.png) per accedere a Workfront Proof.

1. Fai clic su **Impostazioni** > **Impostazioni account**, quindi fai clic su **Impostazioni** scheda .

1. In **Condivisione** sezione, attiva o disattiva **Visibilità di prova basata sull’attivazione dell’area di visualizzazione**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disabilitato</strong> (predefinito)</td> 
      <td>Le bozze sono visibili agli utenti al momento della creazione della bozza.<br><p>Qualsiasi utente associato a un’area di lavoro del flusso di lavoro per la bozza può visualizzare la bozza nei risultati della ricerca immediatamente dopo la creazione della bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abilitato</strong> </td> 
      <td> <p>Le bozze sono visibili agli utenti solo dopo che l’area di visualizzazione a cui sono associate diventa visibile <strong>attivo.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Dopo aver abilitato questa opzione, le bozze esistenti sono ancora visibili agli utenti che possono visualizzarle al momento della creazione.</em> </li> 
         <li>Dopo che un utente ha accesso a una versione di una bozza (poiché l’area di visualizzazione a cui è associato l’utente diventa attiva), l’utente può vedere solo la versione in cui è attivata l’area di visualizzazione. Se una versione precedente non ha mai raggiunto lo stadio a cui è associato l’utente, quest’ultimo non può vedere tale versione della bozza.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

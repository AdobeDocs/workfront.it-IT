---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Prova di una risorsa collegata per Experience Manager Assets o Assets Essentials
description: Dopo aver collegato una risorsa da Experience Manager Assets Essentials, puoi creare una bozza e assegnare agli utenti la possibilità di rivedere e aggiungere commenti alla risorsa.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Prova di una risorsa collegata per Experience Manager Assets o Assets Essentials

Dopo aver collegato una risorsa da Experience Manager Assets Essentials, puoi creare una bozza e assegnare agli utenti la possibilità di rivedere e aggiungere commenti alla risorsa.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p>
   <p>È necessario che la correzione sia abilitata per l’utente.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi disporre di un Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza accesso o superiore</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l’integrazione as a Cloud Service di Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l’integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Crea una bozza

Puoi creare bozze statiche, video o interattive.

Per creare una bozza:

1. Vai al progetto, all&#39;attività o al problema in cui desideri ottenere la bozza, quindi fai clic sul pulsante **Documenti** sezione .
1. Passa il puntatore del mouse sul documento, quindi fai clic sul pulsante **Crea bozza** link che appare sotto il nome del documento.

   >[!NOTE]
   >
   >Se **Generazione automatica di bozze durante il caricamento di documenti** attivato nel profilo utente, il sistema crea automaticamente una prova semplice.

1. Scegliere una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Prova semplice</strong></td> 
      <td>Questa opzione crea una bozza senza alcun flusso di lavoro allegato e applica le impostazioni di bozza predefinite. Puoi aggiornare le impostazioni di correzione predefinite o aggiungere un flusso di lavoro dopo aver creato la bozza. Per ulteriori informazioni sulle impostazioni della bozza, vedi <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modifica impostazioni bozza</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prove avanzate</strong></td> 
      <td> <p>Questa opzione consente di configurare un flusso di lavoro di base o avanzato e di modificare le impostazioni di bozza per la bozza creata. Per ulteriori informazioni, consulta </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Creare una bozza avanzata con un flusso di lavoro di base</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Creare una bozza avanzata con un flusso di lavoro automatizzato</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gestire una bozza esistente

Una volta creata una prova, puoi fare cose come

* Visualizza l’attività della fase corrente
* Aggiornare i revisori e le scadenze
* Modificare il flusso di lavoro

Per ulteriori informazioni su come gestire una bozza esistente, consulta [Gestione delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Rivedi una bozza

I revisori assegnati possono eseguire operazioni quali

* Visualizzare la risorsa ed effettuare commenti
* Aggiungere azioni ai commenti
* Confronto delle versioni
* Approvare o rifiutare la prova

Per ulteriori informazioni sulle operazioni che è possibile eseguire con lo strumento di correzione, consulta [Revisione delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

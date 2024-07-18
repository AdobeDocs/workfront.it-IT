---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Prova di una risorsa collegata per Experience Manager Assets o Assets Essentials
description: Dopo aver collegato una risorsa da Experience Manager Assets Essentials, puoi creare una bozza e assegnare gli utenti per rivederla e aggiungere commenti alla risorsa.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# Prova di una risorsa collegata per Experience Manager Assets o Assets Essentials

Dopo aver collegato una risorsa da Experience Manager Assets Essentials, puoi creare una bozza e assegnare gli utenti per rivederla e aggiungere commenti alla risorsa.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p>
   <p>È necessario che la verifica sia abilitata per l'utente.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi disporre di Assets Essentials di Experience Manager as a Cloud Service e devi essere aggiunto al prodotto come utente nell’Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare Experience Manager Assets as a Cloud Service Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Crea una bozza

Puoi creare bozze statiche, video o interattive.

Per creare una bozza:

1. Vai al progetto, all&#39;attività o al problema in cui desideri la bozza, quindi fai clic sulla sezione **Documenti**.
1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Scegliere una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Bozza semplice</strong></td> 
      <td>Questa opzione crea una bozza senza alcun flusso di lavoro associato e applica le impostazioni predefinite della bozza. Dopo aver creato la bozza, è possibile aggiornare le impostazioni predefinite delle bozze o aggiungere un flusso di lavoro. Per ulteriori informazioni sulle impostazioni della bozza, vedere <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modifica impostazioni bozza</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bozza avanzata</strong></td> 
      <td> <p>Questa opzione consente di configurare un flusso di lavoro di base o avanzato e di modificare le impostazioni della bozza creata. Per ulteriori informazioni, consulta </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Crea una bozza avanzata con un flusso di lavoro di base</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Crea una bozza avanzata con un flusso di lavoro automatizzato</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gestire una bozza esistente

Dopo aver creato una bozza, puoi eseguire operazioni come

* Visualizza attività fase corrente
* Aggiorna revisori e scadenze
* Modificare il flusso di lavoro

Per ulteriori informazioni su come gestire una bozza esistente, vedi [Gestione delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Rivedere una bozza

I revisori assegnati possono eseguire operazioni come

* Visualizzare la risorsa e fare commenti
* Aggiungere azioni ai commenti
* Confronta versioni
* Approvare o rifiutare la bozza

Per ulteriori informazioni sulle operazioni che è possibile eseguire con lo strumento di correzione, vedere [Verifica delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

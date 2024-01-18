---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza per un documento
description: È possibile generare una bozza per un documento nel momento in cui viene caricato in Workfront. Puoi anche generare una bozza per un documento già caricato in Adobe Workfront o per una nuova versione di una bozza già in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: c3bbcaff2643bff43d0c26ee97d2a4ba22680a30
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Creare una bozza per un documento

È possibile generare una bozza per un documento nel momento in cui viene caricato in Workfront.

Puoi anche generare una bozza per un documento già caricato in Adobe Workfront o per una nuova versione di una bozza già in Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> 
   <p>Nuovo: Qualsiasi </p>
   <p>Corrente: Pro o superiore</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Nuovo: Standard</p>
   <p>Corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Caricare un documento e creare una bozza

1. Vai al progetto, all’attività o al problema in cui desideri creare una nuova bozza.
1. Fai clic su **Documenti** scheda.
1. Fare clic su Documenti ![](assets/document-icon.png) nel pannello a sinistra.
1. Clic **Aggiungi nuovo**, quindi fai clic su **Bozza** nel menu visualizzato.

   >[!TIP]
   >
   >È possibile abilitare **Genera automaticamente delle bozze durante il caricamento dei documenti** nel profilo utente per automatizzare questo processo. Per ulteriori informazioni, consulta [Configura le mie impostazioni](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. In **Nuova bozza** pagina visualizzata, è possibile

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Caricare un documento e creare una nuova versione di una bozza

1. Vai al progetto, all’attività o al problema in cui desideri creare una nuova versione di una bozza esistente.
1. Fai clic su **Documenti** scheda.
1. Selezionare il documento in cui si desidera aggiungere una nuova versione.
1. Clic **Aggiungi nuovo** > **Versione** > **Bozza**.
1. In **Nuova versione bozza** pagina visualizzata, è possibile

   * [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Usa il trascinamento della selezione per generare una semplice bozza per una nuova versione

È possibile trascinare un documento dal file system (ad esempio dal desktop) per creare una nuova bozza o una nuova versione di una bozza esistente. La bozza contiene le seguenti impostazioni, a seconda che si stia creando una nuova bozza o una nuova versione:

* **Nuova bozza:** Crea una semplice bozza condivisa solo con te. Puoi modificare le impostazioni di condivisione dopo aver creato la bozza, come descritto in [Modifica impostazioni bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nuova versione della bozza esistente:** Crea una nuova versione con le stesse impostazioni di bozza della versione precedente.

Per generare una nuova bozza o una nuova versione della bozza mediante il trascinamento della selezione:

1. Assicurati che le bozze siano configurate per la generazione automatica, come descritto in .
1. Continua con  [Aggiungere documenti ad Adobe Workfront dal file system](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), che illustra il metodo di trascinamento della selezione per l&#39;aggiunta di documenti. 

## Creare una bozza per un documento esistente

1. Vai al progetto, all’attività o al problema nel punto in cui desideri inserire la bozza, quindi fai clic sul pulsante **Documenti** sezione.
1. Passa il puntatore del mouse sul documento, quindi fai clic su **Crea bozza** sotto il nome del documento.

   >[!NOTE]
   >
   >Se è stato **Genera automaticamente delle bozze durante il caricamento dei documenti** nel tuo profilo utente, il sistema crea automaticamente una semplice bozza.

1. Scegliere una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bozza semplice</td> 
      <td>Questa opzione crea una bozza senza alcun flusso di lavoro associato e applica le impostazioni predefinite della bozza. Dopo aver creato la bozza, è possibile aggiornare le impostazioni predefinite delle bozze o aggiungere un flusso di lavoro. Per ulteriori informazioni sulle impostazioni delle bozze, consulta <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modifica impostazioni bozza</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bozza avanzata</td> 
      <td> <p>Questa opzione consente di configurare un flusso di lavoro di base o avanzato e di modificare le impostazioni della bozza creata. Per ulteriori informazioni, consulta </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Creare una bozza avanzata con un flusso di lavoro di base</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Creare una bozza avanzata con un flusso di lavoro automatizzato</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

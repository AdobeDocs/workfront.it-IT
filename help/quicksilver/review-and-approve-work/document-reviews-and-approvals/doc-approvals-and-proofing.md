---
product-area: documents
navigation-topic: approvals
title: Utilizzare insieme approvazioni unificate e bozze
description: Puoi utilizzare le Approvazioni unificate con la verifica.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 1%

---

# Utilizzare insieme approvazioni unificate e bozze

Approvazioni unificate in Workfront introduce una nuova serie di funzioni per facilitare la revisione e l’approvazione dei documenti. È possibile utilizzare un flusso di lavoro Approvazioni unificate con il visualizzatore di bozze esistente per aggiungere commenti e markup ai documenti in revisione.

Esistono alcune differenze chiave nel flusso di lavoro quando si utilizzano insieme le approvazioni unificate e la verifica:

* I partecipanti vengono visualizzati nel riepilogo del documento, non nel flusso di lavoro di verifica.

* I dettagli Inviato, Aperto, Commento, Decisione (SOCD) nell’elenco dei documenti sono correlati alle verifiche e non riflettono lo stato della decisione del documento.

## Caricare un documento e creare una bozza

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.
Oppure
Trascinare il documento nell&#39;elenco dei documenti.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento e seleziona **Bozza semplice**. È necessario creare una bozza semplice perché non utilizzerai il flusso di lavoro di bozza per le approvazioni.

Gli utenti assegnati come partecipanti possono utilizzare il visualizzatore di bozze per aggiungere commenti e markup al documento. Passare alla sezione successiva per scoprire come aggiungere partecipanti di revisione.

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Aprire il documento Riepilogo e assegnare i partecipanti

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per assegnare i partecipanti:

1. Seleziona il documento caricato e apri il Riepilogo del documento.

   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Fai clic su **Richiedi approvazione**. I partecipanti vengono informati via e-mail.

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Crea una nuova versione in base alle esigenze

Se hai bisogno di un altro ciclo di revisione e approvazione, puoi creare una nuova versione della bozza e aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nel Riepilogo del documento.

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per aggiungere una nuova versione:

1. Trascinare e rilasciare il nuovo file sopra il documento precedente in Workfront. Workfront crea automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionarlo e fare clic su **Crea bozza** > **Bozza semplice**.

1. Selezionare nuovamente il documento, quindi aprire il documento Riepilogo.

   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Fai clic su **Richiedi approvazione**. I partecipanti vengono informati via e-mail.

## Verifica la bozza e prendi una decisione

Il documento non passa a uno stato approvato finché tutti gli approvatori assegnati non scelgono &quot;approvato&quot;.

Per rivedere e approvare un documento:

1. Vai alla notifica e-mail di revisione e fai clic su **Vai alla revisione**.

1. Una volta in Workfront, fai clic su **Vai alla bozza**.

1. Rivedi il contenuto e aggiungi eventuali commenti o markup. Per ulteriori informazioni sull&#39;utilizzo del visualizzatore di bozze, vedere [Rivedere le bozze in Adobe Workfront: article index](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Scegli una delle seguenti decisioni:

   * **Approva**: il documento non necessita di modifiche ed è pronto per l&#39;uso.
   * **Approva con modifiche**: il documento richiede modifiche ed è pronto per l&#39;uso una volta apportate. Non è necessaria un&#39;ulteriore approvazione.
   * **Lavoro necessario**: il documento richiede modifiche e non è pronto per l&#39;uso. Dopo aver apportato le modifiche specificate, il documento deve essere caricato come nuova versione e superare un altro ciclo di approvazioni. Per ulteriori informazioni sul caricamento di una nuova versione, vedere [Creare una nuova versione in base alle esigenze](#create-a-new-version-as-needed) in questo articolo.

Una volta presa una decisione, il proprietario del documento riceve una notifica tramite e-mail.
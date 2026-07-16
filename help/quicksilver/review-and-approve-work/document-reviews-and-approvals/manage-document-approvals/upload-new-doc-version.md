---
product-area: documents
navigation-topic: approvals
title: Caricare una nuova versione del documento e richiedere un’approvazione
description: Puoi caricare una nuova versione del documento e richiedere l’approvazione di altri utenti in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 7%

---

# Caricare una nuova versione del documento e richiedere un’approvazione

Se un documento è contrassegnato come &quot;Da lavorare&quot; in una revisione precedente, è possibile caricare una nuova versione nel documento originale e avviare un altro ciclo di approvazioni. Dopo aver caricato una nuova versione del documento, le versioni precedenti vengono bloccate.

Se il nome del file della nuova versione è diverso da quello della versione precedente, Workfront visualizza il documento con il nome più recente.

Quando si aggiunge una nuova versione a un documento con approvazioni in sospeso, l’approvazione della versione precedente viene visualizzata come &quot;Ritirata&quot;. Il precedente processo di approvazione si chiude, anche se alcuni partecipanti non hanno ancora preso una decisione.

Se la versione più recente del documento viene eliminata, le versioni precedenti rimangono bloccate. Se devi modificare una versione precedente, devi sbloccarla manualmente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> <p>Richiedente o successiva</p>
   <p>Collaboratore o successiva</p>
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Modifica l'accesso all'oggetto associato al documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

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



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## Usa il trascinamento della selezione per aggiungere una nuova versione nell’area dei documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.

Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront. È possibile aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nella pagina Dettagli documento.

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per aggiungere una nuova versione e richiedere l’approvazione:

1. Passare al documento in Workfront.

1. Trascinare il nuovo file sopra il documento precedente. Workfront crea automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo documento. Il numero di versione viene visualizzato nella parte superiore del pannello.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Per copiare gli stessi revisori e approvatori dalla versione precedente del documento, fare clic su **Copia**.
1. Fai clic su **Richiedi approvazione**.

   Il flusso di lavoro di approvazione viene avviato e gli approvatori ricevono una notifica che indica che la loro approvazione è necessaria per la nuova versione del documento. La versione precedente del documento è bloccata e tutte le approvazioni in sospeso relative alla versione precedente vengono ritirate.

## Usa il trascinamento della selezione per aggiungere una nuova versione nella nuova area Documenti

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.

Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront. È possibile aggiungere un flusso di lavoro di approvazione alla nuova versione del documento.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per aggiungere una nuova versione e richiedere l’approvazione:

1. Passare al documento in Workfront.

1. Trascinare il nuovo file sopra il documento precedente. Workfront crea automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo. La versione più recente del documento è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Per copiare gli stessi revisori e approvatori dalla versione precedente del documento, fare clic su **Copia**.
1. Fai clic su **Richiedi approvazione**.

   Il flusso di lavoro di approvazione viene avviato e gli approvatori ricevono una notifica che indica che la loro approvazione è necessaria per la nuova versione del documento. La versione precedente del documento è bloccata e tutte le approvazioni in sospeso relative alla versione precedente vengono ritirate.

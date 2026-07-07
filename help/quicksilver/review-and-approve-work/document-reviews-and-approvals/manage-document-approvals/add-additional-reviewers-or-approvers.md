---
product-area: documents
navigation-topic: approvals
title: Aggiungere altri approvatori o revisori a un flusso di lavoro di approvazione dei documenti
description: È possibile aggiungere ulteriori approvatori o revisori a un documento che dispone già di approvazioni in sospeso.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 82530b9b87f6865ec294adcdc601443ee48dcbcf
workflow-type: tm+mt
source-wordcount: 1130
ht-degree: 3%

---

# Aggiungere altri approvatori o revisori a un flusso di lavoro di approvazione dei documenti

{{highlighted-preview}}

È possibile aggiungere altri approvatori o revisori a un flusso di lavoro di approvazione di un documento che dispone già di approvazioni in sospeso.

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedere gli articoli elencati in [Approvazioni di lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Collaboratore o successiva</p>
   <p>Revisione o successiva</p> 
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard, calendari e documenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione o accesso successivo all’oggetto associato alla richiesta di accesso o approvazione </p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Aggiungere ulteriori approvatori o revisori nell&#39;area dei documenti legacy in Produzione

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Per aggiungere altri approvatori o revisori dal Riepilogo documento:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Selezionare la versione del documento a cui si desidera aggiungere un approvatore o un revisore nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Modifica flusso di lavoro**.

   ![modifica flusso di lavoro di approvazione](assets/edit-approval-in-legacy.png)

1. Individua la fase a cui desideri aggiungere approvatori o revisori, quindi aggiungi il nome o l’e-mail dell’utente nella casella di testo. Se necessario, puoi anche aggiungere un intero team.

1. Una volta aggiunto il nome, scegliere se si tratta di un approvatore o di un revisore.

   ![elenco a discesa approvatore o revisore](assets/choose-approver-or-reviewer.png)

1. Ripetere i passaggi 5-6 per aggiungere altri approvatori o revisori.Dopo il salvataggio, i partecipanti aggiunti ricevono una notifica e-mail che indica che per il documento è necessaria la loro approvazione o revisione.

<div class="preview">

## Aggiungere ulteriori approvatori o revisori nell&#39;area dei documenti legacy in Anteprima

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Per aggiungere altri approvatori o revisori dal Riepilogo documento:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento desiderato. Viene visualizzato il pannello Riepilogo documento relativo al documento.

1. Selezionare la versione del documento a cui si desidera aggiungere un approvatore o un revisore nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Modifica flusso di lavoro**. La finestra di dialogo Richiedi approvazione si apre nella modalità in cui è stata salvata l’ultima approvazione: Base per le approvazioni in una sola fase o Avanzate per le approvazioni in più fasi e le approvazioni con percorsi paralleli.

1. Aggiungi l’utente, il team o l’e-mail:

   * In modalità Base, digita il nome o l&#39;e-mail nel campo **Aggiungi nomi o e-mail**.
   * In modalità avanzata, seleziona il percorso che contiene la fase da aggiornare, quindi digita il nome o l&#39;e-mail nel campo **Aggiungi nomi o e-mail** della fase.

1. Per ogni persona aggiunta, scegliere se si tratta di un approvatore o revisore.

   ![elenco a discesa approvatore o revisore](assets/choose-reviewer-or-approver.png)

1. Fai clic su **Salva**. I partecipanti aggiunti ricevono una notifica e-mail che indica che per il documento è necessaria la loro approvazione o revisione.

>[!TIP]
>
>Per ristrutturare un&#39;approvazione in modalità Base in un&#39;approvazione a più fasi o a percorsi multipli, fare clic su **Vai all&#39;approvazione avanzata** nell&#39;angolo superiore destro. I partecipanti esistenti vengono mantenuti come Percorso 1, Fase 1. Dopo il salvataggio, non è possibile tornare alla modalità Base. Per ulteriori dettagli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

</div>

## Aggiungere ulteriori approvatori o revisori nella nuova area Documenti in Produzione

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)


1. Fare clic su **Modifica flusso di lavoro**.

1. Individua la fase a cui desideri aggiungere approvatori o revisori, quindi aggiungi il nome o l’e-mail dell’utente nella casella di testo. Se necessario, puoi anche aggiungere un intero team.

1. Una volta aggiunto il nome, scegliere se si tratta di un approvatore o di un revisore.

   ![elenco a discesa approvatore o revisore](assets/choose-approver-or-reviewer.png)

1. Ripetere i passaggi 5-6 per aggiungere altri approvatori o revisori.Dopo il salvataggio, i partecipanti aggiunti ricevono una notifica e-mail che indica che per il documento è necessaria la loro approvazione o revisione.

<div class="preview">

## Aggiungere ulteriori approvatori o revisori dal Riepilogo documento nella nuova area Documenti in Anteprima

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per aggiungere altri approvatori o revisori dal Riepilogo documento:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fare clic su **Modifica flusso di lavoro**. La finestra di dialogo Richiedi approvazione si apre nella modalità in cui è stata salvata l’ultima approvazione: Base per le approvazioni in una sola fase o Avanzate per le approvazioni in più fasi e le approvazioni con percorsi paralleli.

1. Aggiungi l’utente, il team o l’e-mail:

   * In modalità Base, digita il nome o l&#39;e-mail nel campo **Aggiungi nomi o e-mail**.
   * In modalità avanzata, seleziona il percorso che contiene la fase da aggiornare, quindi digita il nome o l&#39;e-mail nel campo **Aggiungi nomi o e-mail** della fase.

1. Per ogni persona aggiunta, scegliere se si tratta di un approvatore o revisore.

   ![elenco a discesa approvatore o revisore](assets/choose-reviewer-or-approver.png)

1. Fai clic su **Salva**. I partecipanti aggiunti ricevono una notifica e-mail che indica che per il documento è necessaria la loro approvazione o revisione.

>[!TIP]
>
>Per ristrutturare un&#39;approvazione in modalità Base in un&#39;approvazione a più fasi o a percorsi multipli, fare clic su **Vai all&#39;approvazione avanzata** nell&#39;angolo superiore destro. I partecipanti esistenti vengono mantenuti come Percorso 1, Fase 1. Dopo il salvataggio, non è possibile tornare alla modalità Base. Per ulteriori dettagli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

</div>
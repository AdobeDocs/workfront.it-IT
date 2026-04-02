---
product-area: documents
navigation-topic: approvals
title: Creare un flusso di lavoro di approvazione documento
description: Puoi richiedere l’approvazione di altri utenti per un documento in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 4%

---

# Creare un flusso di lavoro di approvazione documento

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

Puoi richiedere l’approvazione di un documento in Adobe Workfront ad altri utenti o team, oppure chiedere loro di rivedere un documento senza doverlo approvare.

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedere gli articoli elencati in [Approvazioni di lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
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
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard e calendari, documenti</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Creare una richiesta di revisione o approvazione del documento dalla pagina del documento nell’ambiente di produzione

1. Passa il puntatore del mouse sul documento, quindi fai clic su Dettagli documento.
   ![Dettagli documento](assets/doc-details.png)

1. Accanto al nome del documento, seleziona la versione del documento per cui desideri creare un’approvazione nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Fai clic su **Approvazioni** nel pannello a sinistra.

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un responsabile approvazione, fare clic su **Responsabile approvazione** e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, selezionare la casella di controllo **Revisore** e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatore e scadenza](assets/add-approver-and-deadline.png)

1. Ripeti il passaggio precedente per aggiungere altri approvatori o revisori.

## Creare una richiesta di revisione o approvazione del documento dal pannello Riepilogo documento nell’ambiente di produzione

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.

1. Fare clic sul documento desiderato e viene aperto il pannello a sinistra Riepilogo documento per tale documento.

1. Seleziona la versione del documento per cui desideri creare un’approvazione nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel riquadro Riepilogo documento, quindi fai clic su **Aggiungi**.

![Aggiungi approvatori nel riepilogo documenti](assets/doc-summary-add-approvers.png)

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un responsabile approvazione, fare clic su **Responsabile approvazione** e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, selezionare la casella di controllo **Revisore** e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatore e scadenza](assets/add-approver-and-deadline.png)

1. Ripeti il passaggio precedente per aggiungere altri approvatori o revisori.

<div class="preview">

## Creare un flusso di lavoro di approvazione dal pannello Riepilogo nell’ambiente di anteprima nell’area documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Archiviazione Workfront e archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Per creare un flusso di lavoro di approvazione:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Seleziona la versione del documento per cui desideri creare un’approvazione nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**.


1. Compila i seguenti dettagli:

   <table>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Aggiungete un nome di fase. È possibile modificare il nome in modo che sia più descrittivo, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.</td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (opzionale)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Data di scadenza (facoltativo)</strong></td>
   <td>Imposta una data di scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della data di scadenza specificata.</td>
   </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altre fasi in base alle esigenze.

   >[!NOTE]
   >
   >Se aggiungi più fasi, il flusso di lavoro di approvazione procede nell’ordine in cui sono elencate. Quando tutte le decisioni necessarie vengono prese, inizia la fase successiva e la fase precedente viene bloccata.

   ![Dettagli documento](assets/new-stage.png)

</div>

## Creare un flusso di lavoro di approvazione dal pannello Riepilogo nella nuova area del documento

Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per creare un flusso di lavoro di approvazione:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi sull’icona Approvazioni a destra della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fai clic su **Crea flusso di lavoro**, quindi compila i seguenti dettagli:

   <table>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Aggiungete un nome di fase. È possibile modificare il nome in modo che sia più descrittivo, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.</td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (opzionale)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Data di scadenza (facoltativo)</strong></td>
   <td>Imposta una data di scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della data di scadenza specificata.</td>
   </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altre fasi in base alle esigenze.

   >[!NOTE]
   >
   >Se aggiungi più fasi, il flusso di lavoro di approvazione procede nell’ordine in cui sono elencate. Quando tutte le decisioni necessarie vengono prese, inizia la fase successiva e la fase precedente viene bloccata.

   ![Dettagli documento](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->

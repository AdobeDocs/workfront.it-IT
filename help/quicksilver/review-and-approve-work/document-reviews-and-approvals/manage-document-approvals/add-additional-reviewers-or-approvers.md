---
product-area: documents
navigation-topic: approvals
title: Aggiungere altri approvatori o revisori a un flusso di lavoro di approvazione dei documenti
description: È possibile aggiungere ulteriori approvatori o revisori a un documento che dispone già di approvazioni in sospeso.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 6%

---

# Aggiungere altri approvatori o revisori a un flusso di lavoro di approvazione dei documenti

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
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni utilizzando lo storage aziendale Adobe</p> </td> 
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



## Aggiungere ulteriori approvatori o revisori dal Riepilogo documento nell&#39;area documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Archiviazione Workfront e archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Per aggiungere altri approvatori o revisori dal Riepilogo documento:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Selezionare la versione del documento a cui si desidera aggiungere un approvatore o un revisore nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Modifica flusso di lavoro**.

   ![modifica flusso di lavoro di approvazione](assets/edit-approval-in-legacy.png)

1. Individua la fase a cui desideri aggiungere approvatori o revisori, quindi aggiungi il nome o l’e-mail dell’utente nella casella di testo. Se necessario, puoi anche aggiungere un intero team.

1. Una volta aggiunto il nome, scegliere se si tratta di un approvatore o di un revisore.

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
Once you save, the participants added receive an email notification that their approval or review is needed on the document.



## Add additional approvers or reviewers from the Document Summary in the new documents area

Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)


1. Fare clic su **Modifica flusso di lavoro**.

1. Individua la fase a cui desideri aggiungere approvatori o revisori, quindi aggiungi il nome o l’e-mail dell’utente nella casella di testo. Se necessario, puoi anche aggiungere un intero team.

1. Una volta aggiunto il nome, scegliere se si tratta di un approvatore o di un revisore.

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
Once you save, the participants added receive an email notification that their approval or review is needed on the document.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->

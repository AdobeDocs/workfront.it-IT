---
product-area: documents
navigation-topic: approvals
title: Rimuovere approvatori o revisori da un flusso di lavoro di approvazione documento
description: È possibile rimuovere singoli approvatori o revisori da un documento.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 6%

---

# Rimuovere approvatori o revisori da un flusso di lavoro di approvazione documento

È possibile rimuovere singoli approvatori o revisori da una risorsa o da un documento dopo averli assegnati.

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
   <td> <p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni utilizzando lo storage aziendale Adobe</p>  </td> 
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
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Rimuovere approvatori o revisori da un flusso di lavoro di approvazione nell&#39;area documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Archiviazione Workfront e archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Per rimuovere approvatori o revisori da un flusso di lavoro di approvazione:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel pannello Riepilogo documento.

1. Fare clic su **Modifica flusso di lavoro**.

1. Individua il partecipante che desideri rimuovere, quindi fai clic sull&#39;icona **Rimuovi** accanto al nome.

   La richiesta di approvazione o di revisione viene rimossa e l&#39;approvatore riceve una notifica che indica che la sua approvazione non è più necessaria. Viene rimosso anche l’accesso condiviso relativo all’approvazione.

   ![modifica flusso di lavoro di approvazione](assets/edit-approval-in-legacy.png)

1. (Facoltativo) Per cambiare il ruolo di un approvatore in revisore o viceversa, fare clic sul menu a discesa accanto al nome utente e selezionare il nuovo ruolo.

1. Repeat the previous step to remove any additional approvers or reviewers.

</div>


## Remove approvers or reviewers to an approval workflow in the new document area

Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per creare un flusso di lavoro di approvazione:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)


1. Fare clic su **Modifica flusso di lavoro**.

1. Individua il partecipante che desideri rimuovere, quindi fai clic sull&#39;icona **Rimuovi** accanto al nome.

   La richiesta di approvazione o di revisione viene rimossa e l&#39;approvatore riceve una notifica che indica che la sua approvazione non è più necessaria.

1. (Facoltativo) Per cambiare il ruolo di un approvatore in revisore o viceversa, fare clic sul menu a discesa accanto al nome utente e selezionare il nuovo ruolo.

1. Repeat the previous step to remove any additional approvers or reviewers.

   ![remove participants from a stage](assets/add-or-remove-participants.png)

1. Fai clic su **Salva**.
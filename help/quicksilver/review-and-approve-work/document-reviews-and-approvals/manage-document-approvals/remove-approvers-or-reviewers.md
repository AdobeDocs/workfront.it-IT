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
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 4%

---

# Rimuovere approvatori o revisori da un flusso di lavoro di approvazione documento

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

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
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Rimuovere gli approvatori o i revisori dalla pagina Dettagli documento nell’ambiente di produzione

1. Vai alla pagina del documento facendo clic sul nome del documento, quindi seleziona la versione del documento per la quale desideri rimuovere un’approvazione nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Seleziona **Approvazioni** nel pannello a sinistra.

1. Passa il puntatore del mouse sul nome dell&#39;approvatore o del revisore che desideri rimuovere, quindi fai clic sull&#39;icona **Elimina** ![Elimina](../assets/delete.png) che compare dopo il nome.

   La richiesta di approvazione o di revisione viene rimossa e l&#39;approvatore riceve una notifica che indica che la sua approvazione non è più necessaria. Viene rimosso anche l’accesso condiviso relativo all’approvazione.

1. (Facoltativo) Per abbassare di livello un approvatore a revisore anziché rimuoverlo completamente, deselezionare la casella di controllo **Approvatore** in base al nome.

1. Ripeti il passaggio precedente per rimuovere eventuali approvatori o revisori aggiuntivi.

## Rimuovere gli approvatori o i revisori dal Riepilogo documento nell’ambiente di produzione

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Selezionare la versione del documento per la quale si desidera rimuovere un approvatore o un revisore nel menu a discesa della versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel pannello Riepilogo documento. Passa il puntatore del mouse sul nome dell&#39;approvatore o del revisore che desideri rimuovere, quindi fai clic sull&#39;icona **Elimina** ![Elimina](../assets/delete.png) che compare dopo il nome.

   La richiesta di approvazione o di revisione viene rimossa e l&#39;approvatore riceve una notifica che indica che la sua approvazione non è più necessaria. Viene rimosso anche l’accesso condiviso relativo all’approvazione.

1. (Facoltativo) Per abbassare di livello un approvatore a revisore anziché rimuoverlo completamente, deselezionare la casella di controllo **Approvatore** in base al nome.

1. Ripeti il passaggio precedente per rimuovere eventuali approvatori o revisori aggiuntivi.


<div class="preview">

## Rimuovere approvatori o revisori da un flusso di lavoro di approvazione nell’ambiente di anteprima nell’area documenti legacy

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

1. Ripeti il passaggio precedente per rimuovere eventuali approvatori o revisori aggiuntivi.

</div>


## Rimuovere approvatori o revisori da un flusso di lavoro di approvazione nella nuova area del documento

Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per creare un flusso di lavoro di approvazione:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)


1. Fare clic su **Modifica flusso di lavoro**.

1. Individua il partecipante che desideri rimuovere, quindi fai clic sull&#39;icona **Rimuovi** accanto al nome.

   La richiesta di approvazione o di revisione viene rimossa e l&#39;approvatore riceve una notifica che indica che la sua approvazione non è più necessaria.

1. (Facoltativo) Per cambiare il ruolo di un approvatore in revisore o viceversa, fare clic sul menu a discesa accanto al nome utente e selezionare il nuovo ruolo.

1. Ripeti il passaggio precedente per rimuovere eventuali approvatori o revisori aggiuntivi.

   ![rimuovere partecipanti da una fase](assets/add-or-remove-participants.png)
1. Fai clic su **Salva**.
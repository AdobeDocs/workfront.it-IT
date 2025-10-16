---
product-area: documents
navigation-topic: approvals
title: Creare una richiesta di revisione o approvazione documento
description: Puoi richiedere l’approvazione di altri utenti per un documento in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Creare una richiesta di revisione o approvazione documento

Puoi richiedere l’approvazione di un documento in Adobe Workfront ad altri utenti o team, oppure chiedere loro di rivedere un documento senza doverlo approvare.

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedere gli articoli elencati in [Approvazioni di lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td>  
   <td>
   <p>Collaboratore o versione successiva</p>
   <p>Revisione o successiva</p>
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard e calendari, documenti</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una richiesta di revisione o approvazione documento dalla pagina del documento

1. Passa il puntatore del mouse sul documento, quindi fai clic su Dettagli documento.
   ![Dettagli documento](assets/doc-details.png)

1. Accanto al nome del documento, seleziona la versione del documento per cui desideri creare un’approvazione nel menu a discesa della versione. Per impostazione predefinita, viene selezionata la versione più recente.

1. Fai clic su **Approvazioni** nel riquadro a sinistra.

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un responsabile approvazione, fare clic su **Responsabile approvazione** e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, selezionare la casella di controllo **Revisore** e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatore e scadenza](assets/add-approver-and-deadline.png)

1. Ripeti il passaggio precedente per aggiungere altri approvatori o revisori.

## Creare una richiesta di revisione o approvazione del documento dal pannello Riepilogo documento

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.

1. Fare clic sul documento necessario per aprire il riquadro Riepilogo documento per il documento.

1. Seleziona la versione del documento per cui desideri creare un’approvazione nel menu a discesa della versione. Per impostazione predefinita, viene selezionata la versione più recente.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel riquadro Riepilogo documento, quindi fai clic su **Aggiungi**.

![Aggiungi approvatori nel riepilogo documenti](assets/doc-summary-add-approvers.png)

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un responsabile approvazione, fare clic su **Responsabile approvazione** e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, selezionare la casella di controllo **Revisore** e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatore e scadenza](assets/add-approver-and-deadline.png)

1. Ripeti il passaggio precedente per aggiungere altri approvatori o revisori.





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->

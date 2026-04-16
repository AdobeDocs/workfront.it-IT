---
product-area: documents
navigation-topic: approvals
title: Creare un modello di flusso di lavoro di approvazione per i documenti
description: Puoi creare modelli di approvazione per semplificare il processo di approvazione.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 14%

---

# Creare un modello di flusso di lavoro di approvazione per i documenti

Nell’area Configurazione di Workfront, gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili. Una volta creati, i modelli di approvazione possono essere applicati alle risorse nell’area Documenti di un progetto, un’attività o un problema.

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
   <td> <p>Standard</p> 
   <p>Piano</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
ß

## Creare un modello di approvazione

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Revisione e approvazione** > **Modelli di approvazione**.
1. Fai clic su **Nuovo modello** sul lato destro della pagina.

1. Compila i seguenti dettagli:

   <table>
     <tr>
   <td><strong>Nome modello</strong></td>
   <td>Aggiungi un nome modello. </td>
   </tr>
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
   <td><strong>Giornate di lavoro fino alla data di scadenza</strong></td>
   <td>Scegli quanti giorni lavorativi mancano alla scadenza dell’approvazione dopo l’attivazione di una fase.</td>
   </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altre fasi in base alle esigenze.

   >[!NOTE]
   >
   >Se aggiungi più fasi, il flusso di lavoro di approvazione procede nell’ordine in cui sono elencate. Quando tutte le decisioni necessarie vengono prese, inizia la fase successiva e la fase precedente viene bloccata.

   ![Dettagli documento](assets/new-stage.png)

1. Fai clic su **Salva**.

Una volta creato, il modello può essere applicato ai documenti nell’area Documenti di un progetto, un’attività o un problema per avviare il processo formale di revisione e approvazione in Workfront.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->

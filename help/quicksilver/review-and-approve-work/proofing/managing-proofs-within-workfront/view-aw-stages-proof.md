---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Visualizzare le fasi del flusso di lavoro automatizzato su una bozza
description: Puoi tenere traccia dell’avanzamento di una bozza configurata con un flusso di lavoro automatizzato. È possibile visualizzare, modificare, aggiungere, avviare e bloccare il lavoro già eseguito sugli stadi della bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Visualizzare le fasi del flusso di lavoro automatizzato su una bozza

Puoi tenere traccia dell’avanzamento di una bozza configurata con un flusso di lavoro automatizzato. È possibile visualizzare, modificare, aggiungere, avviare e bloccare il lavoro già eseguito sugli stadi della bozza.

Per informazioni sull’aggiunta di fasi e utenti a una bozza con un flusso di lavoro automatizzato, consulta [Aggiungere fasi e utenti a un flusso di lavoro automatizzato su una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Visualizza il diagramma del flusso di lavoro automatizzato

1. Posizionare il puntatore del mouse sulla riga contenente il documento in un elenco di documenti contenente il documento, quindi fare clic su **Flusso di lavoro di correzione**.

   Il diagramma del flusso di lavoro automatizzato viene visualizzato sotto il titolo del flusso di lavoro.

   Le fasi del diagramma sono contrassegnate come segue:

   ![dot.png](assets/dot.png) Fase attiva

   ![grigio_punto.png](assets/grey-dot.png) Fase inattiva\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Stage privato

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Stage bloccato

   Le linee tra gli stadi rappresentano le dipendenze tra gli stadi. Le linee che conducono agli stadi inattivi vengono punteggiate fino a quando lo stadio non viene attivato.

   Puoi passare il cursore sopra una fase del diagramma per visualizzarne l’avanzamento. Se l’area di visualizzazione non è attiva e si dispone dei diritti di modifica nell’area di visualizzazione, è possibile fare clic sul pulsante Attiva area di visualizzazione ![](assets/activate-stage-btn.png) per iniziare lo stage. Se l’area di visualizzazione è attiva e si dispone dei diritti di modifica sull’area di visualizzazione, è possibile bloccarla. ![](assets/lock-stage-btn.png) Per ulteriori informazioni sulla barra di avanzamento (S, O, C, D) , consulta  [Visualizzazione dell&#39;avanzamento e dello stato di una bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Visualizzare un’area di visualizzazione

1. Posizionare il puntatore del mouse sulla riga contenente il documento in un elenco di documenti contenente il documento, quindi fare clic su **Flusso di lavoro di correzione**.
1. Nel diagramma fare clic sull’area di visualizzazione che si desidera visualizzare.

   ![](assets/view-stage-diagram-350x204.png)

1. Per espandere i dettagli di un’area di visualizzazione, fai clic sulla freccia laterale sotto il nome corrispondente.

   ![](assets/stage-details-caret-350x167.png)

## Visualizza tutti gli stadi

Per visualizzare tutte le fasi di un flusso di lavoro automatizzato:

1. Fai clic sul pulsante Cambia visualizzazione nella parte superiore della pagina ![](assets/change-view-btn.png), quindi fai clic su **Visualizza tutti gli stadi**.

   Tutte le fasi del flusso di lavoro automatizzato sono elencate nella sezione , tuttavia i dettagli sono nascosti.

1. Per espandere i dettagli di un’area di visualizzazione, fai clic sulla freccia laterale sotto il nome corrispondente.

## Visualizzare in dettaglio tutte le fasi

Per visualizzare tutte le fasi del flusso di lavoro automatizzato con i relativi dettagli espansi:

1. Fai clic sul pulsante Cambia visualizzazione nella parte superiore della pagina ![](assets/change-view-btn.png), quindi fai clic su **Visualizzare in dettaglio tutte le fasi**.
1. Per visualizzare i dettagli di un’area di visualizzazione, fai clic sulla freccia rivolta verso il basso sotto il nome.

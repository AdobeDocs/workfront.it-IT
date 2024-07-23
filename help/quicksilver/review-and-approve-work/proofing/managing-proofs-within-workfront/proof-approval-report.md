---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Utilizzare il rapporto di approvazione della bozza
description: È possibile utilizzare il rapporto Approvazione bozza per visualizzare informazioni sulle bozze nel proprio ambiente.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 8a388ffa2d30683c08637a4273f628c553e55fdb
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 1%

---

# Utilizzare il rapporto di approvazione della bozza

È possibile utilizzare il rapporto Approvazione bozza per visualizzare informazioni sulle bozze nel proprio ambiente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>piano Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Panoramica sulle licenze di Adobe Workfront*</p> </td> 
   <td> <p>Piano</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Livello di accesso*</strong> </td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Utilizzare il rapporto di approvazione della bozza

{{step1-to-reports}}

1. Fai clic su **Nuovo rapporto**, quindi scorri per selezionare **Approvazione bozza**.

   ![](assets/proof-approval-report.png)

1. (Facoltativo) Aggiungi eventuali campi aggiuntivi.
1. Fai clic su **Salva e Chiudi**.

## Campi aggiuntivi

Puoi aggiungere i seguenti campi al rapporto di approvazione della bozza:

* **Data decisione**: visualizza la data in cui un approvatore prende una decisione su una bozza. Tale data è riportata anche nel Riepilogo stampa della bozza.
* **Fase approvatore**: visualizza le informazioni sulla fase corrente.
* **Modello flusso di lavoro**: visualizza tutti i modelli di flusso di lavoro allegati alla bozza. Se non è allegato alcun modello, la colonna è vuota.
* **In attesa della decisione**: visualizza true per segnalare che una decisione non è stata soddisfatta nella versione più recente quando si verificano le condizioni seguenti:

   * Bozza non archiviata
   * La fase in cui si trova l&#39;approvatore è attiva
   * La bozza è in attesa di approvazione

* **Scadenza bozza**: visualizza la scadenza della bozza. A ogni fase deve essere assegnata una scadenza affinché questo campo possa essere compilato. Nel campo viene visualizzata la scadenza per la fase attivata più di recente.

 

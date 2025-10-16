---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Utilizzare il rapporto di approvazione della bozza
description: È possibile utilizzare il rapporto Approvazione bozza per visualizzare informazioni sulle bozze nel proprio ambiente.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Utilizzare il rapporto di approvazione della bozza

È possibile utilizzare il rapporto Approvazione bozza per visualizzare informazioni sulle bozze nel proprio ambiente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacchetto Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenza Adobe Workfront</p> </td> 
   <td> 
   <p>Standard</p>
   <p>Piano</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong> </td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizzare il rapporto di approvazione della bozza

{{step1-to-reports}}

1. Fai clic su **Nuovo rapporto**, quindi scorri per selezionare **Approvazione bozza**.

   ![Rapporto approvazione bozza](assets/proof-approval-report.png)

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

 

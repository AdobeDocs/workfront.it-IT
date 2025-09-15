---
product-area: documents
navigation-topic: approvals
title: Carica una nuova versione del documento e richiedi un’approvazione
description: Puoi caricare una nuova versione del documento e richiedere l’approvazione di altri utenti in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 42fbb40cb8a0f3c70e22fd04bd3d0ce625f58fec
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Carica una nuova versione del documento e richiedi un’approvazione

Se un documento contrassegnato richiede un lavoro in una revisione precedente, puoi caricare una nuova versione nel documento originale e avviare un altro ciclo di approvazioni. Dopo aver caricato una nuova versione del documento, le versioni precedenti vengono bloccate.

Se il nome del file della nuova versione è diverso da quello della versione precedente, Workfront visualizza il documento con il nome più recente.

Quando si aggiunge una nuova versione a un documento con approvazioni in sospeso, l&#39;approvazione della versione precedente viene visualizzata come Ritirata. Il precedente processo di approvazione si chiude, anche se alcuni partecipanti non hanno ancora preso una decisione.

Se la versione più recente del documento viene eliminata, le versioni precedenti rimangono bloccate. Se devi modificare una versione precedente, devi sbloccarla manualmente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p>
   <p>Collaboratore o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modifica l'accesso all'oggetto associato al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usa il trascinamento per aggiungere una nuova versione

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.


Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront.

È possibile aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nella pagina Dettagli documento.

Per aggiungere una nuova versione:

1. Passare al documento in Workfront.
1. Trascinare il nuovo file sopra il documento precedente. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionarlo e fare clic su **Dettagli documento**.
   ![Aprire la pagina dei dettagli del documento](assets/open-doc-details.png)


1. Nel pannello a sinistra, fai clic su **Approvazioni**, quindi su **Aggiungi**.

1. Per aggiungere tutti i partecipanti precedenti, fare clic su **Aggiungi tutti**. È inoltre possibile aggiungere nuovi partecipanti o rimuovere i partecipanti precedenti in base alle esigenze.


1. Per aggiungere un modello di approvazione esistente, fai clic sul pulsante Modello e inizia a digitare il nome di un modello.

   >[!TIP]
   >
   >   Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, consulta [Creare un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

   ![invia nuova versione per l&#39;approvazione](assets/add-previous-participants.png)



---
product-area: documents
navigation-topic: manage-documents
title: Gestione delle versioni dei documenti
description: È possibile gestire più versioni di un documento in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Gestione delle versioni dei documenti

È possibile gestire più versioni di un documento in Workfront.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza l'accesso al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

* Questo articolo presuppone che il documento abbia più versioni.

   Per informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Visualizza un elenco di tutte le versioni di un documento

1. In Riepilogo, scorri fino alla visualizzazione del **Tutte le versioni** sezione . Qui è possibile visualizzare tutte le versioni del documento.

## Visualizzare e gestire i dettagli di una versione precedente del documento

1. Nella parte superiore della pagina Dettagli documento fare clic sul menu a discesa accanto al nome, quindi fare clic sul nome della versione che si desidera visualizzare e gestire.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Oltre a visualizzare i dettagli della versione, puoi apportare modifiche alla versione, ad esempio nome, metadati e impostazioni di correzione (se è una bozza del documento).

## Scaricare una singola versione di un documento

1. Nel riepilogo, alla voce **Versioni**, fai clic sul menu Altro ![](assets/more-icon.png) a destra della versione, quindi fai clic su **Scarica** nell’elenco a discesa visualizzato.

   ![](assets/more-versions-350x143.png)

## Scarica tutte le versioni di un documento

1. Fai clic su **Dettagli documento**, quindi seleziona **Tutte le versioni** nel pannello a sinistra.

1. Fai clic su **Scarica tutto** in cima all&#39;elenco.

## Eliminare una versione di un documento

Se si carica una versione di un documento per errore o se non è più necessaria una versione, è possibile eliminare la versione e mantenere il documento originale.

>[!IMPORTANT]
>
>Non è possibile recuperare una versione del documento eliminata singolarmente.

Quando si considera l&#39;eliminazione di una versione di un documento, tenere presente quanto segue:

* È possibile eliminare una sola versione alla volta. Se viene eliminata una versione, questa azione viene visualizzata nella **Aggiornamenti** sul documento .
* Se carichi una nuova versione dopo aver eliminato una versione, la nuova versione riceve il numero sequenziale successivo. Ad esempio, se sono presenti 3 versioni di un documento ed elimini la versione 3, il documento successivo caricato sarà la versione 4.
* Gli aggiornamenti di sistema e i commenti effettuati su una versione vengono conservati in Workfront dopo l’eliminazione della versione.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Per eliminare una versione del documento:

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.Trova il documento di cui hai bisogno.
1. In **Versione** nell&#39;area Riepilogo, fai clic sulla versione, quindi fai clic su **Elimina** nell’elenco a discesa visualizzato. La **Elimina** è visibile solo se sono presenti almeno due versioni.

   Se il documento è collegato a un&#39;origine esterna, il collegamento viene eliminato e il documento non è più accessibile tramite Workfront.

   ![](assets/more-versions-350x143.png)

---
product-area: documents
navigation-topic: manage-documents
title: Gestire le versioni dei documenti
description: In Workfront è possibile gestire più versioni di un documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Gestire le versioni dei documenti

<!-- Audited: 5/2025 -->

In Workfront è possibile gestire più versioni di un documento.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Nuovo: Collaboratore o versione successiva<p>
   <p>Oppure</p>
   <p>Corrente: richiesta o successiva </p>


</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizza accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* In questo articolo si presuppone che il documento abbia più versioni.

  Se hai bisogno di informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Visualizzare un elenco di tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Scorri verso il basso fino alla sezione **Versioni** per visualizzare tutte le versioni del documento.

## Visualizzare e gestire i dettagli di una versione precedente del documento

{{step1-to-documents}}

1. Passa il puntatore del mouse sul documento, quindi fai clic su **Dettagli documento**.

1. Nella parte superiore della pagina **Dettagli documento**, fare clic sul menu a discesa accanto al nome, quindi sul nome della versione che si desidera visualizzare e gestire.

   ![Elenco a discesa della versione nella pagina Dettagli documento](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Oltre a visualizzare i dettagli della versione, è possibile modificarla, ad esempio il nome, i metadati e le impostazioni di correzione (se si tratta di una bozza di documento).

## Scarica una versione di un singolo documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Nella sezione **Versioni**, fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra della versione, quindi fai clic su **Scarica** nell&#39;elenco a discesa visualizzato.

   ![Scarica un singolo documento](assets/more-versions-350x143.png)

## Scaricare tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Scorri verso il basso fino alla sezione **Versioni**, quindi fai clic su **Scarica tutto**.

## Eliminare una versione del documento

Se si carica una versione di un documento per errore o se una versione non è più necessaria, è possibile eliminare la versione e mantenere il documento originale.

>[!IMPORTANT]
>
>Non è possibile recuperare una versione del documento eliminata singolarmente.

Quando si considera di eliminare una versione di un documento, tenere presente quanto segue:

* È possibile eliminare una sola versione alla volta. Se una versione viene eliminata, questa azione viene visualizzata nella sezione Aggiornamenti del documento.
* Se si carica una nuova versione dopo aver eliminato una versione, la nuova versione riceve il numero sequenziale successivo. Ad esempio, se sono presenti 3 versioni di un documento e si elimina la versione 3, il documento successivo caricato sarà la versione 4.
* Gli aggiornamenti di sistema e i commenti aggiunti a una versione vengono mantenuti in Workfront dopo l’eliminazione della versione.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Per eliminare una versione del documento:

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare il documento dall&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Scorri verso il basso fino alla sezione **Versioni** per visualizzare tutte le versioni del documento.
1. Nella sezione **Versioni**, fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra della versione, quindi fai clic su **Elimina** nell&#39;elenco a discesa visualizzato.

   >[!NOTE]
   >
   >* L&#39;opzione **Elimina** è visibile solo se sono presenti almeno due versioni.
   >* Se il documento è collegato a un&#39;origine esterna, il collegamento viene eliminato e il documento non è più accessibile tramite Workfront.

   ![Elimina la versione del documento](assets/more-versions-350x143.png)

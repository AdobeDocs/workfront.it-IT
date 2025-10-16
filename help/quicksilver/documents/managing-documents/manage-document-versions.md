---
product-area: documents
navigation-topic: manage-documents
title: Gestire le versioni dei documenti
description: In Workfront è possibile gestire più versioni di un documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Gestire le versioni dei documenti

<!-- Audited: 5/2025 -->

In Workfront è possibile gestire più versioni di un documento.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizza accesso ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione al documento</p></td> 
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

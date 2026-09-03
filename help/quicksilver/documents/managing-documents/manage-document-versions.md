---
product-area: documents
navigation-topic: manage-documents
title: Gestire le versioni dei documenti
description: In Workfront è possibile gestire più versioni di un documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
TQID: https://experienceleague.adobe.com/rCnj3Gx1SB3-UziuppQfifv2hJ6q3OjepNO9FcEEHEk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c83b252faf7791c51475c5b82ca03cb4ee29bfc0
workflow-type: tm+mt
source-wordcount: 1077
ht-degree: 4%

---

# Gestire le versioni dei documenti

<!-- Audited: 5/2025 -->

{{highlighted-preview}}

In Workfront è possibile gestire più versioni di un documento.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando l’archiviazione cloud Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizza accesso ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione al documento</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* In questo articolo si presuppone che il documento abbia più versioni.

  Se hai bisogno di informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Gestione delle versioni dei documenti nell&#39;area documenti legacy

### Visualizzare un elenco di tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Scorri verso il basso fino alla sezione **Versioni** per visualizzare tutte le versioni del documento.

### Visualizzare e gestire i dettagli di una versione precedente del documento

{{step1-to-documents}}

1. Passa il puntatore del mouse sul documento, quindi fai clic su **Dettagli documento**.

1. Nella parte superiore della pagina **Dettagli documento**, fare clic sul menu a discesa accanto al nome, quindi sul nome della versione che si desidera visualizzare e gestire.

   ![Elenco a discesa della versione nella pagina Dettagli documento](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Oltre a visualizzare i dettagli della versione, è possibile modificarla, ad esempio il nome, i metadati e le impostazioni di correzione (se si tratta di una bozza di documento).

### Scarica una versione di un singolo documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Nella sezione **Versioni**, fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra della versione, quindi fai clic su **Scarica** nell&#39;elenco a discesa visualizzato.

   ![Scarica un singolo documento](assets/more-versions-350x143.png)

### Scaricare tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Nell&#39;angolo superiore destro della pagina fare clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/qs-summary-in-new-toolbar-small.png). Viene aperto il pannello laterale **Riepilogo documento**.

1. Scorri verso il basso fino alla sezione **Versioni**, quindi fai clic su **Scarica tutto**.

### Eliminare una versione del documento

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

<div class="preview">

## Gestire le versioni dei documenti nella nuova area Documenti in Anteprima

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Workfront numera ogni versione nell&#39;ordine in cui è stata caricata (ad esempio, V1, V2, V3) in modo che corrisponda ai numeri di versione in Frame.io.

### Visualizzare un elenco di tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina. Il pannello Versioni si apre e elenca ogni versione del documento in Cronologia versioni.

   >[!NOTE]
   >
   >Se una versione dispone di un flusso di lavoro di approvazione, accanto ad essa viene visualizzato lo stato, ad esempio &quot;Approvato&quot; o &quot;Ritirato&quot;. Le versioni senza un flusso di lavoro di approvazione non visualizzano uno stato.

### Richiedi approvazione per una versione

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.
1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina.
1. Fai clic sul menu **Altro** accanto alla versione, quindi fai clic su **Richiedi approvazione**.
1. Configura il flusso di lavoro di approvazione. Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

   >[!NOTE]
   >
   >Se una versione precedente dispone già di un flusso di lavoro di approvazione aperto, la richiesta di approvazione per questa versione lo ritira. La versione precedente mantiene il numero di versione e la cronologia di approvazione, ma il suo stato cambia in &quot;Ritirato&quot;.

### Visualizzare e gestire i dettagli di una versione precedente del documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.
1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina.
1. Fai clic sul menu **Altro** accanto alla versione, quindi fai clic su **Visualizza dettagli**.

### Scarica una versione di un singolo documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina.

1. Fai clic sul menu **Altro** accanto alla versione, quindi fai clic su **Scarica**.

### Scaricare tutte le versioni di un documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina.

1. Fai clic su **Scarica tutto** nella parte superiore del pannello Versioni.

   ![scarica tutte le versioni di un documento](assets/download-all-versions.png)

### Eliminare una versione del documento

{{step1-to-documents}}

1. Nella pagina **Documenti** selezionare un documento nell&#39;elenco.

1. Fai clic sull&#39;icona **Versioni** ![Versioni](assets/versions-icon.png) sul lato destro della pagina.

1. Fai clic sul menu **Altro** accanto alla versione, quindi fai clic su **Elimina**.

   >[!NOTE]
   >
   >L&#39;eliminazione di una versione non modifica i numeri delle altre versioni. Se, ad esempio, si elimina la V3 da un documento con versioni da V1 a V5, le versioni rimanenti mantengono i numeri originali e successivamente non vi è alcuna V3. La versione successiva caricata diventa V6.

</div>

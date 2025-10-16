---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: Report documento con collegamento a una bozza'
description: 'Visualizza: report di documenti con collegamento a una bozza'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# Visualizza: report di documenti con collegamento a una bozza

<!--Audited: 11/2024-->

In questa visualizzazione documento è possibile inserire un collegamento a una bozza della versione corrente del documento.

![Visualizza documento con collegamento bozza](assets/view-document-with-proof-link-350x92.png)

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
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare un report documento con collegamento a una bozza

Per applicare questa visualizzazione:

1. Consente di passare a un elenco di documenti.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.
1. Fai clic su **Aggiungi colonna**.
1. Fare clic su **Passa alla modalità testo**, quindi su **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Sostituisci &quot;Il tuo dominio&quot; con il tuo dominio Workfront effettivo. Ad esempio, se l&#39;URL Workfront della tua azienda è *Company.my.workfront.com*, il dominio è &quot;Azienda&quot;.

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.
1. (Facoltativo) Aggiorna il nome della visualizzazione, quindi fai clic su **Salva visualizzazione**.
1. (Facoltativo) Per garantire che vengano visualizzati solo i documenti con bozze, aggiungi un filtro effettuando le seguenti operazioni:

   1. Fai clic sul menu a discesa **Filtro**, quindi fai clic su **Nuovo filtro**.
   1. Fai clic su **Aggiungi regola filtro** e inizia a digitare &quot;Proprietario bozza&quot;, quindi seleziona **ID proprietario bozza** quando viene visualizzato nell&#39;elenco.
   1. Selezionare **Non è vuoto** per il modificatore di filtro.
   1. Fai clic su **Salva filtro**.
   1. (Facoltativo) Aggiornare il nome del filtro, quindi fare clic su **Salva filtro**.

1. Fai clic sul collegamento nella colonna Collegamento bozza per accedere alla bozza dell’ultima versione del documento.

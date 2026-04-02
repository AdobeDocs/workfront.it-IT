---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: Report documento con collegamento a una bozza'
description: 'Visualizzazione: documentare rapporti con collegamento a una bozza'
author: Courtney
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Visualizzazione: documentare rapporti con collegamento a una bozza

<!--Audited: 11/2024-->

In questa visualizzazione documento è possibile inserire un collegamento a una bozza della versione corrente del documento.

![Visualizza documento con collegamento bozza](assets/view-document-with-proof-link-350x92.png)

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
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

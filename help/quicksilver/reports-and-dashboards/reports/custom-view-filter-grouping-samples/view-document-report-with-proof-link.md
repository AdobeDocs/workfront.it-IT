---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: report di documenti con collegamento a una bozza"
description: "Visualizza: report di documenti con collegamento a una bozza"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Visualizza: report di documenti con collegamento a una bozza

In questa visualizzazione documento è possibile inserire un collegamento a una bozza della versione corrente del documento.

![](assets/view-document-with-proof-link-350x92.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizzare un report documento con collegamento a una bozza

Per applicare questa visualizzazione:

1. Consente di passare a un elenco di documenti.
1. Dalla sezione **Visualizza** menu a discesa, seleziona **Nuova visualizzazione**.

1. Clic **Aggiungi colonna**.
1. Clic **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Sostituisci &quot;Il tuo dominio&quot; con il tuo dominio Workfront effettivo. Ad esempio, se l’URL Workfront della tua azienda è *Company.my.workfront.com*, il tuo dominio è &quot;Azienda&quot;.

1. Clic **Salva**, quindi **Salva visualizzazione**.
1. Digita un nome per la visualizzazione, quindi fai clic su **Salva visualizzazione**.
1. (Facoltativo) Per garantire che vengano visualizzati solo i documenti con bozze, aggiungi un filtro effettuando le seguenti operazioni:

   1. Fai clic su **Filtro** menu a discesa, quindi fai clic su **Nuovo filtro**.
   1. Clic **Aggiungere una regola di filtro** e inizia a digitare Proof Owner (Proprietario bozza), quindi seleziona **ID proprietario bozza** quando viene visualizzato nell’elenco.
   1. Seleziona **Non è vuoto** per il modificatore di filtro.
   1. Clic **Salva filtro**, digita il nome del filtro, quindi fai clic su **Salva filtro**.

1. Fai clic sul collegamento nella colonna Collegamento bozza per accedere alla bozza dell’ultima versione del documento.

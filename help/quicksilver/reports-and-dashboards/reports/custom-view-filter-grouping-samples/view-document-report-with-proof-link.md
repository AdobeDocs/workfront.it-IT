---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: rapporto del documento con collegamento a una bozza"'
description: '''Visualizza: rapporto del documento con collegamento a una bozza"'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Visualizza: rapporto del documento con collegamento a una bozza

In questa visualizzazione documento è possibile inserire un collegamento a una prova della versione corrente del documento.

![](assets/view-document-with-proof-link-350x92.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizzare un rapporto del documento con un collegamento a una bozza

Per applicare questa visualizzazione:

1. Vai a un elenco di documenti.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. Fai clic su **Aggiungi colonna**.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

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

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
1. Digitare un nome per la visualizzazione, quindi fare clic su **Salva visualizzazione**.
1. (Facoltativo) Per visualizzare solo i documenti con bozze, aggiungi un filtro facendo quanto segue:

   1. Fai clic sul pulsante **Filtro** menu a discesa, quindi fai clic su **Nuovo filtro**.
   1. Fai clic su **Aggiungere una regola filtro** e inizia a digitare Proof Owner (Proprietario prova), quindi seleziona **ID proprietario bozza** quando viene visualizzato nell’elenco.
   1. Seleziona **Non vuoto** per il modificatore del filtro.
   1. Fai clic su **Salva filtro**, digita il nome del filtro, quindi fai clic su **Salva filtro**.

1. Fai clic sul collegamento nella colonna Collegamento di prova per accedere alla bozza dell’ultima versione del documento.

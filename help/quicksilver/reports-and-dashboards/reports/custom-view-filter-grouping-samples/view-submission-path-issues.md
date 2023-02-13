---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: percorso di invio dei problemi'
description: Puoi visualizzare il percorso in cui è stato inviato un problema nella visualizzazione di un rapporto sul problema. Il percorso indica la coda, il gruppo di argomenti e l'argomento della coda in cui il problema è stato originariamente inviato.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Visualizza: percorso di invio dei problemi

Puoi visualizzare il percorso in cui è stato inviato un problema nella visualizzazione di un rapporto sul problema. Il percorso indica la coda, il gruppo di argomenti e l&#39;argomento della coda in cui il problema è stato originariamente inviato.

![issue_submit_path.png](assets/issue-submission-path-350x66.png)

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

## Visualizza il percorso di invio per i problemi

1. Vai a un elenco di problemi.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** area, fai clic su **Aggiungi colonna**.

1. Fai clic sull’intestazione della nuova colonna, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <pre>displayname= Percorso del problema<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valuefield=displayQueueBreadcrumb <br>valueformat=HTML<br></pre>

1. Fai clic su **Salva visualizzazione**.

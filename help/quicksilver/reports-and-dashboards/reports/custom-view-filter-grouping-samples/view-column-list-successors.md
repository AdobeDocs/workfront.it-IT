---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: aggiungi un elenco di successori attività in una colonna"'
description: È possibile aggiungere una colonna a una visualizzazione attività per visualizzare un elenco dei successori delle attività. La colonna Successori attività include il numero del successore e il nome.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Visualizza: aggiungere un elenco di successori attività in una colonna

È possibile aggiungere una colonna a una visualizzazione attività per visualizzare un elenco dei successori delle attività. La **Successori attività** include il numero del successore e il nome.

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Aggiungere un elenco dei successori delle attività in una colonna

Per aggiungere questa colonna a una visualizzazione attività:

1. Passare a una visualizzazione attività esistente.
1. Espandi il menu a discesa Visualizza e seleziona **Personalizza visualizzazione**.
1. Fai clic su **Aggiungi colonna**.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sopra **Mostra in questa colonna** e fai clic su **Fare clic per modificare il testo**.

1. Rimuovere tutto il testo nella casella Modalità testo e sostituirlo con il seguente codice:

   <pre>displayname=Successori attività<br>listdelimiter=<br><br>listmethod=nidificato(successors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}).{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Fai clic su **Salva visualizzazione**.

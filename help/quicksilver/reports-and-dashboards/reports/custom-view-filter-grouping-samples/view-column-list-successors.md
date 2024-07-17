---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: aggiungi un elenco di successori attività in una colonna"
description: È possibile aggiungere una colonna a una visualizzazione delle attività per visualizzare un elenco dei successori delle attività. La colonna Successori attività include il numero del successore e il nome.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 2%

---

# Visualizza: aggiungere un elenco di successori attività in una colonna

È possibile aggiungere una colonna a una visualizzazione delle attività per visualizzare un elenco dei successori delle attività. La colonna **Successori attività** include il numero del successore e il nome.

![visualizzazione_attività_con_un_elenco_di_successori_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Aggiungere un elenco di successori attività in una colonna

Per aggiungere questa colonna a una visualizzazione delle attività:

1. Consente di passare a una visualizzazione attività esistente.
1. Espandere il menu a discesa Visualizza e selezionare **Personalizza visualizzazione**.
1. Fai clic su **Aggiungi colonna**.
1. Fare clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area **Mostra in questa colonna** e fai clic su **Fai clic per modificare il testo**.

1. Rimuovere tutto il testo nella casella Modalità testo e sostituirlo con il seguente codice:
   <pre>displayname=Successori attività<br>listdelimiter=<br><br>listmethod=nested(successors).LISTS<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Fai clic su **Salva vista**.

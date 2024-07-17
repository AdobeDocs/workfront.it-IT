---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: consente di visualizzare la relazione padre-figlio in un'attività tramite il rientro delle attività"
description: Per mantenere la distinzione tra relazioni padre e figlio in un elenco di attività esportato, aggiungere una visualizzazione personalizzata all'elenco di attività e assicurarsi che sia selezionata prima di esportare l'elenco.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 2%

---

# Visualizza: consente di visualizzare la relazione padre-figlio in un&#39;attività tramite il rientro delle attività

Per mantenere la distinzione tra relazioni padre e figlio in un elenco di attività esportato, aggiungere una visualizzazione personalizzata all&#39;elenco di attività e assicurarsi che sia selezionata prima di esportare l&#39;elenco.

![](assets/parent-child-indented-custom-view-350x94.png)

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

## Visualizzare la relazione padre-figlio in un&#39;attività applicando un rientro alle attività

1. Vai al progetto con l’elenco attività che desideri esportare.
1. Fai clic sul menu a discesa **Visualizza** e seleziona **Nuova visualizzazione**.

1. Denomina il filtro nell’angolo in alto a sinistra dello schermo.
1. Fai clic sull&#39;intestazione della colonna **Nome attività**.

1. Selezionare **Passa alla modalità testo** nell&#39;angolo superiore destro.
1. Fare clic in un punto qualsiasi della casella di testo per modificare il testo e rimuovere tutto il testo esistente.
1. Incolla il testo seguente:


```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
```

1. Fai clic su **Salva**.
1. Fai clic su **Salva vista**.

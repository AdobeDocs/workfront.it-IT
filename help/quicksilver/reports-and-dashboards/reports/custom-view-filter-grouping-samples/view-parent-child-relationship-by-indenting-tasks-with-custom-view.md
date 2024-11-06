---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: visualizzazione della relazione padre-figlio in un'attività tramite il rientro delle attività"
description: Per mantenere la distinzione tra relazioni padre e figlio in un elenco di attività esportato, aggiungere una visualizzazione personalizzata all'elenco di attività e assicurarsi che sia selezionata prima di esportare l'elenco.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Visualizza: consente di visualizzare la relazione padre-figlio in un&#39;attività tramite il rientro delle attività

<!--Audited: 11/2024-->

Per mantenere la distinzione tra relazioni padre e figlio in un elenco di attività esportato, aggiungere una visualizzazione personalizzata all&#39;elenco di attività e assicurarsi che sia selezionata prima di esportare l&#39;elenco.

![](assets/parent-child-indented-custom-view-350x94.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p> Corrente: 
   <ul>
   <li>Richiesta di modifica di una vista</li> 
   <li>Pianificare la modifica di un rapporto</li>
   </ul>
     </p>
     <p> Nuovo: 
   <ul>
   <li>Collaboratore per modificare una visualizzazione</li> 
   <li>Standard per modificare un rapporto</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare la relazione padre-figlio in un&#39;attività applicando un rientro alle attività

1. Vai al progetto con l’elenco attività che desideri esportare.
1. Fai clic sul menu a discesa **Visualizza** e seleziona **Nuova visualizzazione**.
1. Fai clic sull&#39;intestazione della colonna **Nome attività**.
1. Selezionare **Passa alla modalità testo** nell&#39;angolo superiore destro.
1. Fare clic su **Modifica modalità testo** e rimuovere tutto il testo esistente.
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

1. Fai clic su **Fine** > **Salva visualizzazione**.

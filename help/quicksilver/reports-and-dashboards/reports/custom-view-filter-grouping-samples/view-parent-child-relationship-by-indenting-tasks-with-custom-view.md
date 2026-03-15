---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: consente di visualizzare la relazione padre-figlio in un task rientrando i task.'
description: È possibile mantenere la distinzione tra relazioni padre-figlio in un elenco attività esportato aggiungendo una visualizzazione personalizzata all'elenco attività e verificando che tale visualizzazione sia selezionata prima dell'esportazione dell'elenco.
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 21%

---

# Visualizzazione: mostrare la relazione padre-figlio in un’attività tramite il rientro di attività

<!--Audited: 11/2024-->

È possibile mantenere la distinzione tra relazioni padre-figlio in un elenco attività esportato aggiungendo una visualizzazione personalizzata all&#39;elenco attività e verificando che tale visualizzazione sia selezionata prima dell&#39;esportazione dell&#39;elenco.

![Rientro figlio padre](assets/parent-child-indented-custom-view-350x94.png)

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Visualizzare la relazione padre-figlio in un&#39;attività rientrando le attività

1. Passare al progetto con l&#39;elenco delle attività che si desidera esportare.
1. Fai clic sul menu a discesa **Visualizza** e seleziona **Nuova vista**.
1. Fare clic nell&#39;intestazione di colonna **Nome attività**.
1. Seleziona **Passa alla modalità testo** nell&#39;angolo in alto a destra.
1. Fai clic su **Modifica modalità testo** e rimuovi tutto il testo esistente.
1. Incollate il testo seguente:


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. Fai clic su **Fine** > **Salva vista**.

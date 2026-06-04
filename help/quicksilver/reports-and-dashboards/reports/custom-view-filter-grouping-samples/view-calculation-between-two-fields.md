---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizzazione: mostrare il risultato di un calcolo tra due campi in una colonna'
description: È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ggwDFu-5dxDHNvX7JR9tWf730CFUrk0RF7Bu9QHgu9w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 324
ht-degree: 20%

---

# Visualizzazione: mostrare il risultato di un calcolo tra due campi in una colonna

<!--Audited: 11/2024-->

È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi.

Ad esempio, se desideri conoscere il numero di giorni della settimana trascorsi tra due date, puoi utilizzare la sintassi della modalità testo e le espressioni di dati per calcolare questa differenza.\
È possibile, ad esempio, calcolare la differenza tra i giorni della settimana tra la data di completamento pianificata e la data di completamento effettiva di un&#39;attività e visualizzare il risultato in una colonna.

In questo calcolo è possibile utilizzare altre due date (Inizio effettivo, Completamento effettivo, Inizio previsto, Completamento previsto e così via).\
Per ulteriori informazioni sulle espressioni di dati calcolati, vedere [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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


## Visualizzare il risultato di un calcolo tra due campi in una colonna

Per aggiungere questa colonna a una visualizzazione delle attività:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna**, quindi su **Passa alla modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Facoltativo) Per aggregare i valori visualizzati nella visualizzazione in un raggruppamento, seguire la procedura descritta in [Raggruppamento: visualizza il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.

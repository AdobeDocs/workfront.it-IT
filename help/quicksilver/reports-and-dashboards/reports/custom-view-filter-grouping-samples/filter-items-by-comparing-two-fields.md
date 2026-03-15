---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: eliminare gli elementi in un elenco confrontando due campi'
description: È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È possibile, ad esempio, visualizzare solo i task in cui la data di completamento effettivo del task è successiva alla data di completamento pianificata.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 25%

---

# Filtro: eliminare gli elementi in un elenco confrontando due campi

<!--Audited: 10/2024-->

È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È possibile, ad esempio, visualizzare solo i task in cui la data di completamento effettivo del task è successiva alla data di completamento pianificata.

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
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrare gli elementi confrontando due campi

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Filtro**, seleziona **Nuovo filtro**.

1. Aggiungi un filtro per la **data di completamento:Actual dell&#39;attività** > **Maggiore di** > **Seleziona una data**.

   >[!TIP]
   >
   >Scegliere il modificatore di filtro che si desidera utilizzare per il campo selezionato, se disponibile.

1. Fai clic su **Modalità testo**.
1. Nell’area visualizzata, aggiungi il seguente codice:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Fai clic su **Applica** > **Salva come nuovo**.

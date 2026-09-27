---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: eliminare gli elementi in un elenco confrontando due campi'
description: È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell'attività è successiva alla data di completamento pianificata.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Dk-vO1o3RveoOm0oI9U8CFrlcHvNZP-CylYCALZbH3o'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 25%
---
# Filtro: eliminare gli elementi in un elenco confrontando due campi

<!--Audited: 10/2024-->

È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell&#39;attività è successiva alla data di completamento pianificata.

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

## Filtrare gli elementi confrontando due campi

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Aggiungi un filtro per **Attività:Actual Data di completamento** > **Maggiore di** > **Seleziona una data**.

   >[!TIP]
   >
   >Scegliere il modificatore di filtro da utilizzare per il campo selezionato, se disponibile.

1. Fare clic su **Modalità testo**.
1. Nell’area visualizzata, aggiungi il seguente codice:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Fai clic su **Applica** > **Salva come nuovo**.

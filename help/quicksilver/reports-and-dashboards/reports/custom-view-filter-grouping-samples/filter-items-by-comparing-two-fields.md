---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: elimina elementi in un elenco confrontando due campi'
description: È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell'attività è successiva alla data di completamento pianificata.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filtro: elimina elementi in un elenco confrontando due campi

<!--Audited: 10/2024-->

È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell&#39;attività è successiva alla data di completamento pianificata.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

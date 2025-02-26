---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: elimina elementi in un elenco confrontando due campi'
description: È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell'attività è successiva alla data di completamento pianificata.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Filtro: elimina elementi in un elenco confrontando due campi

<!--Audited: 10/2024-->

È possibile filtrare gli elementi di un elenco confrontando due dei relativi campi. È ad esempio possibile visualizzare solo le attività in cui la data di completamento effettiva dell&#39;attività è successiva alla data di completamento pianificata.

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
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

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrare gli elementi confrontando due campi

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Aggiungi un filtro per **Attività:Data di completamento effettiva** > **Maggiore di** > **Seleziona una data**.

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

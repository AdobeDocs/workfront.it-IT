---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: organizza i risultati elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento'
description: È possibile visualizzare le attività raggruppate per percentuale di completamento in intervalli di 0-25, 26-50, 51-75, 75-99 e 100. A tale scopo, puoi creare un raggruppamento utilizzando la modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Raggruppamento: organizza i risultati elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento

<!--Audited: 10/2024-->

È possibile visualizzare le attività raggruppate per percentuale di completamento in intervalli di 0-25, 26-50, 51-75, 75-99 e 100. A tale scopo, puoi creare un raggruppamento utilizzando la modalità testo.

![Raggruppamento per valore calcolato](assets/grouping-calculated-value-column-to-all-objects.png)

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

## Organizza i risultati elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento

Per applicare questo raggruppamento a un elenco di attività:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Raggruppamento** selezionare **Nuovo raggruppamento**.

1. Fare clic su **Passa alla modalità testo**.
1. Nello spazio disponibile, aggiungi il seguente codice:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.

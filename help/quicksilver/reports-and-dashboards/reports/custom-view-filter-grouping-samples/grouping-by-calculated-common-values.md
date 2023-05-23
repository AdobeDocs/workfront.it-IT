---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: organizza i risultati dell’elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento"
description: È possibile visualizzare le attività raggruppate per percentuale di completamento in intervalli di 0-25, 26-50, 51-75, 75-99 e 100. A tale scopo, puoi creare un raggruppamento utilizzando la modalità testo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Raggruppamento: organizza i risultati elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento

È possibile visualizzare le attività raggruppate per percentuale di completamento in intervalli di 0-25, 26-50, 51-75, 75-99 e 100. A tale scopo, puoi creare un raggruppamento utilizzando la modalità testo.

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
   <td> <p>Richiesta di modifica di un raggruppamento </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modifica l'accesso a Filtri, Viste, Raggruppamenti per modificare un raggruppamento</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Organizza i risultati elenco in base a un valore calcolato comune a tutti gli oggetti del raggruppamento

Per applicare questo raggruppamento a un elenco di attività:

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Clic **Passa alla modalità testo**.
1. Nello spazio disponibile, aggiungi il seguente codice:

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. Clic **Fine**, quindi **Salva raggruppamento**.

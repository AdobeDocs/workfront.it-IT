---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: dettagli predecessore"
description: Questa visualizzazione delle attività mostra i dettagli dei predecessori delle attività utilizzando una visualizzazione di raccolta. In una visualizzazione di insieme è possibile visualizzare informazioni sugli oggetti che si trovano in una relazione uno-a-molti. In questo caso, ogni attività (una) può avere più predecessori (molti). Nella visualizzazione vengono visualizzati il nome delle attività, i nomi dei predecessori, i nomi dei progetti dei predecessori, le date di completamento pianificate dei predecessori e gli stati dei predecessori.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Visualizza: dettagli predecessore

Questa visualizzazione delle attività mostra i dettagli dei predecessori delle attività utilizzando una visualizzazione di raccolta. In una visualizzazione di insieme è possibile visualizzare informazioni sugli oggetti che si trovano in una relazione uno-a-molti. In questo caso, ogni attività (una) può avere più predecessori (molti). Nella visualizzazione vengono visualizzati il nome delle attività, i nomi dei predecessori, i nomi dei progetti dei predecessori, le date di completamento pianificate dei predecessori e gli stati dei predecessori.

Per informazioni sul riferimento alle raccolte nei rapporti, consulta [Fare riferimento alle raccolte in un rapporto](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizza dettagli predecessore

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, seleziona **Nuova visualizzazione**.

1. In **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessori Numeri e nomi<br>column.1.listdelimiter= colonna.1<br><br>column.1.listmethod=nested(predecessors).LISTS<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecessor}).{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Nomi progetto predecessori<br>column.2.listdelimiter= colonna.2.listdelimiter<br><br>column.2.listmethod=nested(predecessors).LISTS<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}.{progetto}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Date di completamento dei predecessori<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors).LISTS<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}.{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Stato dei predecessori<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecessors).LISTS<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. Clic **Salva visualizzazione**.

---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: dettagli predecessori"'
description: Questa visualizzazione attività mostra i dettagli dei predecessori delle attività utilizzando una vista raccolta. In una vista raccolta, è possibile visualizzare informazioni sugli oggetti che si trovano in una relazione "uno-a-molti". In questo caso, ogni attività (una) può avere più predecessori (molti). Nella visualizzazione viene visualizzato il nome delle attività, nonché i nomi dei predecessori, i nomi dei progetti dei predecessori, le date di completamento pianificate dei predecessori e gli stati dei predecessori.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Visualizza: dettagli predecessore

Questa visualizzazione attività mostra i dettagli dei predecessori delle attività utilizzando una vista raccolta. In una vista raccolta, è possibile visualizzare informazioni sugli oggetti che si trovano in una relazione &quot;uno-a-molti&quot;. In questo caso, ogni attività (una) può avere più predecessori (molti). Nella visualizzazione viene visualizzato il nome delle attività, nonché i nomi dei predecessori, i nomi dei progetti dei predecessori, le date di completamento pianificate dei predecessori e gli stati dei predecessori.

Per informazioni sui riferimenti alle raccolte nei rapporti, vedi [Riferimento alle raccolte in un rapporto](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessore_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza dettagli predecessore

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessori Numeri e nomi<br>column.1.listdelimiter=<br><br>column.1.listmethod=nidificato(predecessori).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.value.expression=CONCAT({predecessor}).{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Nomi dei progetti predecessori<br>column.2.listdelimiter=<br><br>column.2.listmethod=nidificato(predecessori).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.value eexpression={predecessor}.{progetto}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Date di completamento predecessori<br>column.3.listdelimiter=<br><br>column.3.listmethod=nidificato(predecessori).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.value eexpression={predecessor}.{scheduledCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Stato predecessori<br>column.4.listdelimiter=<br><br>column.4.listmethod=nidificato(predecessori).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.value eexpression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. Fai clic su **Salva visualizzazione**.

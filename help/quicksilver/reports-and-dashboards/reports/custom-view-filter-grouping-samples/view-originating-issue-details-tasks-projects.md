---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: dettagli problema origine per attività e progetti"
description: Quando un problema viene convertito in un’attività o in un progetto, viene stabilita una relazione tra l’attività o il progetto e il problema. Questa visualizzazione mostra i campi del problema che viene completato automaticamente al completamento dell’attività o del progetto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 4%

---

# Visualizza: dettagli problema di origine per attività e progetti

Quando un problema viene convertito in un’attività o in un progetto, viene stabilita una relazione tra l’attività o il progetto e il problema. Questa vista mostra i seguenti campi del problema che vengono completati automaticamente al completamento dell’attività o del progetto:

* Nome
* Data inserimento
* Data di completamento Pianificata
* Data di completamento effettiva
* Tipo di richiesta
* Nome del creatore
* Assegnato a utente

![attività_con_risoluzione_problemi_campi.png](assets/task-with-resolving-issue-fields-350x38.png)

Per ulteriori informazioni, vedere anche [Visualizza: visualizza le informazioni originali sul problema negli elenchi di attività e progetti](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizza dettagli problema di origine per attività e progetti

1. Consente di passare a un elenco di attività o a un elenco di progetti.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area della modalità testo e fai clic su **Fai clic per modificare il testo**.
1. Rimuovere il testo trovato nella casella **Modalità testo** e sostituirlo con il seguente codice:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>column.0.textmode=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.descriptionkey=name<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.width=150<br>column.1.displayname=Resolvables (Issues)<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(resolvables).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={name}<br>column.1.valueformat=HTML<br>column.2.displayname=Resolvables Entry Date<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(resolvables).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={entryDate}<br>column.2.valueformat=HTML<br>column.3.displayname=Resolvables Due Date<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(resolvables).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Resolvables Actual Completion Date<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(resolvables).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={actualCompletionDate}<br>column.4.valueformat=HTML<br>column.5.displayname=Resolvables Request Type<br>column.5.listdelimiter=<br><br>column.5.listmethod=nested(resolvables).lists<br>column.5.textmode=true<br>column.5.type=iterate<br>column.5.valueexpression={opTaskType}<br>column.5.valueformat=HTML<br>column.6.displayname=Resolvables Originator<br>column.6.listdelimiter=<br><br>column.6.listmethod=nested(resolvables).lists<br>column.6.textmode=true<br>column.6.type=iterate<br>column.6.valueexpression={owner}.{name}<br>column.6.valueformat=HTML<br>column.7.descriptionkey=assignedto<br>column.7.linkedname=assignedTo<br>column.7.listsort=nested(assignedTo).string(name)<br>column.7.namekey=assignedto<br>column.7.querysort=assignedTo:name<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.textmode=true<br>column.7.valuefield=assignedTo:name<br>column.7.valueformat=HTML<br>column.7.width=150</code></pre>

1. Fai clic su **Salva vista**.

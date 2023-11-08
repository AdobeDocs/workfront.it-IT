---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: varianza prevista per la durata e il lavoro pianificato nella visualizzazione di un’attività"
description: Vedere un esempio di una visualizzazione che visualizza le informazioni sulla durata e sulla previsione Lavoro pianificato.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Vista: variazione prevista per la durata e il lavoro pianificato in una vista attività

In questa visualizzazione viene visualizzato quanto segue in una visualizzazione delle attività:

* Informazioni sull&#39;attività con informazioni sull&#39;attività prevista.
* Differenza tra Durata e Durata prevista predefinita.
* Differenza tra Lavoro pianificato e Lavoro pianificato previsto predefinito.

>[!NOTE]
>
> I dati visualizzati nella visualizzazione seguente confrontano i valori effettivi delle attività con i valori associati alle attività Previsione predefinita.

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## Visualizzare lo scostamento previsto per la durata e il lavoro pianificato in una visualizzazione delle attività

1. Consente di passare a un elenco di attività.
1. In **Visualizza** menu a discesa, seleziona **Nuova visualizzazione**.

1. Rimuove tutte le colonne nella vista, tranne la prima.
1. Con la prima colonna selezionata, fai clic su **Passa alla modalità testo**.
1. Copiare il testo sottostante e incollarlo nella prima colonna della visualizzazione:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=Nome attività<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=composto<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayname=Durata attività<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=durata<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask:durationFieldLong<br>column.2.valueformat=composto<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Attività linea di base Dflt: Dur<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Varianza durata"column.3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=Varianza durata<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueexpression=CONCAT(SUB({duration},{defaultBaselineTask}.{duration})/480," giorni")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Varianza durata<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=composto<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Richiesta di lavoro<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=defaultBaselineTask:workFieldLong<br>column.5.valueformat=composto<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Attività Baseline Dflt: Richiesta Lavoro<br>column.6.descriptionkey=workrequired<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Varianza sforzo<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=CONCAT(SUB({workRequired},{defaultBaselineTask}.{workRequired})/60," ore")<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Varianza sforzo</pre>

1. Clic **Salva visualizzazione**.
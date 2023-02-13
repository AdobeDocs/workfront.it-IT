---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Raggruppamento: suddivisione 2 per percentuale dell''attività'
description: "In questo raggruppamento di attività personalizzato è possibile visualizzare le attività raggruppate in base a un intervallo dei valori di completamento della percentuale. Le suddivisioni mostrano la percentuale di completamento di incrementi di 10 punti percentuali: 1-10%, 11-20%, ecc."
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Raggruppamento: suddivisione per percentuale dell&#39;attività 2

In questo raggruppamento di attività personalizzato è possibile visualizzare le attività raggruppate in base a un intervallo dei valori di completamento relativi alla percentuale. Le suddivisioni mostrano la percentuale di completamento di incrementi di 10 punti percentuali: 1-10%, 11-20%, ecc.

Il gruppo seguente organizza i progetti in base al valore di completamento percentuale in uno di questi raggruppamenti:

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10_suddivisione_raggruppamento.png](assets/task-10--breakdown-grouping-350x547.png)

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

## Raggruppa per suddivisione per percentuale attività

Per applicare questo raggruppamento:

1. Passare a un elenco di attività.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Passa alla modalità testo**.
1. Rimuovi il testo nel **Raggruppa il rapporto** area.
1. Sostituisci il testo con il seguente codice:

   <pre>group.0.linkedname=direct<br>group.0.name=Scomposizione percentuale<br>group.0.notime=false<br>group.0.value eexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=11,"1-10 %", IF({percentComplete}&lt;=21,"11-20 %", IF({percentComplete}&lt;=31,"21-30 %", IF({percentComplete})&lt;41,"31-40 %", IF({percentComplete}&lt;51,"41-50 %", IF({percentComplete}&lt;61,"51-60 %", IF({percentComplete}&lt;71,"61-70 %", IF({percentComplete}&lt;81,"77 1-80 %", IF({percentComplete}&lt;91,"81-90 %", IF({percentComplete}&lt;100,"91-99 %","100 %")))))))))))<br>textmode=true</pre>

1. Fai clic su **Salva raggruppamento**.

---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Raggruppamento: ripartizione 2 per percentuale del progetto'
description: "In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori di completamento in percentuale. Le suddivisioni mostrano la percentuale di completamento di incrementi di 10 punti percentuali: 0-10%, 11-20%, 21-30% ecc."
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 4%

---

# Raggruppamento: disaggregazione per percentuale progetto 2

In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori di completamento in percentuale. Le suddivisioni mostrano la percentuale di completamento di incrementi di 10 punti percentuali: 0-10%, 11-20%, 21-30% ecc.

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

![percent_complete_suddivisione_for_projects_in_10__increments.png](assets/percent-complete-breakdown-350x94.png)

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

## Raggruppa per percentuale di raggruppamento del progetto

Per applicare questo raggruppamento:

1. Vai a un elenco di progetti.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Passa alla modalità testo**.
1. Rimuovi il testo nella casella e incolla il seguente codice nello spazio disponibile:
   <pre>group.0.linkedname=direct<br>group.0.name=Scomposizione percentuale<br>group.0.notime=false<br>group.0.value eexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=11,"1-10 %", IF({percentComplete}&lt;=21,"11-20 %", IF({percentComplete}&lt;=31,"21-30 %", IF({percentComplete})&lt;41,"31-40 %", IF({percentComplete}&lt;51,"41-50 %", IF({percentComplete}&lt;61,"51-60 %", IF({percentComplete}&lt;71,"61-70 %", IF({percentComplete}&lt;81,"77 1-80 %", IF({percentComplete}&lt;91,"81-90 %", IF({percentComplete}&lt;100,"91-99 %","100 %")))))))))))<br>textmode=true</pre>

1. Fai clic su **Salva raggruppamento**.

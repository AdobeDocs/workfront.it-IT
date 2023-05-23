---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: raggruppamento percentuale attività 1"
description: '"In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori percentuali di completamento. Le suddivisioni mostrano il valore percentuale di completamento degli incrementi di 25 punti percentuali: 0-25%, 25-50%, ecc.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 2%

---

# Raggruppamento: raggruppamento percentuale attività 1

In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori percentuali di completamento. I raggruppamenti mostrano il valore percentuale di completamento degli incrementi di 25 punti percentuali: 0-25%, 25-50%, ecc. 

Il raggruppamento seguente organizza le attività in base al valore percentuale di completamento in 6 raggruppamenti diversi:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25__breakdown_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Raggruppa per ripartizione percentuale attività

Per applicare questo raggruppamento:

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Clic **Passa alla modalità testo**.
1. Rimuovi il testo nella **Raggruppa il report** area.
1. Sostituisci il testo con il seguente codice:

   <pre>group.0.linkedname=direct<br>group.0.name=Suddivisione percentuale<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}&lt;100,"75-99 %","100 %")))<br>group.0.valueformat=string</pre>

1. Clic **Salva raggruppamento**.

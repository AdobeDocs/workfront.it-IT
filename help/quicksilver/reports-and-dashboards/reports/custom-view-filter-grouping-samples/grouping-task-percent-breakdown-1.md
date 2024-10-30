---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: Raggruppamento percentuale attività 1"
description: '"In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori percentuali di completamento. Le suddivisioni mostrano il valore percentuale di completamento degli incrementi di 25 punti percentuali: 0-25%, 25-50%, ecc.'
author: Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Raggruppamento: raggruppamento percentuale attività 1

<!--Audited: 10/2024-->

In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per un intervallo dei loro valori percentuali di completamento. I raggruppamenti mostrano il valore percentuale di completamento degli incrementi di 25 punti percentuali: 0-25%, 25-50%, ecc.

Il raggruppamento seguente organizza le attività in base al valore percentuale di completamento in 6 raggruppamenti diversi:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![attività_25__breakdown_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Raggruppa per ripartizione percentuale attività

Per applicare questo raggruppamento:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Raggruppamento**, selezionare **Nuovo raggruppamento**.
1. Fare clic su **Aggiungi raggruppamento**.

1. Fare clic su **Passa alla modalità testo**.
1. Rimuovi il testo nell&#39;area **Raggruppa per**.
1. Sostituisci il testo con il seguente codice:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Fai clic su **Fine** > **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.

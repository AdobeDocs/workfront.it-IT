---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: Raggruppamento percentuale attività 2"
description: '"In questo raggruppamento di attività personalizzato, puoi visualizzare le attività raggruppate per un intervallo dei rispettivi valori di percentuale di completamento. Le suddivisioni mostrano il valore percentuale di completamento degli incrementi di 10 punti percentuali: 1-10%, 11-20%, ecc.'''
author: Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Raggruppamento: raggruppamento percentuale attività 2

<!--Audited: 10/2024-->

In questo raggruppamento di attività personalizzato è possibile visualizzare le attività raggruppate per un intervallo dei valori di percentuale di completamento. I raggruppamenti mostrano il valore percentuale di completamento degli incrementi di 10 punti percentuali: 1-10%, 11-20%, ecc.

Il raggruppamento seguente organizza i progetti in base al valore percentuale di completamento in uno di questi raggruppamenti:

* 0%
* 1-10%
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

![attività_10__breakdown_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. Fai clic su **Fine** > **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.

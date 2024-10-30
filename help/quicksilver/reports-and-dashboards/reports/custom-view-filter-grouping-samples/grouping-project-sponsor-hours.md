---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: sponsor del progetto per le ore"
description: Questo raggruppamento di ore organizza le ore per sponsor del progetto in cui le ore sono registrate. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Sponsor progetto. Per accedere a questo campo è necessario utilizzare l'interfaccia Modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: bc99e303047b989b972974b398420a9180e40874
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Raggruppamento: sponsor del progetto per ore

<!--Audited: 10/2024-->

Questo raggruppamento di ore organizza le ore per sponsor del progetto in cui le ore sono registrate. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Sponsor progetto. Per accedere a questo campo è necessario utilizzare l&#39;interfaccia Modalità testo.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Raggruppa per sponsor progetto per ore

Per applicare questo raggruppamento:

1. Consente di passare a un elenco di ore.
1. Dal menu a discesa **Raggruppamento**, selezionare **Nuovo raggruppamento**.

1. Fare clic su **Passa alla modalità testo**.
1. Rimuovere il testo nell&#39;area visualizzata e sostituirlo con il seguente codice:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Fai clic su **Fine**.
1. Aggiorna il nome del raggruppamento, quindi fai clic su **Salva raggruppamento**.

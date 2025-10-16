---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: sponsor progetto per le ore'
description: Questo raggruppamento di ore organizza le ore per sponsor del progetto in cui le ore sono registrate. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Sponsor progetto. Per accedere a questo campo è necessario utilizzare l'interfaccia Modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Raggruppamento: sponsor del progetto per ore

<!--Audited: 10/2024-->

Questo raggruppamento di ore organizza le ore per sponsor del progetto in cui le ore sono registrate. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Sponsor progetto. Per accedere a questo campo è necessario utilizzare l&#39;interfaccia Modalità testo.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

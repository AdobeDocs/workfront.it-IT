---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Attività personali'
description: Questo filtro attività restituisce le richieste di lavoro ad hoc inviate a un utente o gli elementi da fare aggiunti dagli utenti nella propria area Home. Le attività personali non sono collegate a un progetto, ma possono essere spostate in un progetto, se necessario.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Filtro: attività personali

<!--Audited: 10/2024-->

Questo filtro attività restituisce le richieste di lavoro ad hoc inviate a un utente o gli elementi da fare aggiunti dagli utenti nel widget Da fare nell’area Home.

Le richieste di lavoro ad hoc e gli elementi da fare vengono salvati in Adobe Workfront come attività personali.

Le attività personali non sono collegate a un progetto, ma possono essere spostate in un progetto, se necessario. Per informazioni, vedere [Creare attività personali](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Rapporto attività personali](assets/personal-tasks-report.png)

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

## Filtra attività personali

Per creare questo filtro:

1. Consente di passare a un elenco di attività o a un report di attività.
1. Dal menu a discesa **Filtro**, fare clic su **Nuovo filtro**.
1. (Condizionale) Fai clic su **Aggiungi una regola di filtro** per accedere al filtro da un report oppure inizia a selezionare i criteri di filtro nel primo campo, se accedi al filtro da un elenco.
1. (Condizionale) Seleziona i seguenti criteri di filtro:

   * Da un filtro elenco: **Attività** > **Personali** **È true**
   * Da un filtro report: **Attività** > **Personali** > **Uguali (distinzione maiuscole/minuscole)** > **Vero**.
1. Salva il filtro.

   Nell&#39;elenco vengono visualizzate solo le attività personali che non si trovano in alcun progetto.

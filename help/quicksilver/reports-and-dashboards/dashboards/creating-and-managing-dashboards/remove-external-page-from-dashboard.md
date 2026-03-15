---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Rimuovere una pagina esterna da una dashboard
description: È possibile rimuovere una pagina esterna da un dashboard se non è più necessaria.
author: Courtney
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 22%

---

# Rimuovere una pagina esterna da una dashboard

<!-- Audited: 1/2025 -->

È possibile rimuovere una pagina esterna da un dashboard se non è più necessaria.

Tuttavia, non è possibile eliminare una pagina esterna dopo che è stata creata in Adobe Workfront. Puoi eliminare una pagina esterna solo utilizzando l’API. Per informazioni sull&#39;API Workfront, consulta [Nozioni di base sull&#39;API](../../../wf-api/general/api-basics.md). Per informazioni sulla creazione di pagine esterne, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard e calendari</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per il dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rimuovere una pagina esterna da un dashboard

1. Vai al dashboard che contiene la pagina esterna che desideri eliminare.

1. Fai clic su **Azioni dashboard**, quindi fai clic su **Modifica**.

   ![Modifica dashboard](assets/unshimmed-edit-dashboard.png)

1. Sul lato destro dello schermo, individua la pagina esterna che desideri rimuovere e fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png).

   ![Icona Elimina pagina esterna nel dashboard](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Fai clic su **Salva + Chiudi** nell&#39;angolo in basso a sinistra.

   La pagina esterna verrà rimossa dal dashboard selezionato. La pagina esterna rimane in Workfront ed è possibile accedervi da un report. Per informazioni, vedere la sezione &quot;Visualizzare pagine esterne in un report&quot; nell&#39;articolo [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

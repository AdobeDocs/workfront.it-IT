---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Rimuovere una pagina esterna da un dashboard
description: Se non è più necessario, è possibile rimuovere una pagina esterna da un dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Rimuovere una pagina esterna da un dashboard

<!-- Audited: 1/2025 -->

Se non è più necessario, è possibile rimuovere una pagina esterna da un dashboard.

Tuttavia, non puoi eliminare una pagina esterna dopo che è stata creata in Adobe Workfront. Puoi eliminare una pagina esterna solo utilizzando l’API. Per informazioni sull&#39;API Workfront, vedere [Nozioni di base sull&#39;API](../../../wf-api/general/api-basics.md). Per informazioni sulla creazione di pagine esterne, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

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
      <p>Standard</p>
      <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a rapporti, dashboard e calendari</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rimuovere una pagina esterna da un dashboard

1. Passare alla dashboard contenente la pagina esterna da eliminare.

1. Fai clic su **Azioni dashboard**, quindi su **Modifica**.

   ![Modifica dashboard](assets/unshimmed-edit-dashboard.png)

1. Nella parte destra dello schermo individuare la pagina esterna da rimuovere e fare clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png).

   ![Icona Elimina pagina esterna nel dashboard](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Fai clic su **Salva + Chiudi** nell&#39;angolo in basso a sinistra.

   In questo modo la pagina esterna viene rimossa dal dashboard selezionato. La pagina esterna rimane in Workfront ed è accessibile da un report. Per informazioni, vedere la sezione &quot;Visualizzare pagine esterne in un report&quot; nell&#39;articolo [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

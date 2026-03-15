---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Visualizza report pianificati per la consegna'
description: Questo filtro di report visualizza tutti i report che devono essere consegnati automaticamente in Adobe Workfront. È consigliabile utilizzarla con la visualizzazione standard.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 27%

---

# Filtro: visualizzare i rapporti pianificati per la consegna

<!--Audited: 10/2024-->

Questo filtro di report visualizza tutti i report che devono essere consegnati automaticamente in Adobe Workfront. È consigliabile utilizzarla con la visualizzazione standard.

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
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtro recapito report

Per applicare questo filtro:

1. Consente di passare a un elenco di report.

1. Dal menu a discesa **Filtro**, seleziona **Nuovo filtro**.

1. Fai clic su **Passa alla modalità testo**.

1. Nell&#39;area **Imposta regole filtro per il report**, copiare e incollare il codice seguente:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Fai clic su **Salva filtro**.

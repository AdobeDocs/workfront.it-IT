---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: visualizzare i rapporti pianificati per la consegna'
description: Questo filtro per la generazione di rapporti mostra tutti i rapporti pianificati per essere consegnati automaticamente in Adobe Workfront. È meglio utilizzarlo con la visualizzazione standard.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 1%

---

# Filtro: visualizza i rapporti pianificati per la consegna

<!--Audited: 10/2024-->

Questo filtro per la generazione di rapporti mostra tutti i rapporti pianificati per essere consegnati automaticamente in Adobe Workfront. È meglio utilizzarlo con la visualizzazione standard.

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

## Filtro di consegna del rapporto

Per applicare questo filtro:

1. Passare a un elenco di report.

1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Fare clic su **Passa alla modalità testo**.

1. Nell&#39;area **Imposta regole filtro per il report**, copiare e incollare il codice seguente:

   ```
   scheduledReportID=0
   scheduledReportID_Mod=notnull
   ```

1. Fai clic su **Salva filtro**.

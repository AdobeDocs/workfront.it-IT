---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: Percorso di invio per i problemi'
description: È possibile visualizzare il percorso attraverso il quale un problema è stato inviato nella visualizzazione di un report del problema. Il percorso indica la coda, il gruppo di argomenti e l’argomento della coda in cui è stato inviato il problema originariamente.
author: Courtney
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 19%

---

# Visualizzazione: percorso di invio per i problemi

<!--Audited: 11/2024-->

È possibile visualizzare il percorso attraverso il quale un problema è stato inviato nella visualizzazione di un report del problema. Il percorso indica la coda, il gruppo di argomenti e l’argomento della coda in cui è stato inviato il problema originariamente.

![issue_submit_path.png](assets/issue-submission-path-350x66.png)

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Visualizza il percorso di invio per i problemi

1. Vai a un elenco di problemi.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** fare clic su **Aggiungi colonna**.
1. Fai clic sull&#39;intestazione della nuova colonna, quindi fai clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname= Issue Path
   linkedname=direct
   namekey=displayQueueBreadcrumb
   valuefield=displayQueueBreadcrumb
   valueformat=HTML
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.

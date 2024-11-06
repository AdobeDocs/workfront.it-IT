---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: oggetti risolvibili in un rapporto di attività o di progetto"
description: È possibile visualizzare un elenco di tutti gli oggetti risolvibili in una visualizzazione o in un report di progetti o attività.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Visualizzazione: oggetti risolvibili in un report di attività o di progetto

<!--Audited: 11/2024-->

È possibile visualizzare un elenco di tutti gli oggetti risolvibili in una visualizzazione o in un report di progetti o attività.

Per ulteriori informazioni sugli oggetti risolvibili, vedere l&#39;articolo [Panoramica sugli oggetti risolvibili e risolvibili](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

Questa visualizzazione è identica per attività e progetti.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p> Corrente: 
   <ul>
   <li>Richiesta di modifica di una vista</li> 
   <li>Pianificare la modifica di un rapporto</li>
   </ul>
     </p>
     <p> Nuovo: 
   <ul>
   <li>Collaboratore per modificare una visualizzazione</li> 
   <li>Standard per modificare un rapporto</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzazione di oggetti risolvibili in un report di attività o di progetto

1. Consente di passare a un elenco di attività o progetti convertiti dai problemi.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** fare clic su **Aggiungi colonna**.

1. Fai clic sull&#39;intestazione della nuova colonna, quindi fai clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.\
   Nella nuova colonna viene visualizzato un elenco di tutti gli oggetti risolvibili. I nomi degli oggetti nell&#39;elenco non possono essere collegati direttamente agli oggetti.

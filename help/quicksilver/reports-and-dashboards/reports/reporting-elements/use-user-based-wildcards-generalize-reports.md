---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati sull’utente per generalizzare i rapporti
description: È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/S5vsXfapgDf4fjhAPV6iet9kobyEUCM14QMF-ZvvaDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 457
ht-degree: 15%

---

# Utilizzare caratteri jolly basati sull’utente per generalizzare i rapporti

<!-- Audited: 11/2024 -->

È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting. Ad esempio, se si desidera creare un report che mostri le attività assegnate a un utente specifico, è possibile utilizzare il nome dell&#39;utente nel campo Assegnato a del filtro. Tuttavia, se si desidera creare un report che mostra le attività assegnate all&#39;utente connesso, indipendentemente dall&#39;utente, è possibile utilizzare un carattere jolly che indichi che quando un utente visualizza il report, vengono visualizzate solo le informazioni che lo riguardano. In questo modo, il rapporto verrà generato una sola volta, ma poiché si utilizza un carattere jolly nel filtro, si otterranno risultati diversi ogni volta che verrà letto da un altro utente.

Puoi utilizzare caratteri jolly basati sugli utenti per creare i seguenti elementi di reporting:

* Filtri
* Richieste personalizzate
* Visualizzazioni durante l’aggiunta di regole per le colonne

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
   <td role="rowheader">Licenza di Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Piano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard e Calendari per modificare gli elementi di reporting in un rapporto</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
    <td> <p>Gestire le autorizzazioni per un report per modificare gli elementi di reporting in un report</p> <p>Gestire le autorizzazioni per una visualizzazione o un filtro per modificarle</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare un report prima di aggiungere una variabile con caratteri jolly.

Per istruzioni sulla creazione di report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Passaggi pratici

Per inserire un carattere jolly basato sull&#39;utente in un report:

1. Passare a un report per il quale si desidera inserire un carattere jolly basato sull&#39;utente.
1. Fai clic su **Azioni report**, quindi su **Modifica**.

1. Fare clic sulla scheda **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. Inizia a digitare il nome del campo in base al quale desideri filtrare.\
   È necessario digitare i campi che fanno riferimento all&#39;oggetto utente o alle informazioni sugli utenti.
1. Seleziona **Uguale** nel menu a discesa per la variabile filtro.

   >[!TIP]
   >
   >È sempre necessario selezionare la variabile di filtro **Equal** quando si utilizzano i caratteri jolly in Adobe Workfront.

1. Nella casella **Inizia a digitare il nome ...** digitare: `$$USER.ID` o `$$USER.name` se si desidera che nel report vengano visualizzate le informazioni relative all&#39;utente che effettua l&#39;accesso, in base al nome. È possibile inserire altri caratteri jolly che fanno riferimento al gruppo, al team, alla società o ad altre informazioni dell&#39;utente connesso.

   Per un elenco completo dei caratteri jolly basati sull&#39;utente, vedere [Panoramica sulle variabili dei filtri con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Fai clic su **Salva e Chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle viste](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

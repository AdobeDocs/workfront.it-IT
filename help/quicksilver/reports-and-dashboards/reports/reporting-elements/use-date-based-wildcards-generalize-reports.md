---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati sulla data per generalizzare i rapporti
description: È possibile generalizzare un report utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.
author: Courtney
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 10%

---

# Utilizzare caratteri jolly basati sulla data per generalizzare i rapporti

<!-- Audited: 11/2024 -->

È possibile generalizzare un report utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.

Ad esempio, se si desidera creare un report che mostri le attività con una data di inizio pianificata specifica, è possibile utilizzare il controllo selezione data calendario in un filtro per selezionare una data specifica. Tuttavia, se si desidera creare un report che mostri le attività che hanno la Data di inizio pianificata entro un determinato periodo di tempo dalla data di accesso al report, è possibile utilizzare un carattere jolly che indica che quando un utente visualizza il report, vengono visualizzate le informazioni relative a un periodo di tempo rilevante per il momento in cui visualizza il report.

Ad esempio nell&#39;ultima settimana, nell&#39;ultimo anno, nelle prossime due settimane e così via. In questo modo, il report viene creato una volta, ma poiché si utilizza un carattere jolly nel filtro, si ottengono risultati diversi ogni volta che un utente lo legge perché si adatta al giorno in cui esegue il report.

È possibile utilizzare caratteri jolly basati su date per la creazione dei seguenti elementi di reporting:

* Filtri
* Suggerimenti personalizzati
* Visualizzazioni durante l&#39;aggiunta di regole per le colonne

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
   <td> <p>Modificare l'accesso a filtri, viste, raggruppamenti</p> <p>Modificare l’accesso a report, dashboard e calendari per modificare gli elementi di reporting in un report</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
    <td> <p>Gestire le autorizzazioni per un report per modificare gli elementi di un report</p> <p>Gestire le autorizzazioni per una visualizzazione o un filtro per modificarle</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per poter aggiungere variabili jolly a un report, è necessario crearlo.

Per informazioni sulla creazione di un report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Procedure

Per inserire un carattere jolly basato su date in un report:

1. Passare a un report per il quale si desidera inserire un carattere jolly basato su date.
1. Fai clic su **Azioni report**, quindi su **Modifica**.
1. Fare clic sulla scheda **Filtri**.
1. Fare clic su **Aggiungi regola filtro**.
1. Inizia a digitare il nome del campo in base al quale filtrare i dati.\
   È necessario digitare i campi che fanno riferimento a una data.
1. Selezionare **Uguale** nel menu a discesa per la variabile di filtro.

   >[!TIP]
   >
   >Quando si utilizzano i caratteri jolly in Adobe Workfront, è sempre necessario selezionare la variabile di filtro **Equal**.

1. Fare clic sull&#39;interruttore **Imposta data relativa**, quindi nella casella di testo visualizzata digitare: `$$TODAY` se si desidera visualizzare informazioni su un evento che si verifica nello stesso giorno in cui viene eseguito il report.

   Oppure

   Digitare `$$NOW` se si desidera visualizzare informazioni su un evento che si verifica alla stessa data e ora di esecuzione del report.

   Questa data è sempre diversa, in quanto cambia a seconda della data in cui il report viene effettivamente visualizzato da un utente. pertanto, le informazioni contenute nel report sono diverse nei vari giorni.

1. (Facoltativo) Se si desidera visualizzare informazioni che si verificano entro un periodo di tempo successivo alla data di esecuzione del report, digitare `$$TODAY+1w` per visualizzare le informazioni nella settimana successiva oppure `$$TODAY+2m` per visualizzare le informazioni nei due mesi successivi. Puoi anche indicare gli intervalli di tempo per trimestri, ore, giorni o anni.
1. (Facoltativo) Se si desidera visualizzare informazioni su un evento verificatosi in un intervallo di tempo precedente alla data di esecuzione del report, digitare `$$TODAY-1w` per visualizzare le informazioni della settimana precedente oppure `$$TODAY-2m` per visualizzare le informazioni dei due mesi precedenti. Puoi anche indicare gli intervalli di tempo per trimestri, ore, giorni o anni.

   Per un elenco completo degli attributi, dei qualificatori e degli operatori che è possibile utilizzare nei caratteri jolly basati su date, vedere l&#39;articolo [Panoramica sulle variabili di filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Fai clic su **Salva e Chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Panoramica delle variabili di filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creazione o modifica di filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle viste](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

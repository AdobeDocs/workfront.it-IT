---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati sulla data per generalizzare i rapporti
description: È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---

# Utilizzare caratteri jolly basati sulla data per generalizzare i rapporti

<!-- Audited: 11/2024 -->

È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.

Ad esempio, se desideri creare un rapporto che mostri le attività con una data di inizio pianificata specifica, puoi utilizzare il selettore data calendario in un filtro per selezionare una data specifica. Tuttavia, se si desidera creare un report che mostri le attività che hanno la Data inizio pianificata entro un determinato intervallo di tempo dalla data in cui si accede al report, è possibile utilizzare un carattere jolly che indica che quando un utente visualizza il report, vengono visualizzate le informazioni per un intervallo di tempo rilevante per il momento in cui visualizza il report.

Ad esempio nell’ultima settimana, nell’ultimo anno, nelle prossime due settimane, ecc. In questo modo, il report verrà generato una volta, ma poiché si utilizza un carattere jolly nel filtro, il risultato sarà diverso ogni volta che qualcuno lo legge, in quanto si adatta al giorno in cui viene eseguito il report.

Puoi utilizzare caratteri jolly basati sulla data per creare i seguenti elementi di reporting:

* Filtri
* Richieste personalizzate
* Visualizzazioni durante l’aggiunta di regole per le colonne

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard e Calendari per modificare gli elementi di reporting in un rapporto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare gli elementi di reporting in un report</p> <p>Gestire le autorizzazioni per una visualizzazione o un filtro per modificarle</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare un report prima di poter aggiungere variabili con caratteri jolly.

Per informazioni sulla creazione di un report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Passaggi pratici

Per inserire un carattere jolly basato sulla data in un report:

1. Passare a un report per il quale si desidera inserire un carattere jolly basato sulla data.
1. Fai clic su **Azioni report**, quindi su **Modifica**.
1. Fare clic sulla scheda **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. Inizia a digitare il nome del campo in base al quale desideri filtrare.\
   È necessario digitare i campi che fanno riferimento a una data.
1. Seleziona **Uguale** nel menu a discesa per la variabile filtro.

   >[!TIP]
   >
   >È sempre necessario selezionare la variabile di filtro **Equal** quando si utilizzano i caratteri jolly in Adobe Workfront.

1. Fare clic sull&#39;interruttore **Imposta data relativa**, quindi nella casella di testo visualizzata digitare: `$$TODAY` se si desidera visualizzare informazioni su un evento che si verifica nello stesso giorno in cui viene eseguito il report.

   Oppure

   Digitare `$$NOW` se si desidera visualizzare informazioni su un evento che si verifica alla stessa data e ora di esecuzione del report.

   Questa data è sempre diversa, in quanto cambia con la data in cui il rapporto viene effettivamente visualizzato da un utente. le informazioni contenute nel rapporto sono quindi diverse da un giorno all’altro.

1. (Facoltativo) Se si desidera visualizzare le informazioni che si verificano in un intervallo di tempo successivo alla data di esecuzione del report, digitare `$$TODAY+1w` per visualizzare le informazioni nella settimana successiva oppure `$$TODAY+2m` per visualizzare le informazioni nei due mesi successivi. È inoltre possibile indicare gli intervalli di tempo per trimestri, ore, giorni o anni.
1. (Facoltativo) Se si desidera visualizzare informazioni su un evento che si è verificato in un intervallo di tempo precedente alla data di esecuzione del report, digitare `$$TODAY-1w` per visualizzare le informazioni della settimana precedente oppure `$$TODAY-2m` per visualizzare le informazioni dei due mesi precedenti. È inoltre possibile indicare gli intervalli di tempo per trimestri, ore, giorni o anni.

   Per un elenco completo degli attributi, dei qualificatori e degli operatori che è possibile utilizzare nei caratteri jolly basati sulla data, vedere l&#39;articolo [Panoramica delle variabili di filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Fai clic su **Salva e Chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

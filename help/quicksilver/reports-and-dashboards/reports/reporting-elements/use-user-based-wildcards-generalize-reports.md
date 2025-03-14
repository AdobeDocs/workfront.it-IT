---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati sull'utente per generalizzare i rapporti
description: È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Utilizzare caratteri jolly basati sull&#39;utente per generalizzare i rapporti

<!-- Audited: 11/2024 -->

È possibile generalizzare un rapporto utilizzando caratteri jolly anziché informazioni specifiche durante la creazione di determinati elementi di reporting. Ad esempio, se si desidera creare un report che mostri le attività assegnate a un utente specifico, è possibile utilizzare il nome dell&#39;utente nel campo Assegnato a del filtro. Tuttavia, se si desidera creare un report che mostra le attività assegnate all&#39;utente connesso, indipendentemente dall&#39;utente, è possibile utilizzare un carattere jolly che indichi che quando un utente visualizza il report, vengono visualizzate solo le informazioni che lo riguardano. In questo modo, il rapporto verrà generato una sola volta, ma poiché si utilizza un carattere jolly nel filtro, si otterranno risultati diversi ogni volta che verrà letto da un altro utente.

Puoi utilizzare caratteri jolly basati sugli utenti per creare i seguenti elementi di reporting:

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
* [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

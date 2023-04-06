---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati su data per generalizzare i rapporti
description: È possibile generalizzare un rapporto utilizzando caratteri jolly invece di informazioni specifiche quando si creano determinati elementi di reporting.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Utilizzare caratteri jolly basati su data per generalizzare i rapporti

È possibile generalizzare un rapporto utilizzando caratteri jolly invece di informazioni specifiche quando si creano determinati elementi di reporting.

Ad esempio, se desideri creare un rapporto che mostri le attività con una data di inizio pianificata specifica, puoi utilizzare il selettore della data del calendario in un filtro per selezionare una data specifica. Tuttavia, se si desidera creare un rapporto che mostri le attività con la data di inizio pianificata entro un determinato intervallo di tempo a partire dalla data di accesso al rapporto, è possibile utilizzare un carattere jolly che indica che quando un utente visualizza il rapporto visualizza le informazioni per un intervallo di tempo rilevante per il momento in cui visualizza il rapporto.

Ad esempio, nell&#39;ultima settimana, nell&#39;ultimo anno, nelle due settimane successive, ecc. In questo modo, puoi creare il rapporto una volta, ma poiché utilizzi un carattere jolly nel filtro, questo produce risultati diversi ogni volta che qualcuno lo legge, in quanto si adatta al giorno in cui esegue il rapporto.

È possibile utilizzare caratteri jolly basati su data durante la creazione dei seguenti elementi di reporting:

* Filtri
* Prompt personalizzati
* Visualizzazioni durante l&#39;aggiunta di regole per le colonne

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare gli elementi di reporting in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare gli elementi di reporting in un rapporto</p> <p>Gestisci le autorizzazioni per una visualizzazione o un filtro per modificarle</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un rapporto prima di poter aggiungere variabili con caratteri jolly.

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Procedura dettagliata

Per inserire un carattere jolly basato su data in un rapporto:

1. Passa a un rapporto per il quale desideri inserire un carattere jolly basato su data.
1. Fai clic su **Azioni dei rapporti**, quindi **Modifica**.

1. Fai clic sul pulsante **Filtri** scheda .
1. Fai clic su **Aggiungere una regola filtro**.
1. Inizia a digitare il nome del campo per il quale desideri filtrare.\
   È necessario digitare i campi che fanno riferimento a una data.
1. Seleziona **Uguale** nel menu a discesa per la variabile del filtro.

   >[!TIP]
   >
   >È sempre necessario selezionare le **Uguale** quando si utilizzano i caratteri jolly in Adobe Workfront.

1. In **Inizia a digitare il nome ...** casella, tipo: `$$TODAY` se si desidera visualizzare informazioni su un evento che si verifica nello stesso giorno in cui viene eseguito il rapporto.

   Oppure

   Tipo `$$NOW` se si desidera visualizzare informazioni su un evento che si verifica alla stessa data e ora di esecuzione del rapporto.

   Questa data è sempre diversa, in quanto cambia con la data in cui il rapporto viene effettivamente visualizzato da un utente. quindi le informazioni contenute nel rapporto sono diverse da giorno a giorno.

1. (Facoltativo) Se desideri visualizzare informazioni che si verificano entro un intervallo di tempo successivo alla data di esecuzione del rapporto, digita `$$TODAY+1w` per visualizzare le informazioni nella settimana successiva, oppure `$$TODAY+2m` per visualizzare le informazioni nei due mesi successivi. È inoltre possibile indicare i tempi per trimestri, ore, giorni o anni.
1. (Facoltativo) Se desideri visualizzare informazioni su qualcosa che si è verificato in un intervallo di tempo precedente alla data di esecuzione del rapporto, digita `$$TODAY-1w` per visualizzare le informazioni della settimana precedente, oppure `$$TODAY-2m` per visualizzare le informazioni dei due mesi precedenti. È inoltre possibile indicare i tempi per trimestri, ore, giorni o anni.

   Per un elenco completo degli attributi, dei qualificatori e degli operatori utilizzabili nei caratteri jolly basati su data, consulta l’articolo [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Fai clic su **Salva e chiudi**.

## Informazioni aggiuntive

Vedi anche:

* [Programma di creazione di rapporti di base](https://one.workfront.com/s/basic-report-creation-program)
* [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

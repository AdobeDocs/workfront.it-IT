---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare i caratteri jolly basati sull’utente per generalizzare i rapporti
description: È possibile generalizzare un rapporto utilizzando caratteri jolly invece di informazioni specifiche quando si creano determinati elementi di reporting.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Utilizzare i caratteri jolly basati sull’utente per generalizzare i rapporti

È possibile generalizzare un rapporto utilizzando caratteri jolly invece di informazioni specifiche quando si creano determinati elementi di reporting. Ad esempio, se desideri creare un rapporto che mostri le attività assegnate a un utente specifico, puoi utilizzare il nome dell’utente nel campo Assegnato a del filtro. Tuttavia, se desideri creare un rapporto che mostri le attività assegnate all’utente connesso, indipendentemente da chi sia tale utente, puoi utilizzare un carattere jolly che indica che quando un utente visualizza il rapporto visualizza solo le informazioni relative a tale utente. In questo modo, puoi creare il rapporto una volta, ma poiché utilizzi un carattere jolly nel filtro, questo genera risultati diversi ogni volta che un altro utente lo legge.

È possibile utilizzare caratteri jolly basati su utenti durante la creazione dei seguenti elementi di reporting:

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

È necessario creare un rapporto prima di poter aggiungere una variabile con caratteri jolly.

Per istruzioni sulla creazione dei rapporti, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Procedura dettagliata

Per inserire un carattere jolly basato su utente in un rapporto:

1. Passa a un rapporto per il quale desideri inserire un carattere jolly basato su utente.
1. Fai clic su **Azioni dei rapporti**, quindi **Modifica**.

1. Fai clic sul pulsante **Filtri** scheda .
1. Fai clic su **Aggiungere una regola filtro**.
1. Inizia a digitare il nome del campo per il quale desideri filtrare.\
   È necessario digitare i campi che fanno riferimento all&#39;oggetto utente o alle informazioni sugli utenti.
1. Seleziona **Uguale** nel menu a discesa per la variabile del filtro.

   >[!TIP]
   >
   >È sempre necessario selezionare le **Uguale** quando si utilizzano i caratteri jolly in Adobe Workfront.

1. In **Inizia a digitare il nome ...** casella, tipo: `$$USER.ID` o `$$USER.name` se desideri che il rapporto mostri informazioni sull’utente che effettua l’accesso, in base al suo nome. È possibile inserire altri caratteri jolly che fanno riferimento al gruppo, al team, alla società o ad altre informazioni dell&#39;utente connesso.

   Per un elenco completo dei caratteri jolly basati sull’utente, consulta [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Fai clic su **Salva e chiudi**.

## Informazioni aggiuntive

Vedi anche:

* [Programma di creazione di rapporti di base](https://one.workfront.com/s/basic-report-creation-program)
* [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

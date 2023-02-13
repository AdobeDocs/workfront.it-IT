---
product-area: reporting
navigation-topic: reporting-elements
title: "Elementi di reporting: filtri, visualizzazioni e raggruppamenti"
description: Gli elementi principali che ogni elenco e rapporto deve avere in Workfront sono un filtro, una visualizzazione e un raggruppamento. Ogni elemento fornisce informazioni diverse all’interno di qualsiasi rapporto.
author: Lisa
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Elementi di reporting: filtri, visualizzazioni e raggruppamenti

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

In Adobe Workfront sono disponibili diversi elementi per rendere possibile un elenco o un rapporto. Gli elementi principali che ogni elenco e rapporto deve contenere sono un filtro, una visualizzazione e un raggruppamento. Ogni elemento fornisce informazioni diverse all’interno di qualsiasi rapporto.

## Considerazioni sugli elementi di reporting

Quando lavori con filtri, viste e raggruppamenti, considera quanto segue:

* Gli elementi di reporting funzionano come elementi costitutivi del reporting. Definiscono l’aspetto di un rapporto o di un elenco, nonché le informazioni contenute nel rapporto o nell’elenco.
* I rapporti in Workfront sono specifici di un oggetto. È necessario definire l’oggetto principale per un rapporto prima di poterlo generare. Pertanto, tutti gli elementi di reporting sono specifici per un oggetto.
* L’amministratore di Workfront deve concedere l’accesso a filtri, visualizzazioni e raggruppamenti nel livello di accesso per poterli visualizzare o modificare in elenchi e rapporti.

   Per informazioni sulla concessione dell’accesso a filtri, visualizzazioni e raggruppamenti, consulta [Consentire l’accesso a filtri, visualizzazioni e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Per poter visualizzare o modificare i rapporti, l’amministratore di Workfront deve concedere all’utente l’accesso a rapporti, dashboard e calendari a livello di accesso.

   Per informazioni sulla concessione dell’accesso a rapporti, dashboard e calendari, consulta [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Se selezioni un filtro, una visualizzazione o un raggruppamento in un report o in un elenco, Workfront mantiene questa selezione per gli elenchi di tale oggetto anche dopo la disconnessione o la chiusura del browser. Ad esempio, se si seleziona una visualizzazione specifica per un rapporto di attività, tale selezione verrà visualizzata per altri elenchi di attività, ad esempio l&#39;elenco delle attività di un progetto.

## Filtri

Il filtro controlla i risultati visualizzati in un rapporto, in genere restringendo i risultati da generali a specifici. Funziona come un setaccio solo afferrando le informazioni necessarie e riportando quelle informazioni al tuo rapporto.

Ad esempio, se desideri visualizzare solo le attività assegnate all’utente connesso, puoi creare un filtro denominato &quot;Attività personali&quot;, definire i criteri da soddisfare per il filtro ed eseguire il rapporto per visualizzare solo le attività assegnate all’utente connesso.

Alcuni attributi dei filtri sono:

* Per impostazione predefinita, Workfront fornisce diversi filtri per vari oggetti.
* Puoi personalizzare i filtri di tua proprietà o gestirli.

   Per ulteriori informazioni sui filtri, consulta l’articolo [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Icona filtro](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Viste

Definendo la visualizzazione di un rapporto, si definiscono le informazioni incluse nel rapporto. Come tutti gli elementi di reporting, le visualizzazioni si basano su un unico tipo di oggetto.\
Ad esempio, una visualizzazione per un report attività potrebbe mostrare le date di scadenza, includere dettagli finanziari chiave come Costo o essere utilizzata per visualizzare i dettagli di Assegnazioni e Data consegna. Le visualizzazioni possono essere utilizzate per fornire una varietà di dettagli sui dati nel rapporto.

Alcuni attributi delle visualizzazioni sono:

* È possibile utilizzare una visualizzazione Workfront predefinita oppure crearne una personalizzata.
* Puoi applicare ulteriori viste dal campo a discesa Visualizza dopo aver eseguito un rapporto.
* Le visualizzazioni aggiuntive sostituiscono temporaneamente la visualizzazione definita durante la creazione del rapporto; tuttavia, la visualizzazione predefinita viene visualizzata al successivo ritorno al rapporto.

   Per ulteriori informazioni sulle visualizzazioni, consulta l’articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Raggruppamenti

Un raggruppamento controlla la modalità di organizzazione dei dati, facilitando la lettura e la comprensione. I raggruppamenti creano barre orizzontali in un rapporto che mostrano i risultati elencati insieme da attributi comuni. Puoi definire i criteri per la modalità di raggruppamento dei risultati del rapporto durante la creazione del raggruppamento.

Ad esempio, se si raggruppa un elenco di attività che si estendono su più progetti in base al nome del progetto, vengono organizzate tutte le rispettive attività che appartengono a un singolo progetto con tale nome.

Alcuni attributi dei raggruppamenti sono:

* I raggruppamenti sono un elemento di reporting obbligatorio se desideri aggiungere in seguito un grafico al rapporto.
* I raggruppamenti visualizzano un valore aggregato nei risultati. &#x200B;
* I raggruppamenti determinano l&#39;asse nei grafici.
* I raggruppamenti determinano l’identificazione dell’intestazione nei rapporti sulle matrici.\
   Per ulteriori informazioni sui rapporti sulla matrice, consulta l’articolo [Creare un rapporto sulla matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* I raggruppamenti consentono di creare la scheda Riepilogo di un rapporto, fornendo i valori aggregati del rapporto.
* Per impostazione predefinita, in Workfront sono disponibili diversi raggruppamenti per oggetti diversi.
* Puoi personalizzare i raggruppamenti di tua proprietà o gestirli.

   Per ulteriori informazioni sui raggruppamenti, vedi [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Altri elementi di segnalazione

Oltre a filtri, visualizzazioni e raggruppamenti, puoi aggiungere a un rapporto anche i seguenti elementi:

* **Prompt**: Filtro aperto che può essere personalizzato e applicato in modo diverso ogni volta che si esegue un rapporto.\
   Per ulteriori informazioni sui prompt, consulta l’articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Grafico**: Puoi migliorare i rapporti aggiungendo un grafico e visualizzando le informazioni in modo visivo.\
   Per ulteriori informazioni sui grafici nei rapporti, consulta l’articolo [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

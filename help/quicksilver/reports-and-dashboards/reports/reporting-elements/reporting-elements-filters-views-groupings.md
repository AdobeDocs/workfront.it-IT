---
product-area: reporting
navigation-topic: reporting-elements
title: "Elementi di reporting: filtri, visualizzazioni e raggruppamenti"
description: Gli elementi principali di ogni elenco e rapporto in Workfront sono un filtro, una vista e un raggruppamento. Ogni elemento fornisce informazioni diverse all’interno di qualsiasi rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Elementi di reporting: filtri, viste e raggruppamenti

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

In Adobe Workfront sono disponibili diversi elementi che rendono possibile la creazione di un elenco o di un rapporto. Gli elementi principali di ogni elenco e report sono un filtro, una visualizzazione e un raggruppamento. Ogni elemento fornisce informazioni diverse all’interno di qualsiasi rapporto.

## Considerazioni sugli elementi di reporting

Quando si lavora con filtri, viste e raggruppamenti, considera quanto segue:

* Gli elementi di reporting funzionano come elementi costitutivi del reporting. Definiscono l’aspetto di un rapporto o di un elenco, nonché le informazioni contenute nel rapporto o nell’elenco.
* I report in Workfront sono specifici per un oggetto. È necessario definire l&#39;oggetto principale per un report prima di poterlo creare. Pertanto, tutti gli elementi di reporting sono specifici per oggetto.
* L’amministratore di Workfront deve concedere l’accesso a filtri, viste e raggruppamenti nel livello di accesso per poterli visualizzare o modificare in elenchi e rapporti.

  Per informazioni su come concedere l&#39;accesso a filtri, viste e raggruppamenti, vedere [Concedere l&#39;accesso a filtri, viste e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Per poter visualizzare o modificare i rapporti, l’amministratore di Workfront deve concedere l’accesso a rapporti, dashboard e calendari nel tuo livello di accesso.

  Per informazioni sulla concessione dell&#39;accesso a report, dashboard e calendari, vedere [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Se si seleziona un filtro, una visualizzazione o un raggruppamento per un report o un elenco, Workfront mantiene la selezione per gli elenchi dell&#39;oggetto anche dopo la disconnessione o la chiusura del browser. Se ad esempio si seleziona una visualizzazione specifica per un report attività, tale selezione verrà visualizzata per altri elenchi di attività, ad esempio l&#39;elenco delle attività di un progetto.

## Filtri

Il filtro controlla i risultati visualizzati in un rapporto, in genere restringendo i risultati da generali a specifici. Funziona come un setaccio che acquisisce solo le informazioni necessarie e le riporta al report.

Ad esempio, se desideri visualizzare solo le attività assegnate all’utente connesso, puoi creare un filtro denominato &quot;Le mie attività&quot;, definire i criteri che devono essere soddisfatti dal filtro ed eseguire il rapporto per visualizzare solo le attività assegnate all’utente connesso.

Alcuni attributi dei filtri sono:

* Per impostazione predefinita, Workfront fornisce una serie di filtri per vari oggetti.
* Puoi personalizzare i filtri di tua proprietà o gestirli.

  Per ulteriori informazioni sui filtri, vedere l&#39;articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Viste

Definendo la visualizzazione di un rapporto, si definiscono le informazioni da includere nel rapporto. Come tutti gli elementi di reporting, le visualizzazioni si basano su un tipo di oggetto.

Ad esempio, una visualizzazione per un report attività potrebbe mostrare le Date di scadenza, includere dettagli finanziari chiave come il Costo o essere utilizzata per mostrare le assegnazioni e i dettagli della Data di consegna. Le visualizzazioni possono essere utilizzate per fornire una varietà di dettagli sui dati nel rapporto.

Alcuni attributi delle viste sono:

* È possibile utilizzare una visualizzazione predefinita di Workfront oppure crearne una personalizzata.
* Dopo aver eseguito un rapporto, puoi applicare visualizzazioni aggiuntive dal campo a discesa Visualizza.
* Le viste aggiuntive sostituiscono temporaneamente la vista definita durante la creazione del rapporto; tuttavia, la vista predefinita viene visualizzata al successivo ritorno al rapporto.

  Per ulteriori informazioni sulle visualizzazioni, vedere l&#39;articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Raggruppamenti

Un raggruppamento controlla come organizzare i dati, semplificandone la lettura e la comprensione. I raggruppamenti creano barre orizzontali in un rapporto che visualizzano i risultati elencati insieme in base agli attributi comuni. È possibile definire i criteri per la modalità di raggruppamento dei risultati del rapporto durante la creazione del raggruppamento.

Ad esempio, raggruppando un elenco di attività che si estendono su più progetti in base al nome del progetto, vengono organizzate tutte le rispettive attività che appartengono a un singolo progetto con tale nome.

Alcuni attributi dei raggruppamenti sono:

* I raggruppamenti sono un elemento obbligatorio per la generazione di rapporti se in seguito si desidera aggiungere un grafico al rapporto.
* I raggruppamenti visualizzano un valore aggregato nei risultati.&#x200B;
* I raggruppamenti determinano l&#39;asse nei grafici.
* I raggruppamenti determinano l’identificazione dell’intestazione nei rapporti matrice.\
  Per ulteriori informazioni sui report matrice, vedere l&#39;articolo [Creare un report matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* I raggruppamenti consentono di creare la scheda Riepilogo di un rapporto, fornendo i valori aggregati del rapporto.
* Per impostazione predefinita, Workfront fornisce una serie di raggruppamenti per oggetti diversi.
* È possibile personalizzare i raggruppamenti di cui si è proprietari o che si gestiscono.

  Per ulteriori informazioni sui raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Altri elementi di reporting

Oltre a filtri, viste e raggruppamenti, puoi aggiungere a un rapporto i seguenti elementi:

* **Prompt**: filtro aperto che può essere personalizzato e applicato in modo diverso ogni volta che si esegue un report.\
  Per ulteriori informazioni sui prompt, vedere l&#39;articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Grafico**: è possibile migliorare i report aggiungendo un grafico e visualizzando le informazioni in modo visivo.\
  Per ulteriori informazioni sui grafici nei report, vedere l&#39;articolo [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

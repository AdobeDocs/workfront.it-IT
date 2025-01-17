---
product-area: reporting
navigation-topic: text-mode-reporting
title: Panoramica sulla modalità testo
description: È possibile creare un rapporto o un elenco in Adobe Workfront utilizzando l’interfaccia standard o in modalità testo durante la creazione degli elementi che compongono il rapporto o l’elenco.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Panoramica sulla modalità testo

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

È possibile creare un rapporto o un elenco in Adobe Workfront utilizzando l’interfaccia standard o in modalità testo durante la creazione degli elementi che compongono il rapporto o l’elenco.

L’interfaccia standard ti consente di fare riferimento ai campi e ai relativi attributi che sono prontamente disponibili nell’interfaccia di Workfront.

Utilizzando la modalità testo è possibile fare riferimento a campi e attributi che potrebbero non essere disponibili in modalità standard, ma che sono disponibili nel database di Workfront.

Per ulteriori informazioni sulla creazione di rapporti utilizzando la modalità testo, inclusi classi, video e tutorial, consulta la sezione Informazioni sul sito Adobe Experience League.

## Considerazioni prima di utilizzare la modalità testo

>[!TIP]
>
>È inoltre possibile espandere le funzionalità dei campi personalizzati calcolati utilizzando una versione della modalità testo per i campi personalizzati. La sintassi e le regole per la creazione di un campo personalizzato calcolato sono diverse da quelle utilizzate nei report e negli elenchi. Per informazioni sull&#39;aggiunta di un campo personalizzato calcolato, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Prima di iniziare a utilizzare la modalità testo nei rapporti, consigliamo vivamente di seguire le nostre lezioni sui rapporti avanzati per comprendere meglio il linguaggio della modalità testo.
* È consigliabile utilizzare la modalità standard per garantire che i rapporti creati rimangano intatti quando il software Workfront viene aggiornato. Anche se la modalità testo consente di creare visualizzazioni, filtri e raggruppamenti più complessi, è più complessa da mantenere e non è garantita quando il software Workfront viene aggiornato.
* È consigliabile creare sempre tutti gli elementi di reporting nell’interfaccia standard e passare al generatore della modalità testo solo per alcune regolazioni.

  >[!TIP]
  >
  >L’utilizzo del generatore standard offre blocchi predefiniti e pattern di codice importanti che possono essere utilizzati quando si modifica il codice in modalità testo.

* Per creare correttamente report ed elenchi in modalità testo, è necessario utilizzare un set di regole e una sintassi univoca. Prima di iniziare, assicurati di avere familiarità con la sintassi Workfront per la modalità testo.

  Per informazioni sulla sintassi e sulle regole per l&#39;utilizzo della modalità testo, vedere [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Dopo aver personalizzato un elemento di reporting in modalità testo, potrebbe non essere possibile tornare alla modalità standard (in una visualizzazione) oppure il codice dell’elemento creato potrebbe essere eliminato (in filtri e raggruppamenti). Questo perché non tutti i campi supportati in modalità testo sono supportati in modalità standard.

## Interfaccia in modalità standard

Nell&#39;interfaccia della modalità Standard vengono visualizzati i campi per la mappatura degli elementi dell&#39;applicazione che si desidera visualizzare in un report o in un elenco. L’interfaccia in modalità standard è un set di menu a discesa dai quali è possibile selezionare i campi da visualizzare nei rapporti o negli elenchi.

Per ulteriori informazioni sull’interfaccia in modalità standard e su come creare un rapporto o un elenco, consulta:

* [Crea un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Elementi di reporting: filtri, viste e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Interfaccia modalità testo

La modalità testo consente di creare visualizzazioni, filtri, raggruppamenti e prompt più complessi, consentendo di utilizzare campi non disponibili nell&#39;interfaccia della modalità standard. In modalità testo di Workfront è un insieme di istruzioni codificate che indicano gli oggetti che si desidera visualizzare in un report o in un elenco.

Per un elenco completo di tutti i campi da segnalare, consulta [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Non tutti i campi disponibili tramite l’API sono disponibili tramite l’interfaccia in modalità testo. Se utilizzi il campo corretto nel codice in modalità testo e non visualizzi i risultati previsti, il campo potrebbe essere segnalato solo tramite l’API.

## Accedere agli elementi di reporting e modificare la modalità testo {#access-reporting-elements-and-edit-text-mode}

L’accesso all’interfaccia della modalità testo è simile per viste, raggruppamenti e filtri, quando si accede a essi da un rapporto o da un elenco.

Per informazioni sull’utilizzo della modalità testo in viste, filtri e raggruppamenti, consulta:

* [Modificare una visualizzazione utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Modifica un filtro in modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Modificare un raggruppamento utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

I prompt personalizzati possono essere modificati solo in modalità testo. È possibile accedere alle richieste solo da un report.

Per informazioni sull&#39;accesso all&#39;interfaccia in modalità testo per i prompt personalizzati, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Motivi comuni per l’utilizzo della modalità testo {#common-reasons-to-use-text-mode}

Al di fuori della creazione di prompt personalizzati che possono essere configurati solo utilizzando la modalità testo, è consigliabile utilizzare il generatore di rapporti per creare visualizzazioni, filtri e raggruppamenti. Tuttavia, in alcuni casi è possibile utilizzare la modalità testo per migliorare i rapporti e gli elenchi.

Per ulteriori informazioni sugli usi comuni per la modalità testo, vedere [Panoramica sugli usi comuni per la modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

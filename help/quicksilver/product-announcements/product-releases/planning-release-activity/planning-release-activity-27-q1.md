---
content-type: release-notes
title: Attività della versione del primo trimestre 2027 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il primo trimestre 2027.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 949503fecba92a7b8536b4af0b9c684e7f9e3300
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 0%
---
# Attività della versione del primo trimestre 2027 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del primo trimestre 2027.

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Migliore visibilità dei risultati della ricerca rapida nella vista a tabella

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Quando si utilizza la ricerca rapida nella vista tabella per trovare un elemento, vengono eliminati tutti i record che non corrispondono alla ricerca e vengono visualizzati solo gli elementi corrispondenti.

Prima di questo miglioramento, tutti i record venivano visualizzati con quelli che corrispondono ai risultati di ricerca evidenziati.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## Consenti la connessione di record globali di tipi di record connessi nelle aree di lavoro secondarie quando la connettività tra aree di lavoro diverse è disattivata

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Quando due tipi di record globali connessi vengono aggiunti a un&#39;area di lavoro secondaria, è ora possibile disattivare la connettività tra aree di lavoro diverse e collegare comunque i record localmente. Ogni area di lavoro secondaria visualizza solo i propri record per entrambi i tipi di record e può collegarli tra loro. I record dell&#39;area di lavoro globale e di altre aree di lavoro secondarie non vengono più visualizzati.

Prima di questo miglioramento, se la connettività tra aree di lavoro diverse era disattivata per i tipi di record globali connessi, le aree di lavoro secondarie non potevano collegare tra loro i propri record. Se questa opzione è attivata, gli utenti possono visualizzare e collegare i record dall&#39;area di lavoro globale e da tutte le altre aree di lavoro secondarie.

Per ulteriori informazioni, vedere [Panoramica del tipo di record tra aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Visualizzare il conteggio totale dei record nelle visualizzazioni tabella

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Nella vista tabella viene ora visualizzato il numero totale di record e il conteggio viene aggiornato automaticamente quando si applicano filtri, si esegue una ricerca o si modifica la vista. Il conteggio dei record riflette sempre i risultati filtrati completi e rispetta le autorizzazioni.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## Limitazioni del numero di campo di ricerca

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Stiamo introducendo limiti sul numero di campi di ricerca che è possibile aggiungere a un tipo di record:

* Fino a 40 campi di ricerca per tipo di record
* Fino a 5 campi di ricerca a testo lungo per tipo di record. I campi di ricerca connessi vengono conteggiati rispetto al limite del campo originale.
* Fino a 50.000 caratteri nel valore di una singola cella di ricerca di testo lungo. Se il contenuto combinato dei valori di ricerca supera questo limite, i valori vengono visualizzati in ordine di connessione fino al raggiungimento del limite. Vengono omessi il primo valore che lo supererebbe e tutti i valori successivi. Il campo oggetto connesso originale non viene mai modificato.

Viene visualizzato un errore quando si tenta di creare o modificare un campo di ricerca oltre i primi due limiti. Questa modifica non ha effetto sui tipi di record che superano già questi limiti. Puoi modificarli, ma non puoi aggiungere altri campi o valori di ricerca fino a quando non sei al di sotto del limite.

Per informazioni, vedere [Panoramica delle limitazioni degli oggetti di Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

## I nuovi campi ora vengono visualizzati solo nella visualizzazione in cui sono stati creati

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Quando si aggiunge un nuovo campo a un tipo di record, questo viene visualizzato solo nella visualizzazione in cui si sta lavorando e viene nascosto in tutte le altre visualizzazioni esistenti. Le altre visualizzazioni rimangono configurate e, se necessario, puoi scoprire il nuovo campo al loro interno.

Prima di questo miglioramento, i nuovi campi venivano aggiunti in modo visibile a ogni visualizzazione, generando talvolta confusione per gli utenti che non conoscevano i nuovi campi.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Esporta dettagli record da qualsiasi visualizzazione

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

È ora possibile esportare i dettagli di un record da qualsiasi visualizzazione dei dettagli, senza dover passare alla visualizzazione Tutti i campi.

In precedenza, l’opzione di esportazione era disponibile solo quando era selezionata la vista Tutti i campi.

Per informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## Prestazioni migliorate con il caricamento di dati incrementali nelle viste tabella e timeline

<!-- NOTE FROM CSV: Must check with Lilit whether this will come to the timeline view in addition to the table (Lilit said yes; this was messaged before but pulled). The second bullet will change; check with Lilit first. -->

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

Per migliorare le prestazioni su un gran numero di record, sono stati apportati i seguenti miglioramenti alle viste tabella e timeline:

* La visualizzazione ora carica inizialmente i primi 500 record, con i record aggiuntivi caricati automaticamente mentre si scorre in batch di 500.
* La ricerca e il raggruppamento rapidi influiscono solo sui record attualmente caricati nella visualizzazione.

Per informazioni, vedere [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md) e [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## Riordinamento manuale dei raggruppamenti nella vista timeline

>[!NOTE]
>
>Anteprima: 29 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

È ora possibile trascinare e rilasciare raggruppamenti, sottogruppi e record per creare un ordine personalizzato nella visualizzazione timeline. La disposizione manuale viene mantenuta per tutte le sessioni e puoi passare facilmente dall’ordinamento manuale all’ordinamento basato sui campi in base alle esigenze di pianificazione.

La funzionalità di trascinamento della selezione è disponibile sia per le corsie sia per le versioni in pila della vista timeline.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Regole aziendali per i tipi di record globali

>[!NOTE]
>
>Anteprima: 28 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

I responsabili di Workspace possono ora configurare le regole business sui tipi di record globali sia nelle aree di lavoro principali che secondarie. Le regole vengono applicate a tutti i record dello stesso tipo in tutte le aree di lavoro in cui vengono aggiunte.

Le regole business aggiunte nelle aree di lavoro globali vengono visualizzate in sola lettura nelle aree di lavoro secondarie in cui sono stati importati i tipi di record. Le regole business aggiunte nelle aree di lavoro secondarie vengono visualizzate in sola lettura nelle aree di lavoro primarie in cui sono stati creati i tipi di record. Le regole possono essere modificate solo nelle aree di lavoro in cui vengono create.

Per informazioni, vedere [Configurare le regole business di tipo record](/help/quicksilver/planning/architecture/configure-business-rules.md).

## Impostare le impostazioni di richiesta predefinite per la funzionalità Compila modulo nelle richieste di Planning

>[!NOTE]
>
>Anteprima: 21 ottobre 2026
>Versione rapida di produzione: 12 novembre 2026
>Produzione per tutti: 21 gennaio 2027

È ora possibile personalizzare la richiesta visualizzata dagli utenti quando si utilizza la funzionalità del modulo Riempimento basato su IA durante l’invio di una richiesta Planning.

È possibile creare un prompt predefinito durante la creazione di un modulo di richiesta per le richieste di Planning.

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

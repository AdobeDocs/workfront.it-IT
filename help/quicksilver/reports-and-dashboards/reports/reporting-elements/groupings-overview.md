---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Panoramica sui raggruppamenti in Adobe Workfront
description: È possibile aggiungere raggruppamenti per gestire il layout delle informazioni nei rapporti e negli elenchi.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Panoramica sui raggruppamenti in Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

È possibile aggiungere raggruppamenti per gestire il layout delle informazioni nei rapporti e negli elenchi.

Puoi aggiungere i raggruppamenti ai rapporti nei seguenti modi:

* È possibile creare raggruppamenti modificando i raggruppamenti esistenti.

   Per informazioni sulla personalizzazione di un raggruppamento esistente, consulta [Modificare i raggruppamenti esistenti](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Puoi creare raggruppamenti da zero.

   Per informazioni sulla creazione di un raggruppamento da zero, consulta [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Per impostazione predefinita, i raggruppamenti sono evidenziati in grigio o blu nel rapporto o nell’elenco. I risultati del rapporto o dell’elenco sono elencati in base al loro raggruppamento individuale, senza evidenziazione.

È possibile aggiungere fino a tre raggruppamenti a un rapporto. Puoi organizzare le informazioni con un massimo di quattro raggruppamenti creando un rapporto a matrice. Per ulteriori informazioni sui rapporti sulle matrici, vedi [Creare un rapporto sulla matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

In un rapporto di raggruppamento standard, il primo raggruppamento è di colore più scuro, il secondo e il terzo gruppo sono più chiari. Non puoi personalizzare il colore dell’evidenziazione per il raggruppamento o il font del nome del raggruppamento. Il numero tra parentesi dopo il nome del raggruppamento rappresenta il numero di risultati sotto tale raggruppamento. Se il rapporto si estende su più pagine, assicurati di visualizzare *Tutto* i risultati nel rapporto o nell’elenco per ottenere un conteggio accurato dei risultati in ciascun raggruppamento.

![Raggruppamento di campioni](assets/grouping-example-blue.png)

Quando si lavora con i raggruppamenti, tenere presente quanto segue:

* È possibile personalizzare le informazioni contenute nei raggruppamenti esistenti. Anche tutti gli utenti che possono visualizzare i raggruppamenti possono vedere le modifiche.
* Per creare gruppi, l’amministratore di Workfront deve concedere l’accesso a Modifica filtri, visualizzazioni e gruppi .

   Per informazioni sulla concessione dell’accesso a Filtri, Visualizzazioni e Gruppi, consulta [Consentire l’accesso a filtri, visualizzazioni e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Il livello di autorizzazioni di un raggruppamento determina la modalità di salvataggio di un raggruppamento. Se il raggruppamento è stato creato originariamente, è possibile salvare le modifiche; in caso contrario viene richiesto di salvare una versione del raggruppamento. Se apporti modifiche a un raggruppamento condiviso con altri, questo avrà un impatto anche su di essi.
* Puoi personalizzare un raggruppamento condiviso con te solo se l’utente che lo ha condiviso ti ha concesso l’accesso Gestione . Per informazioni sulla condivisione di un raggruppamento, vedi [Condividere un filtro, una visualizzazione o un raggruppamento](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Non è possibile modificare un raggruppamento in linea.
* Non è possibile raggruppare i campi personalizzati per selezione multipla (ad esempio, caselle di controllo) o per campi che possono avere più valori (ad esempio, Gestione risorse).

## Informazioni aggiuntive sui raggruppamenti

È possibile gestire ulteriormente le informazioni del rapporto quando si utilizzano i Raggruppamenti aggregando i valori in ciascuna colonna della riga Raggruppamento e ordinando le informazioni in base al campo del raggruppamento. È inoltre possibile rimuovere un raggruppamento quando non è più necessario.

* [Aggregazione di valori in raggruppamenti](#aggregate-values-in-groupings)
* [Ordina per raggruppamento](#sort-by-a-grouping)
* [Rimuovere un raggruppamento](#remove-a-grouping)

### Aggregazione di valori in raggruppamenti {#aggregate-values-in-groupings}

Puoi aggregare i dati visualizzati nel rapporto nella riga di raggruppamento riepilogando i valori in ogni colonna del rapporto. Per ulteriori informazioni sul riepilogo dei dati delle colonne in un raggruppamento, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Le seguenti eccezioni si applicano agli oggetti principali (ad esempio, le attività principali) quando si aggregano valori per i seguenti campi nei raggruppamenti:
>
>* Tutti i campi relativi al numero e alla divisa, ad eccezione delle ore effettive (ad esempio, Costo manodopera pianificato/effettivo, Costo spesa pianificato/effettivo, Costo pianificato/effettivo, Ore pianificate) aggregano solo i valori relativi alle attività figlio e alle attività autonome. Non aggregano i valori per le attività principali o le attività principali dei genitori.
>* Le ore effettive aggregano i valori per le attività principali e le attività autonome; non aggregano i numeri relativi alle attività principali o alle attività figlio per le attività padre.
>* I campi dati personalizzati per i valori di numero e valuta aggregano tutte le attività: genitori, figli, genitori di genitori e compiti autonomi.


### Ordina per raggruppamento {#sort-by-a-grouping}

I raggruppamenti non possono essere ordinati. Le visualizzazioni possono essere ordinate. Per ordinare un elenco in base al valore acquisito nel raggruppamento, è necessario includere lo stesso valore in una delle colonne della visualizzazione e applicare l’ordinamento nella visualizzazione. In questo modo, l’elenco effettua l’ordinamento in base al valore nel raggruppamento indirettamente (ordina in base al valore nella visualizzazione che viene acquisito anche nel raggruppamento). Per ulteriori informazioni sulla creazione delle viste e sull’ordinamento in base ai valori all’interno delle viste, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Rimuovere un raggruppamento {#remove-a-grouping}

La modalità di rimozione di un raggruppamento dipende dal fatto che il raggruppamento sia stato creato inizialmente o sia stato condiviso con te. Non è possibile rimuovere un raggruppamento predefinito.

* **Se hai creato il raggruppamento e lo rimuovi**, il raggruppamento viene rimosso dal sistema Workfront. Il raggruppamento non è più disponibile per gli utenti con cui lo hai condiviso in precedenza.
* **Se il raggruppamento è stato condiviso con te e lo rimuovi**, il raggruppamento viene rimosso solo per voi. L’utente che lo ha creato originariamente e tutti gli altri utenti con cui è stato condiviso hanno ancora accesso al raggruppamento.

Per informazioni sulla rimozione di un raggruppamento, consulta l’articolo [Rimuovere filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

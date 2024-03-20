---
title: Gestire la visualizzazione calendario
description: È possibile visualizzare i record e i relativi campi in una visualizzazione calendario.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Gestire la visualizzazione calendario

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

È possibile visualizzare i record e i relativi campi in una visualizzazione calendario dalla pagina del tipo di record.

Per informazioni sulle visualizzazioni delle funzionalità di pianificazione di Adobe Workfront e su come gestirle, consulta [Gestire le visualizzazioni record](../views/manage-record-views.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso delle funzionalità di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Configurazione del livello di accesso</td>
   <td> <p>Non sono disponibili controlli del livello di accesso per le funzionalità di pianificazione di Adobe Workfront  </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per la visualizzazione</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Gestire una visualizzazione calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Considera quanto segue:

* È possibile creare una visualizzazione Calendario solo se a un tipo di record sono associati almeno due campi data. Quando a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Calendario non è attiva.
* Esistono i seguenti scenari:

   * Se le date di inizio e di fine non contengono valori, i record non vengono visualizzati nel calendario
   * Quando le date di inizio o fine non hanno un valore, il record viene visualizzato come evento di un giorno
   * Se la data di inizio è successiva alla data di fine, il record non viene visualizzato nel calendario.

Per gestire una vista calendario:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare il calendario.
1. Creare una visualizzazione calendario come descritto nell&#39;articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   I record associati al tipo di record selezionato vengono visualizzati come barre in un calendario. Il colore delle barre corrisponde al colore dell&#39;icona del record.

1. Per spostarsi nel calendario, effettuare una delle seguenti operazioni:

   * Fare clic sulle icone sinistra e destra oppure utilizzare lo scorrimento orizzontale per spostarsi all&#39;indietro e in avanti nel calendario.
   * Clic **Oggi** per centrare il calendario alla data odierna.
   * Per aggiornare gli incrementi di tempo, seleziona una delle seguenti opzioni dal menu a discesa dell’intervallo di tempo:

      * Mese
1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Aggiungere filtri

È possibile ridurre la quantità di informazioni visualizzate sullo schermo utilizzando i filtri.

Quando si lavora con i filtri nella vista calendario, considera quanto segue:

<!-- this list is almost identical to the one for the table view - update both-->

* I filtri creati per una visualizzazione calendario funzionano indipendentemente dai filtri di qualsiasi altra visualizzazione applicata allo stesso tipo di record.

* I filtri sono univoci per la vista selezionata. A due visualizzazioni calendario dello stesso tipo di record possono essere applicati filtri diversi.

* Due utenti che visualizzano la stessa vista calendario visualizzano lo stesso filtro attualmente applicato.

* Non è possibile denominare i filtri creati per una visualizzazione calendario.

* Se si rimuovono i filtri, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.

* L&#39;aggiunta di filtri nella vista calendario è identica all&#39;aggiunta di filtri nella vista tabella.

  Per ulteriori informazioni, consulta la sezione &quot;Aggiungere filtri&quot; nell’articolo [Gestire la vista tabella](/help/quicksilver/maestro/views/manage-the-table-view.md).

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi, ma non per i campi che consentono il collegamento a più record.

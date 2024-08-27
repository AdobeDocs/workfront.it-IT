---
title: Gestire la visualizzazione calendario
description: È possibile visualizzare i record e i relativi campi in una visualizzazione calendario.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Gestire la visualizzazione calendario

{{planning-important-intro}}

È possibile visualizzare i record e i relativi campi in una visualizzazione calendario dalla pagina del tipo di record.

Per informazioni sulle visualizzazioni di Adobe Workfront Planning e su come gestirle, vedere [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su ciò che è incluso in ogni piano di Workfront Planning, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Determinazione prezzi e packaging di Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Autorizzazioni di visualizzazione per modificare temporaneamente le impostazioni di visualizzazione</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Gestire una visualizzazione calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Considera quanto segue:

* È possibile creare una visualizzazione Calendario solo se a un tipo di record sono associati almeno due campi data. Quando a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Calendario non è attiva.

  È possibile selezionare i campi della data di record o i campi della data di ricerca dai tipi di oggetto o record collegati.
* Esistono i seguenti scenari:

   * Se le date di inizio e di fine non contengono valori, i record non vengono visualizzati nel calendario
   * Quando le date di inizio o fine non hanno un valore, il record viene visualizzato come evento di un giorno
   * Se la data di inizio è successiva alla data di fine, il record non viene visualizzato nel calendario.

Per gestire una vista calendario:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare il calendario.
1. Creare una visualizzazione calendario come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   I record associati al tipo di record selezionato vengono visualizzati come barre in un calendario. Il colore delle barre corrisponde al colore dell&#39;icona del record.

1. Per spostarsi nel calendario, effettuare una delle seguenti operazioni:

   * Fare clic sulle icone sinistra e destra oppure utilizzare lo scorrimento orizzontale per spostarsi all&#39;indietro e in avanti nel calendario.
   * Fai clic su **Oggi** per centrare il calendario alla data odierna.
   * Per aggiornare gli incrementi di tempo, seleziona una delle seguenti opzioni dal menu a discesa dell’intervallo di tempo:

      * Mese
1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
   * [Impostazioni](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
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

  Per ulteriori informazioni, vedere la sezione &quot;Aggiungere filtri&quot; nell&#39;articolo [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi.

* Puoi filtrare per campi di ricerca che visualizzano più valori.

### Modificare le impostazioni della vista calendario

La modifica delle impostazioni della vista calendario è identica alla modifica delle impostazioni di una vista timeline.

Per ulteriori informazioni, vedere la sezione &quot;Modificare le impostazioni della visualizzazione della sequenza temporale&quot; nell&#39;articolo [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

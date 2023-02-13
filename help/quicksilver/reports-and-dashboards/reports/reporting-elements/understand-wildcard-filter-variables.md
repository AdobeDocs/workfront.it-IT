---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variabili filtro caratteri jolly
description: Utilizzando i caratteri jolly nei filtri, puoi fare riferimento a un utente o a una data generici invece di un utente o una data specifici. In questo modo, gli elementi generati sono dinamici e i risultati cambiano a seconda del contesto in cui vengono utilizzati.
author: Lisa
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 2%

---

# Variabili filtro caratteri jolly

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Adobe Workfront supporta le variabili di filtro o i caratteri jolly per la creazione dei seguenti elementi:

* Filtri in elenchi, rapporti e planner risorse

   Per informazioni sui filtri Workfront, consulta l’articolo [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Ricerche avanzate

   Per informazioni sulle ricerche avanzate, consulta la sezione . [Usa ricerca avanzata](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) nell&#39;articolo [Ricerca in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* Colonne calcolate nelle visualizzazioni
* Formattazione condizionale nelle visualizzazioni

   Per informazioni sulla formattazione condizionale, consulta l’articolo [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* Campi personalizzati calcolati

   >[!NOTE]
   >
   >Le variabili filtro caratteri jolly non sono supportate quando si fa riferimento a raccolte nidificate in una colonna calcolata.

   Per informazioni sui campi e le colonne personalizzati calcolati, consulta l’articolo [Campi personalizzati calcolati e colonne calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Utilizzando i caratteri jolly, è possibile fare riferimento a un utente o a una data generici anziché a un utente o a una data specifici. In questo modo, gli elementi generati sono dinamici e i risultati cambiano a seconda del contesto in cui vengono utilizzati.

Ad esempio, il filtro per $$USER.homeGroupID in un rapporto di progetto recupera solo i progetti associati al gruppo principale dell&#39;utente che ha effettuato l&#39;accesso.

In Workfront puoi utilizzare variabili di filtro basate su data o basate su utente.

## Variabili del filtro con caratteri jolly basate su data

Le opzioni dei caratteri jolly basati sulla data di Workfront possono essere utilizzate in combinazione con qualsiasi attributo del filtro data.

Per informazioni sull’aggiunta di un carattere jolly basato su data a un rapporto, consulta l’articolo [Utilizzare caratteri jolly basati su data per generalizzare i rapporti](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se si crea un calcolo di data e ora che non include una porzione di ora o che utilizza i caratteri jolly della data $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Coordinated Universal Time), non in base al fuso orario locale. Questo può causare un risultato della data imprevisto.

Scegli tra i seguenti caratteri jolly basati su data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$OGGI</strong> </p> </td> 
   <td> <p>È consigliabile creare filtri sensibili alla data utilizzando questo carattere jolly per evitare di creare nuovamente il filtro domani, la settimana prossima o il mese successivo.</p> <p>Ad esempio, se si desidera visualizzare tutte le attività scadute prima di oggi, è possibile utilizzare la regola seguente in un filtro attività: <em>Data di inizio pianificata inferiore a $$OGGI</em>.</p> <p>$$OGGI è sempre uguale a mezzanotte per il giorno corrente.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>È simile al carattere jolly $$TODAY ma include la data e l'ora correnti. $$NOW è uguale alla data e all'ora correnti.</p> <p>Ad esempio, se desideri visualizzare tutte le voci di ora fornite fino all’ora corrente, puoi farlo utilizzando la seguente regola in un filtro di ora: <em>Data di inizio pianificata inferiore a $$NOW</em>.</p> <p>Nota: Questo carattere jolly non è supportato nel planner risorse.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per indicare diversi periodi di tempo e diversi punti nel tempo (futuri o passati), è possibile combinare i caratteri jolly con i seguenti elementi:

| Attributi |   |
|---|---|
| **q** | trimestre |
| **h** | ora |
| **d** | giorno |
| **w** | settimana |
| **m** | mese |
| **y** | anno |

{style=&quot;table-layout:auto&quot;}

| **Qualificatori** |  |
|---|---|
| **b** | inizio della settimana (domenica) |
| **e** | fine settimana (sabato) |

{style=&quot;table-layout:auto&quot;}

| **Operatori** |  |
|---|---|
| **+** | aggiungi valore al valore jolly |
| **-** | sottrarre valore dal valore jolly |

{style=&quot;table-layout:auto&quot;}

Ad esempio, il carattere jolly `$$TODAYb+2w` si riferisce a &quot;2 settimane dall&#39;inizio di questa settimana&quot;. Il carattere jolly *`$$NOW+2h` si riferisce a &quot;2 ore da ora&quot;.

## Variabili del filtro dei caratteri jolly basate su utente

>[!IMPORTANT]
>
>Se un filtro o un report contiene una variabile di filtro con caratteri jolly basata sull&#39;utente, i risultati mostrano sempre informazioni filtrate dall&#39;utente attualmente connesso. Quando si condivide un filtro o un rapporto di questo tipo con un altro utente, il carattere jolly recupera le informazioni per l&#39;utente che sta visualizzando il rapporto. I due utenti vedono risultati diversi.

Per informazioni sull’aggiunta di un carattere jolly basato su utente a un rapporto, consulta l’articolo [Utilizzare i caratteri jolly basati sull’utente per generalizzare i rapporti](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront fornisce le seguenti variabili basate sull’utente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variabile basata sull'utente più comune è $$USER.ID. Restituisce sempre l'ID dell'utente connesso. Si tratta dell'ID utilizzato per identificare l'utente che ha creato ciascun oggetto e le relative assegnazioni di lavoro.</p> <p>Quando viene utilizzato nei rapporti, questo carattere jolly diminuisce il numero di rapporti che è necessario creare nel sistema. Puoi creare un rapporto e condividerlo con più utenti, e i risultati cambiano in base all’utente che ha effettuato l’accesso e che ha guardato il rapporto.</p> <p>Ad esempio, per creare un rapporto per tutti i problemi assegnati all'utente che ha effettuato l'accesso, puoi utilizzare la seguente regola in un filtro di problemi: <em>Assegnato a ID uguale a $$USER.ID</em>.</p> <p>Workfront utilizza questa variabile nei seguenti filtri incorporati:</p> 
    <ul> 
     <li>I miei report</li> 
     <li>I miei progetti</li> 
     <li>Le mie attività</li> 
     <li>I miei problemi</li> 
     <li>Le Mie Ore</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>La variabile $$USER.categoryID fa riferimento a un modulo personalizzato specifico associato all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>La variabile $$USER.accessLevelID fa riferimento all'ID del livello di accesso associato all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>La variabile $$USER.accessLevelRank fa riferimento al livello di accesso associato all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>La variabile $$USER.companyID fa riferimento alla società associata all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>La variabile $$USER.customerID fa riferimento all'ID dell'account cliente associato all'ambiente. Per l’ambiente, esiste un solo valore possibile per questa variabile e in genere viene utilizzata solo quando si creano integrazioni tramite l’API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>La variabile $$USER.firstName fa riferimento al nome dell'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>La variabile $$USER.lastName fa riferimento al cognome dell'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>La variabile $$USER.name fa riferimento al nome completo dell'utente connesso.</p> <p>Nota:   <p>Questa variabile jolly funziona solo quando si modifica un filtro in modalità testo. Non è possibile utilizzare questo carattere jolly nei filtri che non supportano la modalità testo. Ad esempio, non puoi utilizzare questo carattere jolly nei filtri nelle seguenti aree:</p> 
     <ul> 
      <li> <p>Pianificazione risorse</p> </li> 
      <li> <p>Bilanciamento del carico di lavoro</p> </li> 
      <li> <p>Analisi</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variabile $$USER.homeGroupID fa riferimento all'ID del gruppo principale dell'utente connesso. In qualità di amministratore di gruppo, puoi utilizzare questa variabile per filtrare solo gli elementi che appartengono agli utenti del gruppo home.</p> <p>Ad esempio, per visualizzare tutte le attività incomplete sui progetti nel gruppo finanziario, utilizzare le seguenti regole di filtro in un filtro attività:<br><em>Progetto: ID gruppo uguale a $$USER.homeGroupID </em><br><em>Percentuale completata inferiore a 100</em></p> <p>Per visualizzare tutte le attività incomplete assegnate a singoli utenti di un gruppo specifico che è il Gruppo Home dell'utente connesso, utilizza le seguenti regole di filtro in un filtro attività:</p> <p><em>Assegnato a: ID gruppo uguale a $$USER.homeGroupID<br>Percentuale completata inferiore a 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variabile $$USER.otherGroupIDs fa riferimento a tutti i gruppi (incluso il Gruppo Home) associati al profilo dell'utente connesso.</p> <p>La funzionalità di questa variabile è simile a quella della variabile $$USER.homeGroupID , ad eccezione dei risultati che mostrano informazioni sugli utenti che appartengono a uno qualsiasi dei gruppi associati all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variabile $$USER.homeTeamID fa riferimento all'ID del team principale dell'utente connesso. In qualità di responsabile del team, puoi utilizzare questa variabile per filtrare solo gli elementi che appartengono agli utenti del team principale.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>La variabile $$USER.teamIDs restituisce un elenco di tutti i team associati all'utente connesso.</p> <p>La funzionalità di questa variabile è simile a quella della variabile $$USER.homeTeamID, ad eccezione dei risultati che mostrano informazioni sull'utente che appartiene a uno dei team identificati nel filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variabile $$USER.roleID fa riferimento al ruolo primario dell'utente connesso. Utilizzando questa variabile, è possibile creare rapporti sulle attività o sui problemi assegnati a un ruolo di lavoro specifico.</p> <p>Ad esempio, per visualizzare tutte le attività assegnate al Ruolo primario dell'utente connesso, puoi utilizzare la seguente regola di filtro in un filtro attività:</p> <p><em>Attività: ID ruolo uguale a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>La variabile $$USER.roleIDs fa riferimento a tutti i ruoli di lavoro associati all'utente connesso. Utilizzando questa variabile, puoi creare rapporti sulle attività o sui problemi assegnati a uno qualsiasi dei ruoli di lavoro associati all’utente connesso. </p> <p>Ad esempio, per visualizzare tutte le attività assegnate a uno qualsiasi dei ruoli associati all'utente connesso, puoi utilizzare la seguente regola di filtro in un filtro attività:</p> <p><i>Attività: ID ruolo uguale a $$USERID.roleIDs<br></i> </p> <p>Suggerimento: La <i>Attività: ID ruolo uguale a $$USERID.roleIDs</i> La regola di filtro esiste nei filtri incorporati Attività non assegnate nel ruolo personale e Problemi non assegnati nel ruolo personale. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variabili filtro per caratteri jolly basate su oggetti

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variabile $$OBJCODE fa riferimento al tipo di oggetto. </p> 
     <p>In un modulo personalizzato, quando i tipi di oggetto selezionati del modulo sono incompatibili con un campo a cui si fa riferimento in un campo personalizzato calcolato, è possibile utilizzare questo carattere jolly per evitare la soluzione alternativa alla creazione di moduli duplicati per tali tipi di oggetto.</p> 
     <p>Nel campo personalizzato calcolato, è possibile eseguire questa operazione includendo il carattere jolly in un'espressione IF in modo che il calcolo possa restituire valori diversi per ciascuno dei tipi di oggetto del modulo. </p> 
     <p>Per ulteriori informazioni e un esempio, consulta la sezione . <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Campi personalizzati calcolati nei moduli personalizzati con più oggetti</a> nell'articolo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Aggiungere dati calcolati a un modulo personalizzato</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

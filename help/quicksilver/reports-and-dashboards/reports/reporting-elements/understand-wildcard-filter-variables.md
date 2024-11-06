---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variabili filtro con caratteri jolly
description: Utilizzando i caratteri jolly nei filtri, è possibile fare riferimento a un utente generico o a una data invece di un utente o di una data specifica. In questo modo, gli elementi creati sono dinamici e i risultati cambiano a seconda del contesto in cui vengono utilizzati.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 1%

---

# Panoramica delle variabili filtro con caratteri jolly

<!-- Audited: 11/2024 -->

<!--(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)-->

I caratteri jolly consentono di fare riferimento a un utente o a una data generica anziché a un utente o a una data specifica. In questo modo, gli elementi creati sono dinamici; i risultati cambiano a seconda del contesto in cui vengono utilizzati.

Ad esempio, se si filtra $$USER.homeGroupID in un report di progetti, vengono recuperati solo i progetti associati al Gruppo Predefinito dell&#39;utente connesso.

È possibile utilizzare le variabili di filtro, note anche come caratteri jolly, durante la creazione dei seguenti elementi:

<table>
    <tr>
        <td>Filtri in elenchi, rapporti e Programmazione delle risorse</td>
        <td>Per informazioni sui filtri di Workfront, vedere l'articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Panoramica sui filtri</a>.
</td>
    </tr>
    <tr>
        <td>Ricerche avanzate</td>
        <td>Per informazioni sulle ricerche avanzate, vedere la sezione <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Usa ricerca avanzata</a> nell'articolo <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Cerca in Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Colonne calcolate nelle visualizzazioni</td>
        <td></td>
    </tr>
    <tr>
        <td>Formattazione condizionale nelle visualizzazioni</td>
        <td>Per informazioni sulla formattazione condizionale, vedere l'articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Utilizzare la formattazione condizionale nelle visualizzazioni</a>.
    </tr>
    <tr>
        <td>Campi personalizzati calcolati</td>
        <td>Le variabili di filtro con caratteri jolly non sono supportate quando si fa riferimento a raccolte nidificate in una colonna calcolata.

Per informazioni sui campi e sulle colonne personalizzati calcolati, vedere l&#39;articolo <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Confronto tra campi personalizzati calcolati e colonne calcolate</a>.
</td>
    </tr>
</table>

## Variabili filtro con caratteri jolly basate sulla data

Le opzioni con caratteri jolly basate sulla data possono essere utilizzate in combinazione con qualsiasi attributo del filtro data. Per informazioni sull&#39;aggiunta di un carattere jolly basato sulla data a un report, vedere l&#39;articolo [Utilizzare caratteri jolly basati sulla data per generalizzare i report](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se crei un calcolo di data e ora che non include una porzione di ora o che utilizza i caratteri jolly $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Coordinated Universal Time) e non al fuso orario locale. Questo può causare un risultato di data imprevisto.

Puoi scegliere uno dei seguenti caratteri jolly basati sulla data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$OGGI</strong> </p> </td> 
   <td> <p>È consigliabile creare filtri sensibili alla data utilizzando questo carattere jolly in modo da evitare di creare nuovamente il filtro domani, la prossima settimana o il mese prossimo.</p> <p>Ad esempio, se desideri visualizzare tutte le attività con scadenza precedente a oggi, puoi utilizzare la seguente regola in un filtro attività: <em>Data inizio pianificata inferiore a $$TODAY</em>.</p> <p>$$TODAY è sempre uguale a mezzanotte per il giorno corrente.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>È simile al carattere jolly $$TODAY ma include la data e l'ora correnti. $$NOW corrisponde alla data e all'ora correnti.</p> <p>Ad esempio, se desideri visualizzare tutte le ore inserite fino all'ora corrente, puoi usare la seguente regola nel filtro ore: <em>Data inizio pianificata minore di $$NOW</em>.</p> <p>Nota: questo carattere jolly non è supportato nella pianificazione risorse.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per indicare vari periodi di tempo e vari punti nel tempo (futuri o passati), è possibile combinare i caratteri jolly riportati sopra con i seguenti:

| Attributi |   |
|---|---|
| **q** | trimestre del calendario |
| **h** | ora |
| **d** | giorno |
| **w** | settimana |
| **m** | mese |
| **a** | anno |

{style="table-layout:auto"}

| **Qualificatori** | |
|---|---|
| **b** | inizio del periodo (senza un attributo specificato, per impostazione predefinita inizia la settimana: domenica) |
| **e** | fine periodo (senza un attributo specificato, per impostazione predefinita fine settimana: sabato) |

{style="table-layout:auto"}

| **Operatori** | |
|---|---|
| **+** | aggiungi valore al valore jolly |
| **-** | sottrai valore da valore jolly |

{style="table-layout:auto"}

Ad esempio, il carattere jolly `$$TODAYb+2w` fa riferimento a &quot;2 settimane dall&#39;inizio di questa settimana&quot;. Il carattere jolly *`$$NOW+2h` fa riferimento a &quot;2 ore da ora&quot;.

## Variabili filtro con caratteri jolly basate sull’utente

>[!IMPORTANT]
>
>Se un filtro o un report contiene una variabile di filtro con caratteri jolly basata sull&#39;utente, i risultati mostrano sempre le informazioni filtrate dall&#39;utente attualmente connesso. Quando si condivide un filtro o un report con un altro utente, il carattere jolly recupera le informazioni per l&#39;utente che visualizza il report. I due utenti visualizzano risultati diversi.
>
>Per informazioni sull&#39;aggiunta di un carattere jolly basato sull&#39;utente a un report, vedere l&#39;articolo [Utilizzare caratteri jolly basati sull&#39;utente per generalizzare i report](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Puoi scegliere tra le seguenti variabili basate sull’utente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variabile più comune basata sull'utente è $$USER.ID. In questo modo viene sempre restituito l'ID dell'utente connesso. ID utilizzato per identificare l'utente che ha creato ciascun oggetto e le relative assegnazioni di lavoro.</p> <p>Se utilizzato nei rapporti, questo carattere jolly riduce il numero di rapporti da creare nel sistema. Puoi creare un rapporto e condividerlo con diversi utenti; i risultati cambiano a seconda dell’utente che ha effettuato l’accesso e che osserva il rapporto.</p> <p>Ad esempio, per generare un report per tutti i problemi assegnati all'utente connesso, è possibile utilizzare la seguente regola in un filtro di problemi: <em>Assegnato a ID è uguale a $$USER.ID</em>.</p> <p>Workfront utilizza questa variabile nei seguenti filtri incorporati:</p> 
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
   <td> <p>La variabile $$USER.categoryID fa riferimento a un modulo personalizzato specifico associato all’utente connesso.</p> </td> 
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
   <td> <p>La variabile $$USER.companyID fa riferimento alla società associata all’utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>La variabile $$USER.customerID fa riferimento all’ID dell’account cliente associato al tuo ambiente. Per l’ambiente, esiste un solo valore possibile per questa variabile e in genere viene utilizzata solo durante la creazione di integrazioni tramite l’API.</p> </td> 
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
   <td> <p>La variabile $$USER.name fa riferimento al nome completo dell'utente connesso.</p> <p>Nota:   <p>Questa variabile jolly funziona solo quando si modifica un filtro in modalità testo. Non è possibile utilizzare questo carattere jolly nei filtri che non supportano la modalità testo. Ad esempio, non è possibile utilizzare questo carattere jolly nei filtri nelle seguenti aree:</p> 
     <ul> 
      <li> <p>Pianificazione risorse</p> </li> 
      <li> <p>Bilanciatore dei carichi di lavoro</p> </li> 
      <li> <p>Analisi</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variabile $$USER.homeGroupID fa riferimento all’ID del Gruppo Predefinito dell’utente connesso. In qualità di amministratore di gruppo, puoi utilizzare questa variabile per filtrare solo gli elementi che appartengono agli utenti del gruppo predefinito.</p> <p>Ad esempio, per visualizzare tutte le attività incomplete sui progetti nel gruppo contabilità, utilizzare le seguenti regole di filtro in un filtro attività:<br><em>Progetto: ID gruppo uguale a $$USER.homeGroupID </em><br><em>Percentuale completata inferiore a 100</em></p> <p>Per visualizzare tutte le attività incomplete assegnate a singoli utenti in un gruppo specifico che è il Gruppo Predefinito dell'utente connesso, utilizzare le seguenti regole di filtro in un filtro di attività:</p> <p><em>Assegnato a: ID gruppo uguale a $$USER.homeGroupID<br>Percentuale completata inferiore a 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variabile $$USER.otherGroupIDs fa riferimento a tutti i gruppi (incluso il Gruppo Predefinito) associati al profilo dell’utente connesso.</p> <p>La funzionalità di questa variabile è simile a quella della variabile $$USER.homeGroupID, tranne per il fatto che i risultati visualizzano informazioni sugli utenti che appartengono a uno qualsiasi dei gruppi associati all'utente connesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variabile $$USER.homeTeamID fa riferimento all’ID del team predefinito dell’utente connesso. In qualità di manager del team, puoi utilizzare questa variabile per filtrare solo gli elementi che appartengono agli utenti del team predefinito.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>La variabile $$USER.teamIDs restituisce un elenco di tutti i team associati all'utente connesso.</p> <p>La funzionalità di questa variabile è simile a quella della variabile $$USER.homeTeamID, tranne per il fatto che i risultati visualizzano informazioni sull’utente che appartiene a uno qualsiasi dei team identificati nel filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variabile $$USER.roleID fa riferimento al ruolo primario dell'utente connesso. Utilizzando questa variabile è possibile creare rapporti sulle attività o sui problemi assegnati a una mansione specifica.</p> <p>Ad esempio, per visualizzare tutte le attività assegnate al Ruolo principale dell'utente connesso, è possibile utilizzare la regola di filtro seguente in un filtro attività:</p> <p><em>Attività: ID ruolo uguale a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>La variabile $$USER.roleIDs fa riferimento a tutti i ruoli associati all'utente connesso. Utilizzando questa variabile, è possibile creare rapporti sulle attività o sui problemi assegnati a una qualsiasi mansione associata all'utente connesso. </p> <p>Ad esempio, per visualizzare tutte le attività assegnate a uno qualsiasi dei ruoli associati all'utente connesso, è possibile utilizzare la regola di filtro seguente in un filtro attività:</p> <p><i>Attività: ID ruolo uguale a $$USERID.roleIDs<br></i> </p> <p>Suggerimento: la regola di filtro <i>Attività: ID ruolo è uguale a $$USERID.roleIDs</i> esiste nei filtri incorporati Attività non assegnate nel mio ruolo e Problemi non assegnati nel mio ruolo. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variabili filtro con caratteri jolly basate su oggetti

È possibile scegliere uno dei seguenti caratteri jolly basati su oggetti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variabile $$OBJCODE fa riferimento al tipo di un oggetto. </p> 
     <p>In un modulo personalizzato, quando i tipi di oggetto selezionati del modulo sono incompatibili con un campo a cui si fa riferimento in un campo personalizzato calcolato, è possibile utilizzare questo carattere jolly per evitare la soluzione alternativa di creare moduli duplicati per tali tipi di oggetto.</p> 
     <p>A tale scopo, nel campo personalizzato calcolato includere il carattere jolly in un'espressione IF in modo che il calcolo possa generare valori diversi per ogni tipo di oggetto del modulo. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

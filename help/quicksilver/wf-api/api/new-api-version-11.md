---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 11
description: ReportabileBudgedHour è stato aggiunto all’API di Adobe Workfront come risorsa per il reporting. Contiene campi di riferimento, campi di base e campi predefiniti assenti in BudgetedHour.
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# Novità dell’API versione 11

* [Risorse aggiunte](#added-resources)
* [Risorse rimosse](#removed-resources)
* [Risorse modificate](#modified-resources)

## Risorse aggiunte {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [OrarioA budgetRiportabile](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessor</li> 
     <li style="font-weight: bold;">cliente</li> 
     <li style="font-weight: bold;">user  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">RestricLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OrarioA budgetRiportabile {#reportablebudgetedhour}

ReportabileBudgedHour è stato aggiunto all’API di Adobe Workfront come risorsa per il reporting. Contiene campi di riferimento, campi di base e campi predefiniti assenti in BudgetedHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocateDate </p> <p>La data di allocazione è il primo giorno (una domenica) della settimana per la quale hai preventivato le ore nel Planner risorse.</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>Le ore previste sono ore in cui il budget del gestore risorse per il lavoro che le risorse devono completare sui progetti</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>L'ID Workfront univoco assegnato a un oggetto Reportabile Budgeted Hour specifico.</p> </li> 
     <li style="font-weight: bold;">ScheduledBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>L'ID Workfront univoco assegnato a un progetto specifico.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>L’ID Workfront univoco assegnato a un ruolo di lavoro specifico.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>L'ID Workfront univoco assegnato a un utente specifico.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">progetto</p> <p>Progetto a cui è associato un oggetto ReportabileBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">ruolo</p> <p>Ruolo del lavoro a cui è associato un oggetto ReportabileBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">user</p> <p>Utente a cui è associato un oggetto ReportabileBudgetedHour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operazioni</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">CONTEGGIO</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RAPPORTO </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Risorse rimosse {#removed-resources}

Non sono state rimosse risorse per API v11.

## Risorse modificate {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Approval</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">Percorso approvazione</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">Processo di approvazione</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Assegnazione</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">Attività linea di base</a> </li> 
     <li><a href="#category" class="MCXref xref">Categoria</a> </li> 
     <li><a href="#company" class="MCXref xref">Azienda</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Cliente</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Documento</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iterazione</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Modello di layout</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Nota</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parametro</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programma</a> </li> 
     <li><a href="#project" class="MCXref xref">Progetto</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">Approvazione bozza</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">TempoRiservato</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Rischio</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Attività</a> </li> 
     <li><a href="#team" class="MCXref xref">Team</a> </li> 
     <li><a href="#template" class="MCXref xref">Modello</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">Assegnazione modello</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">AttivitàModello</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Scheda orario</a> </li> 
     <li><a href="#update" class="MCXref xref">Aggiorna</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">NoteUtente</a> </li> 
     <li><a href="#work" class="MCXref xref">Lavoro </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Un oggetto AccessLevelPermissions rappresenta un set di autorizzazioni. Questo insieme di autorizzazioni può quindi essere associato a un livello di accesso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l'autorizzazione di modificare le priorità e le ore di budget nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondarioActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Se un utente non ha accesso a un oggetto in Workfront di cui ha bisogno, può richiedere l&#39;accesso a tale oggetto. L&#39;oggetto AccessRequest rappresenta questa richiesta.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>È stato aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l'autorizzazione di modificare le priorità e le ore di budget nel planner.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un oggetto AccessRule rappresenta un set di regole nei livelli di accesso personalizzati che determina il modo in cui gli utenti possono condividere i progetti creati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l'autorizzazione di modificare le priorità e le ore di budget nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondarioActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approval {#approval}

Un dato elemento di lavoro, ad esempio un&#39;attività, un documento o una scheda attività, può richiedere che un supervisore o un altro utente si disconnetta dall&#39;elemento di lavoro. Un oggetto Approvazione rappresenta l&#39;azione di disconnessione su un elemento di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">I campi seguenti hanno aggiunto gli elementi di convalida AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi validatori specificano che le date sugli oggetti associati non possono essere impostate prima dell'anno 1900 o dopo 2200.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">effectiveStartDate</li>
     <li style="font-weight: bold;">ConstrDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">ScheduledStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti all’API pubblica per la trasparenza nel calcolo dell’EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Noto anche come Valore realizzato, il BCWP (Budgeted Cost of Work Performed) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = percentuale effettiva di completamento x budget attività. Per i progetti, BCWP = SUM (valori BCWP di tutte le attività principali e individuali).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Noto anche come Valore pianificato, il Costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completato al momento del calcolo di questa metrica. Per le attività, BCWS = percentuale di completamento pianificata x budget attività. Per i progetti, BCWS = SUM (valori BCWS di tutte le attività principali e individuali).</p></li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati rimossi dall'oggetto Approvazione.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato aggiunto all'oggetto Approvazione.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Rimosso dall'oggetto Approvazione  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunto all'oggetto Approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Percorso approvazione {#approvalpath}

Un oggetto ApprovedPath è un ramo all&#39;interno di un processo di approvazione. I percorsi di approvazione si basano sullo stato dell&#39;oggetto a cui è associato il processo di approvazione.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Processo di approvazione {#approvalprocess}

Un oggetto ApprovazioneProcesso è un&#39;approvazione in più passaggi che può essere associata a un progetto, un task o un problema.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Assegnazione {#assignment}

Un oggetto di assegnazione rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato per lavorare su di esso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Attività linea di base {#baselinetask}

Le linee di base sono istantanee di come si presentavano le prestazioni di un progetto in un dato momento nel tempo. Archiviano informazioni chiave sul progetto, come date chiave, avanzamento, valori dei costi e dei ricavi. Quando si crea una baseline, le informazioni sull&#39;attività vengono acquisite anche sulle attività della baseline della baseline.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria {#category}

Un oggetto Category è un modulo personalizzato. È possibile creare rapporti per questo oggetto e mostrarli anche in altri rapporti sugli oggetti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Azienda {#company}

Un oggetto Società rappresenta un&#39;organizzazione costituita da una raccolta di persone. Le società sono associate a un utente o a un progetto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">All'oggetto CustomEnum sono state aggiunte le azioni seguenti</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> <p>Le seguenti query sono state aggiunte all'oggetto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente {#customer}

Un oggetto Customer rappresenta un&#39;organizzazione che utilizza un&#39;istanza di Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Sono stati aggiunti i valori possibili: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Condizioni del progetto)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Condizioni attività)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Condizioni del problema)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">Sono state aggiunte le seguenti azioni all’oggetto Cliente</p> 
    <ul> 
     <li style="font-weight: bold;">golEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Un oggetto CustomerPreferences rappresenta il set di preferenze che un cliente ha impostato per la propria istanza di Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Sono stati aggiunti i valori possibili:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.authPolicy (requisiti di complessità della password)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (lunghezza minima password)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (timeout sessione mobile)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (User Time Off)</li> 
       <li style="font-weight: normal;">scheda attività:default.timesheet.manualrole (ruolo di controllo manuale)</li> 
       <li style="font-weight: normal;">bozza:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">bozza:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Documento {#document}

Un oggetto Document rappresenta un file (ad esempio materiale scritto, immagini o altre forme di informazioni).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>All'oggetto Document sono state aggiunte le azioni seguenti.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Iterazione {#iteration}

Un oggetto Iteration rappresenta una singola iterazione Agile. Le iterazioni sono periodi di tempo discreti utilizzati per pianificare e completare storie Agile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti all’oggetto Iteration .</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">punti completati</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modello di layout {#layout-template}

Un oggetto Modello di layout rappresenta una particolare disposizione degli elementi di layout, ad esempio il menu principale, il pannello di navigazione o l’area principale. I modelli di layout possono essere assegnati a utenti, team, gruppi o ruoli di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un modello di layout è impostato per mostrare le marche temporali per le date di scadenza nell’Elenco di lavoro e nel Calendario e false se è impostato per nascondere le marche temporali.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

Un&#39;attività cardine è un indicatore di un&#39;attività che indica che si tratta di un punto chiave del progetto. Generalmente utilizzato per indicare un evento significativo come il completamento di una fase del progetto o di una serie di attività critiche. Un oggetto MilestonePath è un insieme di pietre miliari.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Nota {#note}

Un oggetto Note è un commento o un aggiornamento effettuato su un oggetto Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti all’oggetto Note .</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>like</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un oggetto OpTask è comunemente noto come Problema. Un problema è un elemento di lavoro che in genere indica che c&#39;è un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell&#39;Help Desk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">I campi seguenti hanno aggiunto gli elementi di convalida AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valori specificano che le date sugli oggetti associati non possono essere impostate prima dell’anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">effectiveStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">ScheduledStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti a OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">L'ID Workfront univoco di un oggetto Kanban Board.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">La percentuale di completamento è un parametro che restituisce la quantità completata di un problema, sotto forma di percentuale.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">lavorare  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi Ricerca</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>lavorare</p> <p style="font-weight: normal;">Rimosso</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte all'oggetto OpTask</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parametro {#parameter}

Un oggetto Parameter è un campo personalizzato.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">È stato aggiunto il valore possibile TYAH (Typeahead).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Questo campo è stato aggiunto e fa riferimento al codice oggetto di un oggetto di riferimento. I codici oggetto per tutti gli oggetti si trovano nella <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarle.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrizione</p> <p style="font-weight: normal;">Aggiunta della convalida MAX_LENGTH, che specifica che la lunghezza della descrizione non supera i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programma {#program}

Un oggetto Program è un sottoinsieme all&#39;interno di un portfolio, dove progetti simili possono essere raggruppati insieme.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrizione</p> <p style="font-weight: normal;">Aggiunta della convalida MAX_LENGTH, che specifica che la lunghezza della descrizione non supera i 4000 caratteri.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Aggiunta della convalida MAX_LENGTH, che specifica che la lunghezza del nome non è superiore a 255 caratteri.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Progetto {#project}

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento di base principale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo specifico comune.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">I campi seguenti hanno aggiunto gli elementi di convalida AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valori specificano che le date sugli oggetti associati non possono essere impostate prima dell’anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">effectiveStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">ScheduledStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti all’API pubblica per la trasparenza nel calcolo dell’EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Noto anche come Valore realizzato, il BCWP (Budgeted Cost of Work Performed) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = percentuale effettiva di completamento x budget attività. Per i progetti, BCWP = SUM (valori BCWP di tutte le attività principali e individuali).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Noto anche come Valore pianificato, il Costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completato al momento del calcolo di questa metrica. Per le attività, BCWS = percentuale di completamento pianificata x budget attività. Per i progetti, BCWS = SUM (valori BCWS di tutte le attività principali e individuali).</p></li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato rimosso dall'oggetto Project.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approvazione bozza {#proofapproval}

Un oggetto ProofApproved rappresenta un&#39;approvazione direttamente connessa a una bozza.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se una bozza è in attesa di una decisione e false in caso contrario.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un oggetto QueueDef rappresenta una coda, ovvero un progetto pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare i Problemi ad esso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l'autorizzazione di modificare le priorità e le ore di budget nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### TempoRiservato {#reservedtime}

Un oggetto ReservedTime rappresenta i giorni specificati nell&#39;ora personale di un utente, indicando che l&#39;utente non sarà disponibile per il lavoro.

La risorsa ReservedTime ha aggiunto il flag REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno rimosso il flag NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>Il campo seguente è stato rimosso dall'oggetto ReservedTime.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>attività</p> <p style="font-weight: normal;">Rimosso  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operazioni</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>MODIFICA</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

Un oggetto ResourcePlannerFilter è un insieme di regole che determinano quali elementi verranno visualizzati nel Planner risorse.

La risorsa ResourcePlannerFilter ha aggiunto il flag SHARABLE. Non sono state apportate altre modifiche all&#39;oggetto.

### Rischio {#risk}

Un oggetto Risk rappresenta un possibile evento che può impedire il completamento di un progetto nei tempi stabiliti o entro il budget previsto. Si aggiungono rischi ai progetti nella fase di pianificazione per individuare potenziali ostacoli prima dell&#39;approvazione di qualsiasi lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>Nell’oggetto Rischio sono stati aggiunti i campi seguenti:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enterByID</p> <p style="font-weight: normal;">ID dell’utente che ha creato l’oggetto in origine.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Data in cui un oggetto è stato inviato da un utente in Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Il parametro Data ultimo aggiornamento restituirà la data in cui è stato effettuato l’ultimo aggiornamento a un oggetto,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Ultimo aggiornamento per ID è un parametro che restituisce l’ID utente dell’ultimo utente che ha aggiornato l’oggetto.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> <p style="font-weight: normal;">I seguenti campi di riferimento sono stati aggiunti all'oggetto RIsk.</p> 
    <ul> 
     <li style="font-weight: bold;">enterBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Un oggetto ScheduledReport rappresenta un report configurato per la distribuzione.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Sono stati aggiunti i seguenti valori possibili:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un oggetto ScoreCardQuestion rappresenta una domanda che è stata aggiunta a una scorecard. Queste domande sono solitamente determinate dal gestore del Portfolio e le loro risposte consentono al manager di comprendere quanto un progetto sia in linea con gli obiettivi del portfolio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">È stato aggiunto il valore possibile TYAH (Typeahead)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Attività {#task}

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">I campi seguenti hanno aggiunto gli elementi di convalida AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valori specificano che le date sugli oggetti associati non possono essere impostate prima dell’anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">effectiveStartDate</li>
     <li style="font-weight: bold;">ConstrDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">ScheduledStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti all’API pubblica per la trasparenza nel calcolo dell’EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Noto anche come Valore realizzato, il BCWP (Budgeted Cost of Work Performed) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = percentuale effettiva di completamento x budget attività. Per i progetti, BCWP = SUM (valori BCWP di tutte le attività principali e individuali).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Noto anche come Valore pianificato, il Costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completato al momento del calcolo di questa metrica. Per le attività, BCWS = percentuale di completamento pianificata x budget attività. Per i progetti, BCWS = SUM (valori BCWS di tutte le attività principali e individuali).</p></li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato rimosso dall'oggetto Task.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato aggiunto all’oggetto Task.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Rimosso  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Un oggetto Team è un insieme di utenti che possono essere assegnati a un elemento di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Questo campo è stato aggiunto all'oggetto Team. Tipo di stima dell'altezza determina il modo in cui viene stimato il carico di lavoro di un brano. Se stimato in ore, questo è il numero di ore pianificate aggiunte alla storia. Se stimato in punti, ogni punto aggiungerà al brano un numero di ore pianificate in base a come vengono impostati i punti (il valore predefinito è 8 ore). I valori possibili per Tipo di stima Agile sono:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (punti della storia)</li> 
       <li style="font-weight: normal;">ORE (ore)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (ore come punti)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modello {#template}

Un oggetto Template rappresenta un pattern per un progetto. I progetti possono essere creati da Modelli per risparmiare tempo. Un modello contiene un team e attività, che verranno copiati in un progetto quando viene utilizzato il modello.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di tipo Avanti da allegare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorità</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Assegnazione modello {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AttivitàModello {#templatetask}

Un oggetto TemplateTask rappresenta un oggetto Task che fa parte di un modello. Le attività modello diventano attività nel progetto in cui viene utilizzato il modello.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p style="font-weight: normal;">I campi seguenti hanno aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorità</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Scheda orario {#timesheet}

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Rimosso</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aggiorna {#update}

È possibile aggiornare gli elementi di lavoro in Workfront per informare gli utenti dello stato corrente. Un oggetto Update rappresenta uno di questi aggiornamenti. Gli aggiornamenti possono essere immessi dagli utenti o creati dal sistema Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">È stato aggiunto il valore possibile referenceObjectCustomData (enum.updatetypeenum.referenceoggtcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> <p style="font-weight: normal;">Le seguenti query sono state aggiunte all'oggetto Update.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all’oggetto User .</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteUtente {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all’oggetto User .</p> 
    <ul> 
     <li style="font-weight: bold;">confirmMyNotifications</li> 
     <li style="font-weight: bold;">unknownAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Lavoro  {#work}

Un oggetto Work è un&#39;interfaccia comune ereditata da Task e OpTask e condivide il codice comune tra i due.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">I campi seguenti hanno aggiunto gli elementi di convalida AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valori specificano che le date sugli oggetti associati non possono essere impostate prima dell’anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">effectiveStartDate</li>
     <li style="font-weight: bold;">ConstrDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">ScheduledStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti all’API pubblica per la trasparenza nel calcolo dell’EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Noto anche come Valore realizzato, il BCWP (Budgeted Cost of Work Performed) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = percentuale effettiva di completamento x budget attività. Per i progetti, BCWP = SUM (valori BCWP di tutte le attività principali e individuali).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Noto anche come Valore pianificato, il Costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completato al momento del calcolo di questa metrica. Per le attività, BCWS = percentuale di completamento pianificata x budget attività. Per i progetti, BCWS = SUM (valori BCWS di tutte le attività principali e individuali).</p></li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il possibile valore ET. Questo valore rappresenta l'unità di tempo trascorso mesi, che si riferisce a mesi senza considerare fine settimana o giorni festivi.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato rimosso dall'oggetto Work.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Il campo seguente è stato aggiunto all’oggetto Work.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Rimosso  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

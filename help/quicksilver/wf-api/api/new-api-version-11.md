---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 11 dell’API
description: ReportableBudgedHour è stato aggiunto all’API di Adobe Workfront come risorsa per la generazione di rapporti. Sono disponibili campi di riferimento, campi core e campi predefiniti assenti in OraPreventivata.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# Novità della versione 11 dell’API

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

* [ReportableBudgetedHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">utente  </li> 
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
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
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

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour è stato aggiunto all’API di Adobe Workfront come risorsa per la generazione di rapporti. Sono disponibili campi di riferimento, campi core e campi predefiniti assenti in OraPreventivata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>La data di allocazione è il primo giorno (una domenica) della settimana per cui sono state preventivate le ore nella Programmazione delle risorse.</p> </li> 
     <li> <p style="font-weight: bold;">BudgetedHours </p> <p>Le ore preventivate sono ore preventivate dal responsabile delle risorse per il lavoro che le risorse devono completare nei progetti</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>L'ID Workfront univoco assegnato a uno specifico oggetto Ora preventivata da segnalare.</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>L’ID Workfront univoco assegnato a un progetto specifico.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>ID Workfront univoco assegnato a una mansione specifica.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>L’ID Workfront univoco assegnato a un utente specifico.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">progetto</p> <p>Progetto a cui è associato un oggetto ReportableBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">ruolo</p> <p>Ruolo a cui è associato un oggetto ReportableBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">utente</p> <p>Utente a cui è associato un oggetto ReportableBudgetedHour.</p> </li> 
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
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RAPPORTO </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Risorse rimosse {#removed-resources}

Nessuna risorsa rimossa per API v11.

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
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Assegnazione</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">AttivitàPrevista</a> </li> 
     <li><a href="#category" class="MCXref xref">Categoria</a> </li> 
     <li><a href="#company" class="MCXref xref">Azienda</a> </li> 
     <li><a href="#customenum" class="MCXref xref">EnumPersonalizzata</a> </li> 
     <li><a href="#customer" class="MCXref xref">Cliente</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">PreferenzeCliente</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Documento</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iterazione</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Modello di layout</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">PercorsoMilestone</a> </li> 
     <li><a href="#note" class="MCXref xref">Nota</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parametro</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programma</a> </li> 
     <li><a href="#project" class="MCXref xref">Progetto</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">DefCoda</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
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
     <li><a href="#templateassignment" class="MCXref xref">AssegnazioneModello</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Scheda orario</a> </li> 
     <li><a href="#update" class="MCXref xref">Aggiorna</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">NotaUtente</a> </li> 
     <li><a href="#work" class="MCXref xref">Lavoro </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Un oggetto AccessLevelPermissions rappresenta un insieme di autorizzazioni. Questo set di autorizzazioni può quindi essere associato a un Livello di accesso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l’autorizzazione di modificare le priorità e le ore preventivate nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Se un utente non ha accesso a un oggetto in Workfront di cui ha bisogno, può richiedere l’accesso a tale oggetto. L&#39;oggetto AccessRequest rappresenta questa richiesta.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">azione</p> <p>È stato aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l’autorizzazione di modificare le priorità e le ore preventivate nel planner.  </p> </li> 
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
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l’autorizzazione di modificare le priorità e le ore preventivate nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approval {#approval}

Per un determinato elemento di lavoro, ad esempio un&#39;attività, un documento o una scheda orario, può essere necessario che un supervisore o un altro utente approvi l&#39;elemento di lavoro. Un oggetto Approval rappresenta l&#39;azione di approvazione di un elemento di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">Nei campi seguenti sono stati aggiunti i validatori AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi validatori specificano che le date sugli oggetti associati non possono essere impostate prima del 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">I seguenti campi sono stati aggiunti all’API pubblica per la trasparenza nel calcolo di EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = Percentuale di completamento effettiva x Budget attività. Per i progetti, BCWP = SUM(valori BCWP di tutte le attività padre e di quelle singole).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completata al momento del calcolo di questa metrica. Per le attività, BCWS = Percentuale di completamento pianificata x Budget attività. Per i progetti, BCWS = SUM(valori BCWS di tutte le attività padre e singole).</p></li>
    </ul><p style="font-weight: normal;">Nei campi seguenti è stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati rimossi dall'oggetto Approval.</p>
    <ul>
     <li style="font-weight: bold;">reservTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato aggiunto all'oggetto Approval.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservTime</p> <p style="font-weight: normal;">Rimosso dall’oggetto Approval  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Aggiunto all'oggetto Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Un oggetto ApprovalPath è un ramo di un processo di approvazione. I percorsi di approvazione si basano sullo stato dell&#39;oggetto a cui è associato il processo di approvazione.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Un oggetto ApprovalProcess è un&#39;approvazione in più passaggi che può essere associata a un progetto, un&#39;attività o un problema.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
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

Un oggetto assegnazione rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato a lavorarci.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AttivitàPrevista {#baselinetask}

Le linee di base sono istantanee delle prestazioni di un progetto in un determinato momento. Memorizzano informazioni chiave sul progetto, come date chiave, avanzamento, costi e ricavi. Quando si crea una previsione, le informazioni sulle attività vengono acquisite anche sulle attività previste della previsione.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria {#category}

Un oggetto Category è un modulo personalizzato. È possibile creare report per questo oggetto e visualizzarlo anche in altri report oggetto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
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

Un oggetto Company rappresenta un&#39;organizzazione costituita da un insieme di persone. Le aziende sono associate a un utente o a un progetto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
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

### EnumPersonalizzata {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all'oggetto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> <p>Le query seguenti sono state aggiunte all'oggetto CustomEnum</p> 
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
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Sono stati aggiunti i possibili valori: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Condizioni progetto)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Condizioni attività)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (condizioni problema)  </li> 
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
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all'oggetto Customer</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### PreferenzeCliente {#customerpreferences}

Un oggetto CustomerPreferences rappresenta l&#39;insieme di preferenze impostate da un cliente per l&#39;istanza di Workfront.

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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Sono stati aggiunti i possibili valori:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Password Complexity Requirements)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Lunghezza minima password)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (timeout sessione mobile)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (Indisponibilità utente)</li> 
       <li style="font-weight: normal;">scheda orario:default.timesheet.manualrole (ruolo di controllo manuale)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proof.defaultnonRecipientRole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proof.defaultnonrecipientguestrole)  </li> 
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

Un oggetto Document rappresenta un file, ad esempio materiale scritto, immagini o altre forme di informazioni.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte all'oggetto Document.</p> 
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

Un oggetto Iteration rappresenta una singola iterazione Agile. Le iterazioni sono periodi di tempo distinti utilizzati per pianificare e completare le storie di Agile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti all'oggetto Iteration.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">punti completati</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modello di layout {#layout-template}

Un oggetto modello di layout rappresenta una particolare disposizione di elementi layout, ad esempio il menu principale, il pannello di navigazione o l&#39;area Home. I modelli di layout possono essere assegnati a utenti, team, gruppi o mansioni.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con il valore true se un modello di layout è impostato per mostrare i timestamp per le date di scadenza nell’elenco di lavoro e nel calendario e false se è impostato per nascondere i timestamp.  </p> </li> 
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

### PercorsoMilestone {#milestonepath}

Una milestone è un indicatore di un&#39;attività che indica che si tratta di un punto chiave nel progetto. Generalmente utilizzato per indicare un evento significativo, ad esempio il completamento di una fase del progetto o di una serie di attività critiche. Un oggetto MilestonePath è un insieme di milestone.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
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
   <td> <p>I campi seguenti sono stati aggiunti all'oggetto Note.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>piace</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un oggetto OpTask è comunemente noto come Issue. Un problema è un elemento di lavoro che in genere indica la presenza di un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell’helpdesk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">Nei campi seguenti sono stati aggiunti i validatori AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valdator specificano che le date sugli oggetti associati non possono essere impostate prima dell'anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">I campi seguenti sono stati aggiunti a OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">ID Workfront univoco di un oggetto Kanban Board.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">La percentuale di completamento è un parametro che restituisce l’importo completato di un’emissione, come percentuale.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">lavoro  </li>
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
     <li style="font-weight: bold;"> <p>lavoro</p> <p style="font-weight: normal;">Rimosso</p> </li> 
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
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore TYAH (automatico).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Questo campo è stato aggiunto e fa riferimento al codice oggetto di un oggetto di riferimento. I codici oggetto per tutti gli oggetti si trovano nel <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarli.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrizione</p> <p style="font-weight: normal;">È stata aggiunta la convalida MAX_LENGTH che specifica che la lunghezza della descrizione non deve superare i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programma {#program}

Un oggetto Program è un sottoinsieme all&#39;interno di un portfolio, in cui è possibile raggruppare progetti simili.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descrizione</p> <p style="font-weight: normal;">È stata aggiunta la convalida MAX_LENGTH che specifica che la lunghezza della descrizione non deve superare i 4000 caratteri.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">È stata aggiunta la convalida MAX_LENGTH che specifica che la lunghezza del nome non deve superare i 255 caratteri.  </p> </li> 
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

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento fondamentale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo comune specifico.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">Nei campi seguenti sono stati aggiunti i validatori AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valdator specificano che le date sugli oggetti associati non possono essere impostate prima dell'anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">I seguenti campi sono stati aggiunti all’API pubblica per la trasparenza nel calcolo di EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = Percentuale di completamento effettiva x Budget attività. Per i progetti, BCWP = SUM(valori BCWP di tutte le attività padre e di quelle singole).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completata al momento del calcolo di questa metrica. Per le attività, BCWS = Percentuale di completamento pianificata x Budget attività. Per i progetti, BCWS = SUM(valori BCWS di tutte le attività padre e singole).</p></li>
    </ul><p style="font-weight: normal;">I campi seguenti hanno aggiunto il flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato rimosso dall'oggetto Project.</p>
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

### ProofApproval {#proofapproval}

Un oggetto ProofApproval rappresenta un&#39;approvazione direttamente connessa a una bozza.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano che ha il valore true se una bozza è in attesa di una decisione e false in caso contrario.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DefCoda {#queuedef}

Un oggetto QueueDef rappresenta una coda, ovvero un progetto che è stato pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare i problemi.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti hanno aggiunto il possibile valore BUDGETING_INFORMATION. Questo consente agli utenti con l’autorizzazione di modificare le priorità e le ore preventivate nel planner.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

Un oggetto ReservedTime rappresenta i giorni specificati nell&#39;Ora personale di un utente, a indicare che l&#39;utente non sarà disponibile per il lavoro.

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
    </ul> <p>Il seguente campo è stato rimosso dall'oggetto ReservedTime.</p> 
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

Un oggetto ResourcePlannerFilter è un insieme di regole che determinano gli elementi da visualizzare nella Programmazione delle risorse.

La risorsa ResourcePlannerFilter ha aggiunto il flag SHARABLE. Non sono state apportate altre modifiche all&#39;oggetto.

### Rischio {#risk}

Un oggetto Rischio rappresenta un possibile evento che può impedire il completamento di un progetto in tempo o entro i limiti del budget. I progetti in fase di pianificazione presentano rischi aggiuntivi per individuare potenziali ostacoli prima dell’approvazione di qualsiasi lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti all'oggetto Risk:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">ID dell'utente che ha creato l'oggetto.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Data in cui un oggetto è stato inviato da un utente in Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Il parametro Last Update Date restituisce la data in cui è stato effettuato l'ultimo aggiornamento di un oggetto.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID è un parametro che restituirà l'ID utente dell'ultimo utente che ha aggiornato l'oggetto.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> <p style="font-weight: normal;">I campi di riferimento seguenti sono stati aggiunti all'oggetto RIsk.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Un oggetto ScheduledReport rappresenta un report configurato per la consegna.

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

Un oggetto ScoreCardQuestion rappresenta una domanda aggiunta a una scorecard. Queste domande sono solitamente determinate dal manager del Portfolio e le loro risposte consentono al manager di capire quanto un progetto sia in linea con gli obiettivi del portfolio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore TYAH (automatico)  </p> </li> 
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
   <td colspan="2">Campi diretti<p style="font-weight: normal;">Nei campi seguenti sono stati aggiunti i validatori AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valdator specificano che le date sugli oggetti associati non possono essere impostate prima dell'anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">I seguenti campi sono stati aggiunti all’API pubblica per la trasparenza nel calcolo di EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = Percentuale di completamento effettiva x Budget attività. Per i progetti, BCWP = SUM(valori BCWP di tutte le attività padre e di quelle singole).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completata al momento del calcolo di questa metrica. Per le attività, BCWS = Percentuale di completamento pianificata x Budget attività. Per i progetti, BCWS = SUM(valori BCWS di tutte le attività padre e singole).</p></li>
    </ul><p style="font-weight: normal;">Nei campi seguenti è stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato rimosso dall'oggetto Task.</p>
    <ul>
     <li style="font-weight: bold;">reservTimeID</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato aggiunto all'oggetto Task.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservTime</p> <p style="font-weight: normal;">Rimosso  </p> </li> 
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

Un oggetto Team è un insieme di Utenti che possono essere assegnati a un elemento di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Questo campo è stato aggiunto all'oggetto Team. Il tipo di stima agile determina come viene stimato il carico di lavoro di una storia. Se stimato in ore, si tratta del numero di ore pianificate che vengono aggiunte alla storia. Se stimato in punti, ogni punto aggiungerà un numero di ore pianificate alla storia in base a come vengono impostati i punti (il valore predefinito è 8 ore). I valori possibili per il tipo di stima Agile sono:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (Punti storia)</li> 
       <li style="font-weight: normal;">ORE (ore)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (ore come punti)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modello {#template}

Un oggetto Template rappresenta un pattern per un progetto. I progetti possono essere creati dai modelli per risparmiare tempo. Un modello contiene un team e delle attività, che verranno copiate in un progetto quando viene utilizzato il modello.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Questo campo è stato aggiunto ed è un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
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

### AssegnazioneModello {#templateassignment}

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
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un oggetto TemplateTask rappresenta un oggetto Task che fa parte di un oggetto Template. Le Attività Modello diventano Attività nel Progetto in cui viene utilizzato il Modello.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p style="font-weight: normal;">Nei campi seguenti è stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi raccolta</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Scheda orario {#timesheet}

Un oggetto Timesheet rappresenta un foglio ore virtuale che consente agli utenti di immettere le ore effettivamente lavorate per le attività, i progetti e i tipi di ore di lavoro comune.

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
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Query</td> 
   <td> <p style="font-weight: normal;">Le query seguenti sono state aggiunte all'oggetto Update.</p> 
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
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all'oggetto User.</p> 
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

### NotaUtente {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Azioni</td> 
   <td> <p style="font-weight: normal;">Le azioni seguenti sono state aggiunte all'oggetto User.</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount  </li> 
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

Un oggetto Work è un&#39;interfaccia comune ereditata sia da Task che da OpTask e condivide il codice comune tra i due.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campi diretti<p style="font-weight: normal;">Nei campi seguenti sono stati aggiunti i validatori AT_DATE_BEFORE_YEAR e AT_DATE_AFTER_YEAR. Questi valdator specificano che le date sugli oggetti associati non possono essere impostate prima dell'anno 1900 o dopo il 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">I seguenti campi sono stati aggiunti all’API pubblica per la trasparenza nel calcolo di EAC (Stima al completamento).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività effettivamente completata al momento del calcolo di questa metrica. Per le attività, BCWP = Percentuale di completamento effettiva x Budget attività. Per i progetti, BCWP = SUM(valori BCWP di tutte le attività padre e di quelle singole).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta il costo preventivato dell'importo dell'attività che avrebbe dovuto essere completata al momento del calcolo di questa metrica. Per le attività, BCWS = Percentuale di completamento pianificata x Budget attività. Per i progetti, BCWS = SUM(valori BCWS di tutte le attività padre e singole).</p></li>
    </ul><p style="font-weight: normal;">Nei campi seguenti è stato aggiunto il possibile valore ET. Questo valore rappresenta l’unità di tempo Mesi trascorsi, che si riferisce ai mesi indipendentemente dai fine settimana o dalle festività.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato rimosso dall'oggetto Lavoro.</p>
    <ul>
     <li style="font-weight: bold;">reservTimeID</li>
    </ul><p style="font-weight: normal;">Il seguente campo è stato aggiunto all'oggetto Work.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservTime</p> <p style="font-weight: normal;">Rimosso  </p> </li> 
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

---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 13 dell’API
description: Adobe Workfront ha rilasciato la versione API 13 il 22 aprile 2021. La versione 13 dell’API presenta le seguenti modifiche rispetto alla versione 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 2%

---

# Novità della versione 13 dell’API

Adobe Workfront ha rilasciato la versione API 13 il 22 aprile 2021. La versione 13 dell’API presenta le seguenti modifiche rispetto alla versione 12.

## Risorse aggiunte

Non sono state aggiunte risorse per API versione 13.

## Risorse rimosse

Nessuna risorsa rimossa per API versione 13.

## Risorse modificate

Le seguenti risorse sono state modificate per API versione 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">Livello di accesso</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">PreferenzeCliente</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">VersioneDocumento</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Gruppo </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">VoceDiario</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">ModelloLayout</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">CartellaCollegata</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">AttivitàOperativa</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Progetto</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ApprovazioneBozza</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">DefCoda</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Attività</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Scheda orario</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">ModelloUIT</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">DelegaUtente</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Lavoro </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LivelloAccesso {#accesslevel}

Un oggetto AccessLevel è associato agli utenti e descrive il set di autorizzazioni AccessLevelPermissions che determinano gli elementi a cui l&#39;utente può accedere.

Per ulteriori informazioni sui livelli di accesso, vedere [Funzionamento dei livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrizione</b> </p> <p>È stata aggiunta la convalida MAX_LENGTH che specifica che la lunghezza della descrizione non deve superare i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Un oggetto BreadCrumb rappresenta un elemento nella gerarchia padre/figlio di un elemento di lavoro di Workfront. Le breadcrumb indicano in che modo un elemento di lavoro si inserisce nella struttura più ampia di Portfoli, progetti, progetti e attività.

Per ulteriori informazioni sulle breadcrumb, consulta [Panoramica delle breadcrumb nella nuova esperienza Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>I codici oggetto si trovano in <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Un oggetto BurndownEvent rappresenta un oggetto che modifica il bundown di un&#39;iterazione.

Per ulteriori informazioni sul burndown, vedi [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> <p>I campi seguenti hanno rimosso il flag NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### PreferenzeCliente {#customerpreferences}

Un oggetto CustomerPreferences rappresenta l&#39;insieme di preferenze impostate da un cliente per l&#39;istanza di Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Sono stati aggiunti i possibili valori:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">scheda orario:default.timesheet.restrictions.timesheet.edit.owners.admins (config.timesheet.restricted.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte alla risorsa CustomerPreferences.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Accetta l’argomento:</p> 
      <ul> 
       <li> <p>preferenze (mappa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Un oggetto DocumentVersion rappresenta una versione specifica di un file, ad esempio materiale scritto, immagini o altre forme di informazioni.

Per ulteriori informazioni sulle versioni dei documenti, vedere [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valore possibile aggiunto:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Flag aggiunto NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppo  {#group}

Un oggetto Group rappresenta un insieme di utenti e team. I gruppi spesso rappresentano la struttura di reparto.

Per ulteriori informazioni sui gruppi, vedi [Gruppi e team in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Azioni</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Questa azione restituisce una matrice dei gruppi padre del gruppo (gruppi di cui il gruppo specificato è un sottogruppo).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### VoceDiario {#journalentry}

L&#39;oggetto JournalEntry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Voce diario, viene creata una voce corrispondente ogni volta che tale campo viene modificato.

La risorsa JournalEntry ha aggiunto il flag REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> <p>I campi seguenti hanno rimosso il flag NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>dataVoce</b> </p> </li> 
     <li> <p><b>nomeCampo</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>I campi seguenti hanno aggiunto il flag NOT_FILTERABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Gli amministratori di Adobe Workfront o di gruppi possono creare modelli per personalizzare gli elementi di layout in Adobe Workfront. L&#39;oggetto LayoutTemplate è specifico di Adobe Workfront Classic.

Per l&#39;oggetto che rappresenta i modelli di layout nella nuova esperienza Adobe Workfront, vedi [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrizione</b> </p> <p>È stata aggiunta la convalida MAX_LENGTH che specifica che la lunghezza della descrizione non deve superare i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un oggetto LinkedFolder rappresenta una cartella collegata da un provider di documenti esterno, ad esempio Google Drive o Dropbox.

Per ulteriori informazioni sulle cartelle collegate, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valore possibile aggiunto:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Campi Ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>preferitiDaUtentiMM</b> </p> </li> 
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
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Campi diretti</p> </td> 
   <td> <p>I campi seguenti sono stati aggiunti alla risorsa ProofApproval.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DataDecisione</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DefCoda {#queuedef}

Un oggetto QueueDef rappresenta una coda, ovvero un progetto che è stato pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare i problemi.

Per ulteriori informazioni sulle code di richieste, vedere [Creare una coda di richieste](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Aggiunto. I valori possibili sono:</p> 
      <ul> 
       <li> <p>0 (dopo i moduli personalizzati)</p> </li> 
       <li> <p>1 (prima dei moduli personalizzati)</p> </li> 
      </ul> </li> 
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
   <td> <p>Campi Ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>preferitiDaUtentiMM</b> </p> </li> 
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

### Scheda orario {#timesheet}

Un oggetto Timesheet rappresenta un foglio ore virtuale che consente agli utenti di immettere le ore effettivamente lavorate per le attività, i progetti e i tipi di ore di lavoro comune.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi core</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Rimosso</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Un oggetto Timesheet rappresenta un foglio ore virtuale che consente agli utenti di immettere le ore effettivamente lavorate per le attività, i progetti e i tipi di ore di lavoro comune.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi predefiniti</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Gli amministratori di Adobe Workfront o di gruppi possono creare modelli per personalizzare gli elementi di layout in Adobe Workfront. L’oggetto UITemplate è specifico per la nuova esperienza Adobe Workfront.

Per l&#39;oggetto che rappresenta i modelli di layout in Adobe Workfront Classic, vedere [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte alla risorsa UITemplate.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Accetta l’argomento:</p> 
      <ul> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Considera gli argomenti:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DelegaUtente {#userdelegation}

Un oggetto UserDelegation rappresenta l&#39;atto di delegare il lavoro da un utente a un altro per un periodo di tempo specifico.

L&#39;oggetto UserDelegation ha aggiunto il flag REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> <p>I campi seguenti hanno rimosso il flag NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>dataInizio</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi predefiniti</td> 
   <td> <p>Sono stati aggiunti i seguenti campi:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>dataInizio</b> </p> </li> 
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
   <td> <p>Campi Ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>preferitiDaUtentiMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

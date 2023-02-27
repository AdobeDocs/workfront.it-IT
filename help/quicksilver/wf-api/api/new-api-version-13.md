---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 13
description: Adobe Workfront ha rilasciato l’API versione 13 il 22 aprile 2021. La versione 13 dell’API presenta le seguenti modifiche rispetto alla versione 12.
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Novità dell’API versione 13

Adobe Workfront ha rilasciato l’API versione 13 il 22 aprile 2021. La versione 13 dell’API presenta le seguenti modifiche rispetto alla versione 12.

## Risorse aggiunte

Non sono state aggiunte risorse per l’API versione 13.

## Risorse rimosse

Non sono state rimosse risorse per l’API versione 13.

## Risorse modificate

Le risorse seguenti sono state modificate per l’API versione 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">LivelloAccesso</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Gruppo </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Progetto</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">Approvazione bozza</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Attività</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Scheda orario</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">Profilo scheda attività</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">Modello UIT</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelega</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Lavoro </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LivelloAccesso {#accesslevel}

Un oggetto AccessLevel è associato agli utenti e descrive il set di AccessLevelPermissions che determinano a cosa può accedere l&#39;utente.

Per ulteriori informazioni sui livelli di accesso, vedi [Funzionamento dei livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrizione</b> </p> <p>Aggiunta della convalida MAX_LENGTH, che specifica che la lunghezza della descrizione non supera i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Un oggetto BreadCrumb rappresenta un elemento nella gerarchia padre/figlio di un elemento di lavoro Workfront. Le breadcrumb indicano come un elemento di lavoro si adatta alla struttura più ampia di Portfoli, progetti, progetti e attività.

Per ulteriori informazioni sulle breadcrumb, consulta [Panoramica delle breadcrumb nella nuova esperienza Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>I codici oggetto si trovano nella <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Un oggetto BurndownEvent rappresenta un oggetto che modifica il raggruppamento di un&#39;iterazione.

Per ulteriori informazioni sul menu a discesa, vedi [Burn](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

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

### CustomerPreferences {#customerpreferences}

Un oggetto CustomerPreferences rappresenta il set di preferenze che un cliente ha impostato per la propria istanza di Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Sono stati aggiunti i valori possibili:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">scheda attività:default.timesheet.limit.timesheet.edit.owner.admins (config.timesheet.limit.timesheet.edit.Owner.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte alla risorsa CustomerPreferences .</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Accetta l'argomento seguente:</p> 
      <ul> 
       <li> <p>preferenze (mappa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Un oggetto DocumentVersion rappresenta una versione specifica di un file (ad esempio materiale scritto, immagini o altre forme di informazione).

Per ulteriori informazioni sulle versioni dei documenti, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>È stato aggiunto il flag NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppo  {#group}

Un oggetto Group rappresenta un set di utenti e team. I gruppi rappresentano spesso la struttura dipartimentale.

Per ulteriori informazioni sui gruppi, consulta [Gruppi e team in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Azioni</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getGenents</b> </p> <p>Questa azione restituisce una matrice dei gruppi principali del gruppo (gruppi di cui il gruppo specificato è un sottogruppo).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

È possibile impostare l&#39;oggetto JournalEntry per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Journal Entry, ogni volta che tale campo viene modificato viene creata una voce Journal corrispondente.

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
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
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

Gli amministratori di Adobe Workfront o gli amministratori di gruppo possono creare modelli per personalizzare gli elementi di layout in Adobe Workfront. L&#39;oggetto LayoutTemplate è specifico di Adobe Workfront Classic.

Per l&#39;oggetto che rappresenta i modelli di layout nella nuova esperienza Adobe Workfront, vedi [Modello UIT](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrizione</b> </p> <p>Aggiunta della convalida MAX_LENGTH, che specifica che la lunghezza della descrizione non supera i 4000 caratteri.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un oggetto LinkedFolder rappresenta una cartella collegata da un provider di documenti esterno, ad esempio Google Drive o Dropbox.

Per ulteriori informazioni sulle cartelle collegate, consulta [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Campi Ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoriteByUsersMM</b> </p> </li> 
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
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Campi diretti</p> </td> 
   <td> <p>I campi seguenti sono stati aggiunti alla risorsa ProofApprovazione .</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DataDecisione</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un oggetto QueueDef rappresenta una coda, ovvero un progetto pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare i Problemi ad esso.

Per ulteriori informazioni sulle code di richiesta, vedi [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Aggiunta completata. I valori possibili sono:</p> 
      <ul> 
       <li> <p>0 (dopo i moduli personalizzati)</p> </li> 
       <li> <p>1 (Prima dei moduli personalizzati)</p> </li> 
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
     <li> <p><b>favoriteByUsersMM</b> </p> </li> 
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

### Scheda orario {#timesheet}

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

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

### Profilo scheda attività {#timesheetprofile}

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

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

### Modello UIT {#uitemplate}

Gli amministratori di Adobe Workfront o gli amministratori di gruppo possono creare modelli per personalizzare gli elementi di layout in Adobe Workfront. L&#39;oggetto LayoutTemplate è specifico per la nuova esperienza Adobe Workfront.

Per l&#39;oggetto che rappresenta i modelli di layout in Adobe Workfront Classic, consultare [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> <p>Le azioni seguenti sono state aggiunte alla risorsa UITemplate .</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Accetta l'argomento seguente:</p> 
      <ul> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Accetta gli argomenti seguenti:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelega {#userdelegation}

Un oggetto UserDelegate rappresenta l&#39;atto di delegare il lavoro da un utente a un altro per un periodo di tempo specifico.

L&#39;oggetto UserDelega ha aggiunto il flag REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> <p>I campi seguenti hanno rimosso il flag NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi predefiniti</td> 
   <td> <p>Sono stati aggiunti i campi seguenti:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>Campi Ricerca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoriteByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

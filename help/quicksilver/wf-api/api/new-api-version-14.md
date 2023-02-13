---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 14
description: Adobe Workfront ha rilasciato l’API versione 14 il 9 settembre 2021. La versione 14 dell’API presenta le seguenti modifiche rispetto alla versione 14.
author: John
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# Novità dell’API versione 14

Adobe Workfront ha rilasciato l’API versione 14 il 9 settembre 2021. La versione 14 dell’API presenta le seguenti modifiche rispetto alla versione 14.

## Risorse aggiunte

Non sono state aggiunte risorse per l’API versione 14.

## Risorse rimosse

Non sono state rimosse risorse per l’API versione 14.

## Risorse modificate

Le risorse seguenti sono state modificate per l’API versione 14.

* [BillingRecord (BILL)](#billingrecord-bill)
* [Categoria (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Cliente (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Gruppo (GRUPPO)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Progetto (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Allocazione risorse (RSALLO)](#resource-allocation-rsallo)
* [Ruolo (RUOLO)](#role-role)
* [Modello (TMPL)](#template-tmpl)
* [Scheda attività (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

Un oggetto BillingRecord registra i ricavi, le ore o le spese che è possibile fatturare. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.

Per ulteriori informazioni sui record di fatturazione, vedi [Creazione di record di fatturazione](../../manage-work/projects/project-finances/create-billing-records.md).

L&#39;oggetto BillingRecord ha aggiunto il flag **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Aggiunta completata. Una categoria è un modulo personalizzato. Questo parametro è stato aggiunto per supportare la possibilità di aggiungere Forms personalizzati agli oggetti BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi di riferimento</td> 
   <td> 
    <ul> 
     <li> <p><b>categoria</b> </p> <p>Aggiunta completata. Una categoria è un modulo personalizzato. Questo parametro è stato aggiunto per supportare la possibilità di aggiungere moduli personalizzati agli oggetti BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi raccolta</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Aggiunta completata. Rappresenta un insieme di Categorie (moduli personalizzati) associate all'oggetto BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Aggiunta completata. Questa azione ricalcola le espressioni nei campi modulo personalizzati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria (CTGY) {#category-ctgy}

Un oggetto Category è un modulo personalizzato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Questo valore è stato aggiunto per supportare la possibilità di aggiungere moduli personalizzati agli oggetti BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovedStatus</b> </p> <p>Questa azione prende i parametri objID e objCode e restituisce un valore booleano.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

L&#39;oggetto CustomEnum consente la conversione dei codici di stato in testo leggibile dall&#39;utente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Query</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Aggiunta completata. Questa query supporta la possibilità di creare e gestire gli stati per gruppi e sottogruppi. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Gestire gli stati dei gruppi</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente (CUST) {#customer-cust}

Un oggetto Customer rappresenta un&#39;organizzazione che utilizza un&#39;istanza di Workfront.

Si tratta di un oggetto interno.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Un oggetto CustomerPreferences rappresenta il set di preferenze che un cliente ha impostato per la propria istanza di Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p>Consenti agli utenti di aggiungere immagini negli aggiornamenti (aggiornamenti:images.toggle)</p> </li> 
      </ul> <p>Questo parametro supporta la possibilità di aggiungere immagini agli aggiornamenti degli elementi di lavoro. </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Un oggetto DocumentVersion rappresenta una versione specifica di un file (ad esempio materiale scritto, immagini o altre forme di informazione).

Per ulteriori informazioni sulle versioni dei documenti, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Aggiunta completata. Questo campo registra la data e l’ora dell’ultimo callback da Workfront Proof, se la versione è associata a una bozza.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppo (GRUPPO) {#group-group}

Un oggetto Group rappresenta un set di utenti e team. I gruppi rappresentano spesso la struttura dipartimentale.

Per ulteriori informazioni sui gruppi, consulta [Gruppi e team in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Aggiunta completata. Questa azione prende una matrice di groupIDs e li aggiunge come sottogruppi al gruppo specificato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Un oggetto NoteTag rappresenta l&#39;atto di assegnare tag a un utente o a un team in un aggiornamento a un elemento di lavoro.

Per ulteriori informazioni sull’assegnazione tag negli aggiornamenti, consulta [Assegnare tag agli altri utenti in caso di aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operazioni</td> 
   <td> <p>Le seguenti operazioni sono state aggiunte all'oggetto NoteTag :</p> 
    <ul> 
     <li> <p><b>CONTEGGIO</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RAPPORTO</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Progetto (PROJ) {#project-proj}

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento di base principale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo specifico comune.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Aggiunta completata.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Un oggetto QueueDef rappresenta una coda, ovvero un progetto pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare problemi a tale area.

Per ulteriori informazioni sulle code di richiesta, vedi [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Aggiunta completata. Questa azione supporta la possibilità di trovare le richieste utilizzando il percorso attraverso la coda delle richieste e i gruppi di argomenti.</p> <p>Per ulteriori informazioni sulla ricerca delle code di richiesta per percorso, vedi <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Creare richieste e generare bozze nell’app web Workfront</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Creare e inviare richieste Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Allocazione risorse (RSALLO) {#resource-allocation-rsallo}

Un oggetto Assegnazione risorse rappresenta la stima delle risorse necessarie per un determinato progetto. Questo oggetto viene utilizzato solo nel Planner risorse legacy. Per il campo corrispondente nel nuovo planner risorse, utilizzare l&#39;ora a budget (BGHR).

L&#39;oggetto Assegnazione risorse ha rimosso il flag **SEGNALABILE**.

### Ruolo (RUOLO) {#role-role}

Un oggetto Role (job role) rappresenta una capacità funzionale o un set di competenze che un utente potrebbe riempire, ad esempio Designer o Product Manager.

Per informazioni sui ruoli di lavoro, consulta [Panoramica sul ruolo del lavoro](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata. Si tratta di un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi predefiniti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modello (TMPL) {#template-tmpl}

Un oggetto Template rappresenta un pattern per un progetto. I progetti possono essere creati da modelli per risparmiare tempo. Un modello contiene un team e attività, che verranno copiati in qualsiasi progetto creato dal modello.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Aggiunta completata. Questo campo è stato aggiunto per supportare la capacità di associare gruppi a modelli.</p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modificare i modelli di progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gruppo</p> <p style="font-weight: normal;">Aggiunta completata. Questo campo è stato aggiunto per supportare la capacità di associare gruppi a modelli.</p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modificare i modelli di progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->

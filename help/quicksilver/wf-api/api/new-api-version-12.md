---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 12
description: Workfront ha rilasciato la versione 12 dell’API il 12 novembre 2020. La versione 12 dell’API presenta le seguenti modifiche rispetto alla versione 11
author: Becky
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# Novità dell’API versione 12

Workfront ha rilasciato la versione 12 dell’API il 12 novembre 2020. La versione 12 dell’API presenta le seguenti modifiche rispetto alla versione 11

## Risorse aggiunte

Le seguenti risorse sono nuove nella versione 12 dell’API Workfront.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Un oggetto BreadCrumb rappresenta un elemento nella gerarchia padre/figlio di un elemento di lavoro Adobe Workfront. Le breadcrumb indicano come un elemento di lavoro si adatta alla struttura più ampia di Portfoli, progetti, progetti e attività.

Per ulteriori informazioni sulle Breadcrumb in Workfront, vedi [Panoramica delle breadcrumb nella nuova esperienza Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Azione</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

I campi RTF sono ora disponibili per più oggetti. L&#39;oggetto RichTextParameterValue è stato aggiunto a Workfront per supportare questa disponibilità.

Per ulteriori informazioni, consulta [Campi di testo RTF nell’API di Adobe Workfront](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Risorse rimosse

Non sono state rimosse risorse per l’API versione 12.

## Risorse modificate

Le seguenti risorse sono state modificate per l’API Workfront versione 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">LivelloAccesso</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnuncioAllegato</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Approval</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Azienda</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Cliente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Documento</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Gruppo </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parametro</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programma</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Attività</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">AttivitàModello</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Scheda orario</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Utente</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Lavoro </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### LivelloAccesso {#accesslevel}

Un oggetto AccessLevel è associato agli utenti e descrive il set di AccessLevelPermissions che determinano a cosa può accedere l&#39;utente.

Per ulteriori informazioni sui livelli di accesso, vedi [Funzionamento dei livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Un oggetto AccessLevelPermissions rappresenta un&#39;autorizzazione specifica per accedere, creare o modificare un oggetto Workfront. Tali autorizzazioni possono quindi essere associate a un livello di accesso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiornare le ore pianificate nel servizio di bilanciamento del carico di lavoro.</p> <p>Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aggiorna le ore pianificate dell'attività durante la gestione delle allocazioni degli utenti</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiungere campi ai moduli personalizzati.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un utente con un livello di accesso che include questa autorizzazione può condividere un campo personalizzato a livello di sistema con l'accesso Elimina.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per campi e widget personalizzati</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondarioActions</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">action</p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiornare le ore pianificate nel servizio di bilanciamento del carico di lavoro.</p> <p>Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aggiorna le ore pianificate dell'attività durante la gestione delle allocazioni degli utenti</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiungere campi ai moduli personalizzati.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un utente con un livello di accesso che include questa autorizzazione può condividere un campo personalizzato a livello di sistema con l'accesso Elimina.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per campi e widget personalizzati</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiornare le ore pianificate nel servizio di bilanciamento del carico di lavoro.</p> <p>Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aggiorna le ore pianificate dell'attività durante la gestione delle allocazioni degli utenti</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiungere campi ai moduli personalizzati.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un utente con un livello di accesso che include questa autorizzazione può condividere un campo personalizzato a livello di sistema con l'accesso Elimina.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per campi e widget personalizzati</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondarioActions</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Un oggetto ActivityLog è un elenco completo di tutte le attività che hanno avuto luogo in un dato account di prova Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operazioni</p> </td> 
   <td> <p>L'operazione seguente è stata rimossa dall'oggetto ActivityLog:</p> 
    <ul> 
     <li> <p><strong>AGGIUNGI</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnuncioAllegato {#announcementattachment}

Un oggetto AnnouncementAttachment rappresenta un file allegato a un annuncio Workfront.

Per ulteriori informazioni sugli allegati dell&#39;annuncio, vedi [Inviare annunci](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Sono stati aggiunti i valori possibili:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Sono stati rimossi i seguenti flag:</p> 
      <ul> 
       <li> <p>DINAMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Sono stati aggiunti i seguenti flag</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINAMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workFfort</strong> </p> <p>Questo campo è stato aggiunto e indica se un utente deve compiere un piccolo, medio o grande sforzo giornaliero per completare un'attività. I valori possibili sono:</p> 
      <ul> 
       <li> <p>1 (piccolo)</p> </li> 
       <li> <p>2 (medio)</p> </li> 
       <li> <p>3 (grande)</p> </li> 
      </ul> <p>Per ulteriori informazioni sullo sforzo di lavoro in Workfront, vedi <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

Una sezione Calendario è un rapporto sul calendario.

Per ulteriori informazioni sui rapporti sul calendario, vedi [Panoramica dei rapporti sul calendario](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> <p style="font-weight: normal;">I campi seguenti sono stati aggiunti all'oggetto CalendarSection per supportare la nuova funzionalità di utilizzo di date personalizzate nei report calendario. </p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Utilizzare campi data personalizzati in un rapporto calendario</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Azienda {#company}

Un oggetto Società rappresenta un&#39;organizzazione costituita da una raccolta di persone.

Per ulteriori informazioni sulle aziende, vedi [Creare e modificare aziende](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID del gruppo a cui è associata la società.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gruppo</p> <p style="font-weight: normal;">Gruppo a cui è associata l'azienda. L'associazione di una società a un gruppo consente all'amministratore del gruppo di estendere l'accesso e le autorizzazioni del gruppo all'azienda.</p> </li> 
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
  <tr> 
   <td>Azioni</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Questa azione utilizza un argomento CustomerProductTypeEnum e restituisce un valore booleano che indica se il cliente dispone di un account per quel prodotto. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (abilita l'integrazione dello zoom nel flusso degli aggiornamenti)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Aggiunta completata</p> </li> 
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
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">È stato rimosso il valore possibile:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> <p>All'oggetto Document sono state aggiunte le azioni seguenti.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Questa azione prende l'argomento documentVersonID (stringa) e restituisce una mappa che indica la decisione del revisore.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Questa azione utilizza i seguenti argomenti:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (stringa)</p> </li> 
       <li> <p>revisoreDecision (stringa)</p> </li> 
       <li> <p>commento (stringa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppo  {#group}

Un oggetto Group rappresenta un set di utenti e team. I gruppi rappresentano spesso la struttura dipartimentale.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">ID del Business Leader assegnato al gruppo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">Il Business Leader assegnato al gruppo. Un Business Leader è qualcuno che prende decisioni commerciali per il gruppo.</p> <p style="font-weight: normal;">Per ulteriori informazioni sugli imprenditori, consulta <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Panoramica di Business Leader</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Azioni</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Questa azione utilizza i seguenti argomenti:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (stringa)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Questa azione utilizza i seguenti argomenti:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removeMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">È stato rimosso il valore possibile:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un oggetto OpTask è comunemente noto come Problema. Un problema è un elemento di lavoro che in genere indica che c&#39;è un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell&#39;Help Desk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Campi diretti</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>L'ordine indica la posizione di un'attività o di un brano nel backlog Agile.</p> <p>Questo campo ha rimosso i seguenti flag:
       <ul>
        <li>DINAMICO,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> <p>Queste azioni hanno aggiunto lo stato dell'argomento per supportare la nuova funzionalità del pulsante Start, che cambia lo stato di un elemento di lavoro quando un utente fa clic sul pulsante per indicare che ha iniziato a lavorare sull'elemento.</p> <p>Per ulteriori informazioni, consulta <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parametro {#parameter}

Un oggetto Parameter è un campo personalizzato.

La risorsa Parameter ha aggiunto il flag SHARABLE.

Per ulteriori informazioni sui campi personalizzati, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p>RICH (Rich Text)</p> <p>Per ulteriori informazioni, consulta <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campi di testo RTF nell’API di Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>È stato aggiunto il valore possibile:</p> 
      <ul> 
       <li> <p>RICH (campo di testo con formattazione)</p> <p>Per ulteriori informazioni, consulta <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campi di testo RTF nell’API di Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>etichetta</strong> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi raccolta</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi predefiniti</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>etichetta</strong> </p> <p>Aggiunta completata</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarle.

Per ulteriori informazioni sui portfolio, vedi [Panoramica del Portfolio in Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID del gruppo a cui è associato il portfolio.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gruppo</p> <p style="font-weight: normal;">Gruppo a cui è associato il portafoglio. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programma {#program}

Un oggetto Program è un sottoinsieme di progetti all&#39;interno di un portfolio, dove progetti simili possono essere raggruppati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID del gruppo a cui è associato il programma.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campi di riferimento</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gruppo</p> <p style="font-weight: normal;">Gruppo a cui è associato il programma. </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiornare le ore pianificate nel servizio di bilanciamento del carico di lavoro.</p> <p>Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aggiorna le ore pianificate dell'attività durante la gestione delle allocazioni degli utenti</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utente con un livello di accesso che include questa autorizzazione può aggiungere campi ai moduli personalizzati.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un utente con un livello di accesso che include questa autorizzazione può condividere un campo personalizzato a livello di sistema con l'accesso Elimina.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per campi e widget personalizzati</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>Sono stati aggiunti i seguenti possibiliValori:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Un oggetto ScheduledReport rappresenta un report configurato per la distribuzione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Sono stati aggiunti i valori possibili:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un oggetto ScoreCardQuestion rappresenta una domanda che è stata aggiunta a una scorecard. Queste domande sono solitamente determinate dal gestore del Portfolio e le loro risposte consentono al manager di comprendere quanto un progetto sia in linea con gli obiettivi del portfolio.

Per ulteriori informazioni sulle domande della scorecard, vedi [Creare una scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">È stato aggiunto il possibile valore RICH (Campo di testo con formattazione) </p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campi di testo RTF nell’API di Adobe Workfront</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Attività {#task}

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>workFfort</strong> </p> <p>Questo campo è stato aggiunto e indica se un utente deve compiere un piccolo, medio o grande sforzo giornaliero per completare un'attività. I valori possibili sono:</p> 
      <ul> 
       <li> <p>1 (piccolo)</p> </li> 
       <li> <p>2 (medio)</p> </li> 
       <li> <p>3 (grande)</p> </li> 
      </ul> <p>Per ulteriori informazioni sullo sforzo di lavoro in Workfront, vedi <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> <p>Queste azioni hanno aggiunto lo stato dell'argomento per supportare la nuova funzionalità del pulsante Start, che cambia lo stato di un elemento di lavoro quando un utente fa clic sul pulsante per indicare che ha iniziato a lavorare sull'elemento.</p> <p>Per ulteriori informazioni, consulta <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Un oggetto Team è un insieme di utenti che possono essere assegnati a un elemento di lavoro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti alla risorsa Team:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Questo campo rappresenta il numero di giorni in cui una scheda completata rimane sulla bacheca Kanban.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Questo campo associa un team a un gruppo. Questo identifica il team come parte del gruppo e consente all’amministratore del gruppo di gestire i team.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Questo è un parametro booleano che indica se il pulsante Work on It del team è stato configurato come pulsante Start. Quando un membro del team fa clic su un pulsante Start per iniziare a lavorare su un elemento di lavoro, lo stato dell'elemento cambia da Nuovo a uno stato configurato nelle impostazioni del team.</p> </li> 
     <li> <p>I campi seguenti consentono di specificare gli stati personalizzati per il pulsante Start sui singoli elementi di lavoro.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Per ulteriori informazioni sul pulsante Start, vedi <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campi di riferimento</td> 
   <td> <p>Il campo seguente è stato aggiunto alla risorsa Team:</p> 
    <ul> 
     <li> <p><strong>gruppo</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AttivitàModello {#templatetask}

Un oggetto TemplateTask rappresenta un oggetto Task che fa parte di un modello. Le attività modello diventano attività nel progetto in cui viene utilizzato il modello.

Per ulteriori informazioni sulle attività dei modelli, consulta [Modificare un’attività modello](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>workFfort</strong> </p> <p>Questo campo è stato aggiunto e indica se un utente deve compiere un piccolo, medio o grande sforzo giornaliero per completare un'attività. I valori possibili sono:</p> 
      <ul> 
       <li> <p>1 (piccolo)</p> </li> 
       <li> <p>2 (medio)</p> </li> 
       <li> <p>3 (grande)</p> </li> 
      </ul> <p>Per ulteriori informazioni sullo sforzo di lavoro in Workfront, vedi <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Scheda orario {#timesheet}

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

Per ulteriori informazioni sui fogli presenze, consulta [Panoramica sui fogli presenze](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi core</td> 
   <td> <p>Il campo seguente è stato rimosso dalla risorsa Scheda attività:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aggiorna

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Sono stati aggiunti i seguenti valori possibili:</p> 
      <ul> 
       <li> <p>InitiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>InitiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Per ulteriori informazioni sulle iniziative, vedi <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative nel planner dello scenario</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Utente {#user}

Un oggetto User rappresenta una persona con un account in Workfront in grado di accedere e interagire con il sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campi diretti</td> 
   <td> <p>I campi seguenti sono stati aggiunti alla risorsa Utente :</p> 
    <ul> 
     <li> <p><strong>effectiveDeactivationDate</strong> </p> <p>Rappresenta la data e l’ora in cui un utente è stato disattivato.</p> <p>Per ulteriori informazioni sugli utenti disattivati, consulta <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>Questo campo mostra l’accesso dell’utente agli obiettivi di Workfront. I valori possibili sono:</p> 
      <ul> 
       <li> <p>Nessun accesso</p> </li> 
       <li> <p>Viste</p> </li> 
       <li> <p>Modif</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni</td> 
   <td> <p>È stata aggiunta la seguente azione alla risorsa Utente:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Questa azione prende i seguenti argomenti</p> 
      <ul> 
       <li> <p>id (stringa)</p> </li> 
       <li> <p>objCode (stringa)</p> </li> 
      </ul> </li> 
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
   <td>Campi diretti</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>L'ordine indica la posizione di un'attività o di un brano nel backlog Agile.</p> <p>Questo campo ha rimosso i seguenti flag:</p> 
      <ul> 
       <li> <p>DINAMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Questo campo ha aggiunto i seguenti flag:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINAMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workFfort</strong> </p> <p>Questo campo è stato aggiunto e indica se un utente deve compiere un piccolo, medio o grande sforzo giornaliero per completare un'attività. I valori possibili sono:</p> 
      <ul> 
       <li> <p>1 (piccolo)</p> </li> 
       <li> <p>2 (medio)</p> </li> 
       <li> <p>3 (grande)</p> </li> 
      </ul> <p>Per ulteriori informazioni sullo sforzo di lavoro in Workfront, vedi <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>

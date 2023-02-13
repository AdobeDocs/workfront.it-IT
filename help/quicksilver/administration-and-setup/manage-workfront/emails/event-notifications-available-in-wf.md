---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Notifiche di eventi disponibili in Adobe Workfront
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti quali progetti, attività e problemi, come spiegato nelle notifiche degli eventi.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '5070'
ht-degree: 27%

---

# Notifiche di eventi disponibili in Adobe Workfront

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti quali progetti, attività e problemi, come spiegato in [Notifiche degli eventi](../../../workfront-basics/using-notifications/event-notifications.md).

Queste notifiche possono essere configurate a livello di sistema e di gruppo:

* Per informazioni sulla configurazione delle notifiche degli eventi a livello di sistema, vedi [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Per informazioni sulla configurazione delle notifiche degli eventi a livello di gruppo, consulta [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

I singoli utenti possono inoltre attivare e disattivare le notifiche dei singoli eventi nel loro profilo individuale. Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Nelle tabelle seguenti sono elencate tutte le notifiche dell’evento Adobe Workfront, una breve descrizione dell’evento e se l’evento è attivo o inattivo per impostazione predefinita.

## Azione richiesta

Vedi anche [Notifiche: Azioni necessarie](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th>Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Richiesta di accesso all'utente</p> </td> 
   <td> <p>Qualcuno ha richiesto a me l'accesso.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Aggiunta di richiesta documento al richiedente</p> </td> 
   <td> <p>Richiedi di caricare i documenti.</p> <p>Il richiedente del documento riceve una notifica e-mail quando riceve una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento in attesa di approvazione per gli approvatori</p> </td> 
   <td> <p>Devo approvare un documento.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue al nuovo incaricato</p> </td> 
   <td> <p>Quando si cambia l'incaricato di una Issue, invia una Email al nuovo incaricato.</p> <p>L’assegnatario del problema riceve una notifica e-mail solo se lo stato del progetto è Corrente e lo stato del problema non è Chiuso o se è simile a Chiuso.</p> <p>Gli utenti con una licenza di revisione o richiesta non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un problema.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dall’abilitazione dell’impostazione "Approvatore non richiesto per il team di progetto (per i processi di approvazione che includono un ruolo)" (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il ruolo di Approvatore .</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di approvatore ricevono una notifica e-mail.</p> <p>Viene inviata una notifica se il progetto si trova nello stato Pianificazione o Corrente. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione dell'approvatore delegato</p> </td> 
   <td> <p>Devo rivedere un'approvazione del problema che mi è stata delegata.</p> <p>Quando un utente delega un'approvazione di un problema a un altro utente, viene inviata una notifica. </p> <p>Una notifica viene inviata solo quando il progetto è nello stato Corrente.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un progetto.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dall’abilitazione dell’impostazione "Approvatore non richiesto per il team di progetto (per i processi di approvazione che includono un ruolo di lavoro)" (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>).</p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il ruolo di Approvatore .</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di approvatore ricevono una notifica e-mail.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Progetto in attesa di approvazione dell'approvatore delegato</td> 
   <td> <p>Devo rivedere l'approvazione di un progetto per il quale ho una delega.</p> </td> 
   <td> Attivi</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso d'Incarico Attività al Nuovo Incaricato</p> </td> 
   <td> <p>Quando viene cambiato l'incaricato primario di un'attività, invia una Email al nuovo incaricato.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail se viene assegnato l'assegnatario principale dell'attività, a meno che l'assegnatario non sia l'utente che ha effettuato l'assegnazione.</p> <p>Viene inviata una notifica se lo stato del progetto è Corrente e l’attività non è contrassegnata Completa.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un'attività.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dall’abilitazione dell’impostazione "Approvatore non richiesto per il team di progetto (per i processi di approvazione che includono un ruolo)" (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il ruolo di Approvatore .</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di approvatore ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current al momento della richiesta.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione dell'approvatore delegato</p> </td> 
   <td> <p>Devo rivedere l'approvazione di un'attività per la quale ho una delega.</p> <p>Quando un utente delega un'approvazione di un problema a un altro utente, viene inviata una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Current al momento della richiesta.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Scheda orario riaperta a utente</p> </td> 
   <td> <p>La mia scheda orario è stata riaperta.</p> <p>Il proprietario della scheda attività riceve una notifica e-mail quando la scheda attività viene riaperta, a meno che l'utente che ha riaperto la scheda attività non sia anche il proprietario della scheda attività.</p> <p>Viene inviata una notifica e-mail solo se lo stato della scheda attività è Aperto.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Invia per Email l'Avviso del Timesheet Respinto all'Utente</p> </td> 
   <td> <p>Quando si rispinge un Timesheet, invia una Email all'utente.</p> <p>Il proprietario della scheda attività riceve una notifica e-mail quando la scheda attività viene rifiutata, a meno che l'utente che ha rifiutato la scheda attività non sia anche il proprietario.</p> <p>Viene inviata una notifica e-mail solo se lo stato della scheda attività viene rifiutato.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Invia per Email l'Avviso della Presentazione del Timesheet all'Autorizzatore</p> </td> 
   <td> <p>Quando si presenta un Timesheet, invia una Email all'Autorizzatore.</p> <p>L'approvatore della scheda attività riceve una notifica e-mail quando viene inviata una scheda attività che deve approvare, a meno che l'utente che ha inviato la scheda attività non sia anche l'approvatore della scheda attività.</p> <p>Viene inviata una notifica solo se viene inviato lo stato della scheda attività.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro al team</p> </td> 
   <td> <p>Il mio team riceve una nuova richiesta di lavoro.</p> <p>I membri del team ricevono una notifica e-mail quando il team riceve una nuova richiesta di lavoro. (L’utente che ha inviato la richiesta non riceve una notifica se è membro del team.)</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente al momento della richiesta di lavoro e lo stato della richiesta di lavoro è Nuovo.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro ad Assegnatario elemento di lavoro</p> </td> 
   <td> <p>Ricevo una nuova richiesta di lavoro.</p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail, a meno che l’utente che effettua la richiesta non sia anche l’assegnatario. </p> <p>Non viene inviata alcuna notifica se lo stato dell’attività è Completo o se lo stato del problema è Chiuso.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current al momento della richiesta.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
 </tbody> 
</table>

## Richieste che ho presentato

Vedi anche [Notifiche: Richieste che ho presentato](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Modifica stato approvazione documento al richiedente</p> </td> 
   <td> <p>Completata una richiesta di approvazione documento.</p> <p>Il richiedente del documento riceve una notifica e-mail al completamento della richiesta di approvazione del documento.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Completamento di richiesta documento al richiedente</p> </td> 
   <td> <p>Richiesta di caricamento documento completata.</p> <p>Il richiedente del documento riceve una notifica e-mail quando viene soddisfatta una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso del Issue all'Autore della Issue</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email all'autore.</p> <p>Il contatto principale su un problema riceve una notifica quando aggiunge un problema in un progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Assegnazione problema al contatto principale del problema</td> 
   <td> <p>Qualcuno è assegnato a un problema per il quale sono il contatto principale.</p> <p>Il contatto principale su un problema riceve una notifica quando il problema viene assegnato a un utente. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue Completa all'autore</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email all'autore.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso del Cambio Stato Progetto all'utente che ha inserito il progetto</p> </td> 
   <td> <p>Quando si cambia lo stato del progetto, invia una Email all'utente che ha inserito il progetto.</p> <p>L’utente che ha creato il progetto riceve una notifica e-mail quando cambia lo stato del progetto.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta richiesta al contatto principale del problema</p> </td> 
   <td> <p>Invio una richiesta (conferma).</p> <p>Il contatto principale sul problema riceve una notifica e-mail quando invia un problema.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current e se il progetto utilizza una visualizzazione "Is Help Desk".</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione richiesta al contatto principale del problema</p> </td> 
   <td> <p>Qualcuno è assegnato alla mia richiesta.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un utente viene assegnato al problema, a meno che il contatto principale e l’utente assegnato siano lo stesso utente.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current e se il progetto utilizza una visualizzazione "Is Help Desk".</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Richiesta chiusa al contatto principale del problema</p> </td> 
   <td> <p>La mia richiesta è chiusa (conferma).</p> <p>Il contatto principale del problema riceve una notifica e-mail quando la richiesta viene chiusa.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current e se il progetto utilizza una visualizzazione "Is Help Desk".</p> <p>Se le notifiche per "completamento problemi" sono abilitate, verranno sempre attivate al posto di "Richiesta chiusa al contatto principale di emissione". Se desideri che questa notifica venga attivata, devi disattivare le notifiche di completamento del problema.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento richiesta al contatto principale del problema</p> </td> 
   <td> <p>Documento modificato o caricato su un problema per il quale sono il contatto principale.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un documento viene caricato o modificato sul problema, a meno che l'utente che ha caricato o modificato il documento non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e se nella scheda Configurazione coda è abilitata l’opzione "Pubblica come coda della richiesta di aiuto". &lt;!— DISEGNATO IN FLARE: Per ulteriori informazioni sulla pubblicazione di un progetto come coda di richiesta della Guida, consulta 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Panoramica della scheda Dettagli coda in un progetto</a>.

    —>&lt;/p> &lt;/td>
<td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica stato richiesta al contatto principale del problema</p> </td> 
   <td> <p>Le modifiche di stato cambia su mia richiesta.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando lo stato del problema cambia, a meno che l’utente che ha modificato lo stato non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e il progetto utilizza una visualizzazione "Is Help Desk".</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
 </tbody> 
</table>

## Comunicazione

Vedi anche [Notifiche: Comunicazione](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Commento al proprietario del documento</p> </td> 
   <td> <p>È stato aggiunto un commento sul mio documento.</p> <p>Il proprietario di un documento in Workfront riceve una notifica e-mail quando un commento viene pubblicato sul documento, a meno che l'utente che ha pubblicato il commento non sia anche il proprietario del documento.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current. </p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Commento su &lt;request name=""&gt; su &lt;project name=""&gt; (rif.# &lt;request reference="" number=""&gt;)</em></p> <p> Oggetto della notifica giornaliera del riassunto:<em> Digest of Communication &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Attivi </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Aggiunta nota richiesta al contatto principale del problema</p> </td> 
   <td> <p>Quando un commento viene pubblicato su una richiesta, invia un'e-mail al contatto principale del problema.</p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta, a meno che l'utente che ha pubblicato il commento non sia anche il contatto principale per il problema.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td>Aggiornamento diretto all'utente</td> 
   <td> <p>Qualcuno mi include in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag agli altri utenti in caso di aggiornamenti</a>.</p> <p>In questo caso, l’utente incluso nell’aggiornamento diretto riceve una notifica e-mail sull’aggiornamento.</p> <p>La notifica e-mail viene inviata solo se l’utente dispone dei diritti di accesso all’oggetto&lt;!&gt;— DISEGNATO IN FLARE: e non è lo stesso utente che inserisce l'aggiornamento

    -->. &lt;/p> &lt;p>Questa notifica di evento è attivata per impostazione predefinita e non può essere disattivata.&lt;/p> &lt;/td>
<td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Aggiornamento diretto al team</p> </td> 
   <td> <p>Qualcuno include il mio team in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag agli altri utenti in caso di aggiornamenti</a>.</p> <p>In questo caso, qualsiasi membro del team incluso nell'aggiornamento diretto riceve una notifica e-mail sull'aggiornamento.</p> <p>La notifica e-mail viene inviata solo agli utenti che hanno diritti di accesso all’oggetto dell’aggiornamento.</p> <p>Se l’utente che invia l’aggiornamento diretto è membro del team incluso, l’utente che invia l’aggiornamento non riceve una notifica e-mail.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento elemento lavoro a Partecipanti argomento</p> </td> 
   <td> <p>Qualcuno ha commentato su un argomento che mi interessa.</p> <p>I partecipanti al thread e gli utenti inclusi in un messaggio diretto ricevono una notifica e-mail quando un utente fa un commento nel thread.</p> <p>Per ricevere una notifica, gli utenti devono disporre dell’accesso Visualizza .</p> <p>I seguenti utenti non ricevono una notifica:</p> 
    <ul> 
     <li> <p>Team inclusi in un messaggio diretto</p> </li> 
     <li> <p>Proprietario della nota</p> </li> 
     <li> <p>Contatto principale</p> </li> 
    </ul> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento sull'elemento di lavoro ad assegnatario elemento di lavoro</p> </td> 
   <td> <p>Qualcuno ha commentato uno degli elementi del mio lavoro.</p> <p>L'assegnatario dell'elemento di lavoro riceve una notifica e-mail ogni volta che un utente aggiunge un aggiornamento a un elemento di lavoro, a meno che l'utente che aggiunge l'aggiornamento non sia anche l'assegnatario.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Risposta alla richiesta di lavoro a Richiedente lavoro</p> </td> 
   <td> <p>Qualcuno ha risposto alla mia richiesta.</p> <p>Dopo che un utente invia una richiesta e un altro utente risponde a tale richiesta, l’utente che ha inviato la richiesta riceve una notifica e-mail.</p> <p>Una notifica e-mail non viene inviata se:</p> 
    <ul> 
     <li> <p>L’utente che risponde è lo stesso utente che ha effettuato la richiesta</p> </li> 
     <li> <p>L'utente non ha accesso per visualizzare la nota</p> </li> 
    </ul> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni di omologazione

Vedi anche [Notifiche: Informazioni di omologazione](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Delega dell'approvazione a un altro utente</p> </td> 
   <td> <p>Sono delegato come approvatore.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica dello stato di approvazione del problema delegato</p> </td> 
   <td> <p>Una richiesta di approvazione del problema delegata è stata completata. </p> <p>Quando deleghi un’approvazione di un problema a un altro utente, riceverai una notifica e-mail al termine dell’approvazione (che approvi o rifiuti l’approvazione del problema). </p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica dello stato di approvazione del progetto delegata</p> </td> 
   <td> <p>Una richiesta di approvazione del progetto delegata è stata completata.</p> <p>Quando deleghi un’approvazione di un progetto a un altro utente, riceverai una notifica e-mail al termine dell’approvazione (che approvi o rifiuti l’approvazione del progetto).</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica dello stato di approvazione dell'attività delegata</p> </td> 
   <td> <p>Lo stato di approvazione di un'attività delegata è stato completato.</p> <p>Quando si delega un'approvazione di un'attività a un altro utente, viene inviata una notifica e-mail al termine dell'approvazione (che approvi o rifiuti l'approvazione dell'attività).</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento approvazione documento all'approvatore</p> </td> 
   <td> <p>Annullata una richiesta di approvazione documento.</p> <p>L'approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Approvazione Timesheet all'Utente</p> </td> 
   <td> <p>Quando si approva e si chiude un Timesheet, invia una Email all'utente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sul lavoro assegnato

Vedi anche [Notifiche: Informazioni sul lavoro assegnato](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Attività</td> 
   <td>Il completamento di tutte le attività predecessore ad attività dipendenti sul team assegnato</td> 
   <td> <p>Tutti i predecessori dei compiti del team sono completati.</p> <p>Gli assegnatari dell’attività (tutti i membri del team) ricevono una notifica e-mail.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td>Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Il completamento di tutte le Attività Predecessore ad Attività Dipendenti</p> </td> 
   <td> <p>Quando sono completate tutte le attività predecessori, invia una Email a tutti i principali utenti incaricati alle attività dipendenti.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisione di approvazione da rilasciare assegnata a</p> </td> 
   <td> <p>Un problema che io risolvo è approvato o rifiutato.</p> <p>L’assegnatario di un problema riceve una notifica e-mail quando viene presa una decisione di approvazione (approvata o rifiutata).</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Decisione di approvazione all'attività assegnata a</p> </td> 
   <td> <p>Quando viene approvata o respinta un'Attività che va approvata, invia una Email all'incaricato.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail quando l'attività viene approvata o rifiutata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue Completa all'Incaricato</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email all'incaricato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Data di completamento problema pianificata cambiata</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un problema al quale sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando cambia la data di completamento pianificata, a meno che l’utente che ha modificato la data di completamento pianificata non sia anche l’assegnatario.</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da Planning.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica stato del problema a Problema assegnato a</p> </td> 
   <td> <p>Le modifiche dello stato su uno degli elementi del mio lavoro.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando lo stato cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento richiesta a Problema assegnato a</p> </td> 
   <td> <p>I documenti vengono caricati o modificati sulle richieste alle quali sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando i documenti vengono caricati o modificati su un problema aggiunto.</p> <p>Non viene inviata una notifica e-mail se l’utente che ha inserito il problema è l’assegnatario del problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e se nella scheda Configurazione coda è abilitata l’opzione "Pubblica come coda della richiesta di aiuto".&lt;!— DISEGNATO IN FLARE: Per ulteriori informazioni sulla pubblicazione di un progetto come coda di richiesta della Guida, consulta 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Panoramica della scheda Dettagli coda in un progetto</a>.

    —>&lt;/p> &lt;/td>
<td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Attività Completata all'Incaricato</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email all'incaricato.</p> <p>Al completamento dell’attività, l’Assegnatario dell’attività riceve una notifica e-mail. Le notifiche non vengono inviate quando un’attività personale viene completata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>Gli utenti con una licenza Revisore o Richiedente non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Attività Completata ad Incaricati delle Attività dipendenti</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email a tutti gli incaricati di attività dipendenti.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando uno dei predecessori dell’attività è stato completato.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Data di completamento attività pianificata modificata</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un'attività a cui sono assegnato.</p> <p>L'Assegnatario dell'attività riceve una notifica e-mail quando cambia la data di completamento pianificata dell'attività, a meno che l'utente che ha modificato la data di completamento pianificata non sia anche l'Assegnatario dell'attività.</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da Planning.</p> <p>Non viene inviata alcuna notifica relativa alle attività personali.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica stato dell'attività a Attività assegnata a</p> </td> 
   <td> <p>Le modifiche stato su un'attività a cui sono assegnato.</p> <p>L'Assegnatario dell'attività riceve una notifica e-mail quando lo stato dell'attività cambia, a meno che l'utente che ha modificato lo stato non sia anche l'assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui progetti su cui mi trovo

Vedi anche [Notifiche: Informazioni sui progetti su cui mi trovo](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso di Stato Attuale alla Squadra</p> </td> 
   <td> <p>Quando si cambia lo stato del progetto da Idea/Approvato/Richiesta/Pianificazione ad Attuale, invia una Email alla squadra.</p> <p>Gli utenti del progetto ricevono una notifica e-mail quando il progetto diventa attivo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Invia per Email l'Avviso del Documento alla Squadra di Progetto</p> </td> 
   <td> <p>Un documento viene aggiunto a un progetto su cui mi trovo.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando un documento viene aggiunto al progetto, fatta eccezione per l’utente che ha aggiunto il documento.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue alla Squadra del Progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email alla squadra.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue Completa alla squadra</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email alla squadra.</p> <p>Ogni utente del progetto riceve una notifica.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'attività principale alla squadra progetto</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email alla squadra.</p> <p>Tutti gli utenti del team di progetto ricevono una notifica al completamento di un'attività cardine. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso del Progetto Completato alla squadra</p> </td> 
   <td> <p>Quando si completa un progetto, invia una Email alla squadra.</p> <p>Gli utenti di un team di progetto ricevono una notifica e-mail al completamento dello stato del progetto.</p> <p>Suggerimento: Se i progetti vengono completati regolarmente, l’abilitazione di questa opzione consente di creare un sacco di e-mail per gli utenti che hanno un numero limitato di attività su molti progetti. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso del Cambio Stato Progetto alla squadra</p> </td> 
   <td> <p>Quando si cambia lo stato del progetto, invia una Email alla squadra.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando cambia lo stato del progetto. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso della aggiunta Utente, all'Utente</p> </td> 
   <td> <p>Quando si aggiunge un utente alla squadra di progetto, invia una Email all'utente.</p> <p>L’utente aggiunto al progetto riceve una notifica e-mail quando viene aggiunto, a meno che l’utente non sia stato aggiunto automaticamente al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Attività Completo alla squadra</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email alla squadra.</p> <p>I membri del team del progetto ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue non Assegnata alla Squadra Progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto su cui mi trovo.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui progetti che possiedo

Vedi anche [Notifiche: Informazioni sui progetti che possiedo](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Invia per Email l'Avviso del Documento al Proprietario del Progetto</p> </td> 
   <td> <p>Un documento viene aggiunto a un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che ha aggiunto il documento non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue al Proprietario del Progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica data conferma problema al proprietario del progetto</p> </td> 
   <td> <p>Modifiche della data di conferma per un problema su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando la data di commit cambia per un problema del progetto, a meno che l’utente che modifica la data di commit sia lo stesso utente del proprietario del progetto.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue Completa al Proprietario</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email al Proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'attività principale al Proprietario</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email al Proprietario del progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso del Proprietario al nuovo Proprietario</p> </td> 
   <td> <p>Quando si cambia il Proprietario del progetto, invia una Email al nuovo Proprietario.</p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso dello Stato Avanzamento Progetto al Proprietario</p> </td> 
   <td> <p>Un progetto che possiedo è indietro.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica data assunzione attività a Proprietario progetto</p> </td> 
   <td> <p>Modifiche della data di conferma per un'attività su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando la data di commit cambia per un'attività del progetto, a meno che l'utente che ha modificato la data di commit sia anche il proprietario del progetto.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Attività Completo al Proprietario progetto</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email una Notifica Stato Avanzamento Attività al Proprietario progetto</p> </td> 
   <td> <p>Quando si cambia lo stato di avanzamento di un'attività da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue non Assegnato al Proprietario del Progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto di cui sono titolare.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui progetti che sponsorizzo

Vedi anche [Notifiche: Informazioni sui progetti che sponsorizzo](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Invia per Email l'Avviso del Documento allo Sponsor Progetto</p> </td> 
   <td> <p>Un documento viene aggiunto a un progetto che sponsorizzo.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che il documento non venga aggiunto dallo sponsor del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il documento non è Privato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue allo sponsor del progetto</p> </td> 
   <td> <p>Un problema viene aggiunto a un progetto che sponsorizzo.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue Completa allo sponsor progetto</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email allo sponsor di Progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'attività principale allo sponsor</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un’attività cardine viene completata su un progetto sponsorizzato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso dello Stato Avanzamento Progetto allo Sponsor</p> </td> 
   <td> <p>Un progetto che sponsorizzo è indietro.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto viene ritardato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso del Sponsor al Nuovo Sponsor</p> </td> 
   <td> <p>Quando si cambia lo Sponsor, invia una Email al nuovo sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene impostato come sponsor di un progetto.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dell'Attività Completo allo Sponsor</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso dello Stato Avanzamento Attività allo Sponsor</p> </td> 
   <td> <p>Quando si cambia lo stato di avanzamento di un'attività da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email allo sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue non Assegnato allo sponsor del Progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto che sponsorizzo.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni varie

Vedi anche [Notifiche: Informazioni varie](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Notifica</td> 
   <td> <p>Notifica aggiunta</p> </td> 
   <td> <p>Messaggio inviato al centro notifiche.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento di richiesta documento al richiedente</p> </td> 
   <td> <p>Annulla da me una richiesta di caricamento del documento.</p> <p>Il richiedente del documento riceve una notifica e-mail quando una richiesta di documento viene annullata.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Avviso errore</p> </td> 
   <td> <p>È stato trovato un errore che richiede la tua attenzione.</p> <p>Una notifica e-mail viene generata dopo che Workfront tenta e non riesce a connettersi a un account POP. Dopo 25 tentativi, Workfront disabilita la connessione all’account POP al fine di preservare le risorse e invia una notifica. </p> <p>La notifica e-mail viene inviata al proprietario del progetto, se l’e-mail POP è associata a una coda di richiesta, o agli amministratori di Workfront, se l’account POP è associato alla funzione "Posta in arrivo" in Configurazione e-mail.
     <!--
      DRAFTED IN FLARE:
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      --></p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue al Proprietario risorsa</p> </td> 
   <td> <p>Quando si cambia l'incaricato di una Issue, invia una email al Proprietario della risorsa.</p> <p>Il Gestore assegnatari riceve una notifica e-mail quando una modifica interessa un utente che gestisce.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Invia per Email l'Avviso del Nuovo Utente all'Utente</p> </td> 
   <td> <p>Quando si crea un utente in Workfront, invia una Email all'utente.</p> <p>Dopo la creazione del nuovo utente, l’utente riceve un invito e-mail, avvisandolo che è stato creato un account Workfront e chiedendo loro di impostare la password.</p> <p>Quando crei un nuovo utente, gli utenti possono selezionare l’opzione "Invia un invito a questa persona" (come descritto in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a><span style="font-weight: 400;">). Tuttavia, quando l’opzione "Nuovo utente a utente" è abilitata a livello globale, tutti i nuovi utenti ricevono l’invito e-mail, indipendentemente dal fatto che sia selezionata l’opzione "Invia un invito a questa persona".</span></p> </td> 
   <td> Inattiva </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Condivisione oggetto con il team</p> </td> 
   <td> <p>Qualcuno condivide un oggetto con il mio team.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Condivisione oggetto con utente</p> </td> 
   <td> <p>Qualcuno condivide un oggetto con me.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Invia per Email l'Avviso della aggiunta Utente al Proprietario della Risorsa</p> </td> 
   <td> <p>Una delle mie persone viene aggiunta a un progetto.</p> <p>Un manager riceve una notifica e-mail quando uno dei suoi rapporti diretti viene aggiunto a un progetto.</p> <p>Gli utenti con una licenza di revisione non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto aggiunto a un portfolio o programma</p> </td> 
   <td> <p>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà.</p> </td> 
   <td> <p>Attivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso del cambio dell'Incaricato Attività al Proprietario della Risorsa</p> </td> 
   <td> <p>Quando viene cambiato l'incaricato primario di un'attività, invia una Email al Proprietario della risorsa.</p> <p>Il responsabile dell'assegnatario dell'attività riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> Progetto <br>Attività <br>Problema</td> 
   <td>Nuovo aggiornamento per l'iscritto </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Viene inviata un'e-mail quando viene effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono iscritto.</span> </p> </td> 
   <td>Attivi</td> 
  </tr> 
 </tbody> 
</table>

## Delega

Vedi anche [Notifiche: Delega](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo Oggetto | Evento | Descrizione | Stato predefinito |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Attività e problemi | Delega di attività e problemi all’assegnatario | Delego le mie attività e i miei problemi (conferma) | Attivi |
| Attività e problemi | Revoca la delega di attività e problemi all’assegnatario | Revoco la delega delle mie attività e dei miei problemi (conferma) | Attivi |
| Attività e problemi | Delega di attività e problemi al delegato | Qualcuno mi delega le sue attività e i suoi problemi | Attivi |
| Attività e problemi | Arresta le attività e rilascia la delega | Qualcuno mi revoca la delega delle sue attività e dei suoi problemi | Attivi |

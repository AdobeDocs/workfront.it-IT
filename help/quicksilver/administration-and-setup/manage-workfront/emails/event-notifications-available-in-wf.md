---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Notifiche degli eventi disponibili in Adobe Workfront
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività e problemi, come spiegato in Notifiche degli eventi.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '5006'
ht-degree: 29%

---

# Notifiche degli eventi disponibili in Adobe Workfront

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività e problemi, come spiegato in [Notifiche degli eventi](../../../workfront-basics/using-notifications/event-notifications.md).

Queste notifiche possono essere configurate a livello di sistema e di gruppo:

* Per informazioni sulla configurazione delle notifiche degli eventi a livello di sistema, consulta [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Per informazioni sulla configurazione delle notifiche degli eventi a livello di gruppo, consulta [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

I singoli utenti possono anche attivare e disattivare le notifiche dei singoli eventi nel loro profilo individuale. Per ulteriori informazioni, consulta [Modifica le tue notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Nelle tabelle seguenti sono elencate tutte le notifiche degli eventi di Adobe Workfront, una breve descrizione dell’evento e se l’evento è attivo o inattivo per impostazione predefinita.

## Azione richiesta

Vedi anche [Notifiche: azione necessaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

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
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Aggiunta di richiesta documento al richiedente</p> </td> 
   <td> <p>Richiedi di caricare i documenti.</p> <p>Il richiedente del documento riceve una notifica e-mail quando riceve una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento in attesa di approvazione per agli approvatori</p> </td> 
   <td> <p>Devo approvare un documento.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Asegnazione problema al Problema assegnato a</p> </td> 
   <td> <p>Mi viene assegnato un problema.</p> <p>L’assegnatario del problema riceve una notifica e-mail solo se lo stato del progetto è Corrente e lo stato del problema non è Chiuso o se è equivalente a Chiuso.</p> <p>Gli utenti con una licenza Revisione o Richiesta non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un problema.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l’impostazione "Approvatore non deve necessariamente trovarsi nel team di progetto (per i processi di approvazione che includono un ruolo)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, a tutti gli utenti del sistema viene inviata una notifica e-mail con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di "Approvatore" ricevono una notifica e-mail.</p> <p>Se il progetto è nello stato Pianificazione o Corrente, viene inviata una notifica. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione dell'approvatore delegato</p> </td> 
   <td> <p>Devo rivedere l'approvazione di un problema per il quale ho una delega.</p> <p>Quando un utente delega un’approvazione del problema a un altro utente, riceve una notifica. </p> <p>Una notifica viene inviata solo quando il progetto è nello stato Corrente.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un progetto.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l’impostazione "Approvatore non deve necessariamente trovarsi nel team del progetto (per i processi di approvazione che includono una mansione)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>).</p> <p>Se questa opzione è abilitata</strong>, a tutti gli utenti del sistema viene inviata una notifica e-mail con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di "Approvatore" ricevono una notifica e-mail.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Progetto in attesa di approvazione dell'approvatore delegato</td> 
   <td> <p>Devo rivedere l'approvazione di un progetto per il quale ho una delega.</p> </td> 
   <td> Attiva</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Invia per Email l'Avviso d'Incarico Attività al Nuovo Incaricato</p> </td> 
   <td> <p>Quando viene cambiato l'incaricato primario di un'attività, invia una Email al nuovo incaricato.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail se viene designato come assegnatario principale dell'attività, a meno che l'assegnatario non sia l'utente che ha effettuato l'assegnazione.</p> <p>Se lo stato del progetto è Corrente e l'attività non è contrassegnata come Completa, viene inviata una notifica.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione degli approvatori</p> </td> 
   <td> <p>Devo approvare un'attività.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l’impostazione "Approvatore non deve necessariamente trovarsi nel team di progetto (per i processi di approvazione che includono un ruolo)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, a tutti gli utenti del sistema viene inviata una notifica e-mail con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il ruolo di "Approvatore" ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione dell'approvatore delegato</p> </td> 
   <td> <p>Devo rivedere l'approvazione di un'attività per la quale ho una delega.</p> <p>Quando un utente delega un’approvazione del problema a un altro utente, riceve una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Scheda orario riaperta a utente</p> </td> 
   <td> <p>La mia scheda orario è stata riaperta.</p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene riaperta, a meno che l’utente che ha riaperto la scheda non sia anche il proprietario della scheda orario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è Aperto.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Scheda orario respinta all'utente</p> </td> 
   <td> <p>La mia scheda oraria è stata respinta.</p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene rifiutata, a meno che l’utente che ha rifiutato la scheda orario non sia anche il proprietario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è Rifiutato.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Invio della scheda orario all'approvatore</p> </td> 
   <td> <p>Devo approvare una scheda orario.</p> <p>L'approvatore della scheda orario riceve una notifica e-mail quando viene inviata una scheda orario da approvare, a meno che l'utente che ha inviato la scheda non sia anche l'approvatore della scheda orario.</p> <p>Una notifica viene inviata solo se lo stato della scheda orario è Inviato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro al team</p> </td> 
   <td> <p>Il mio team riceve una nuova richiesta di lavoro.</p> <p>I membri del team ricevono una notifica e-mail quando ricevono una nuova richiesta di lavoro. L’utente che ha inviato la richiesta non riceve una notifica se è membro del team.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta di lavoro e lo stato della richiesta di lavoro è Nuovo.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro ad Assegnatario elemento di lavoro</p> </td> 
   <td> <p>Ricevo una nuova richiesta di lavoro.</p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail, a meno che l’utente che effettua la richiesta non sia anche l’assegnatario. </p> <p>Non viene inviata una notifica se lo stato dell’attività è Completo o se lo stato del problema è Chiuso.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Richieste che ho effettuato

Vedi anche [Notifiche: richieste che ho effettuato](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

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
   <td> <p>Completata una richiesta di approvazione documento.</p> <p>Il richiedente del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene completata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Completamento di richiesta documento al richiedente</p> </td> 
   <td> <p>Richiesta di caricamento documento completata.</p> <p>Il richiedente del documento riceve una notifica e-mail quando viene soddisfatta una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta problema al contatto principale del problema</p> </td> 
   <td> <p>Aggiungo una issue al progetto.</p> <p>Il contatto principale per un problema riceve una notifica quando aggiunge un problema in un progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Assegnazione problema al contatto principale del problema</td> 
   <td> <p>Qualcuno è assegnato a un problema per il quale sono il contatto principale.</p> <p>Il contatto principale per un problema riceve una notifica quando il problema viene assegnato a un utente. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento del problema al contatto primario del problema</p> </td> 
   <td> <p>Un problema di cui sono il contatto principale è stato completato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica dello stato del progetto a Inserito da</p> </td> 
   <td> <p>Modifica dello stato di un progetto che ho creato.</p> <p>L’utente che ha creato il progetto riceve una notifica e-mail quando lo stato del progetto cambia.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta richiesta al contatto principale del problema</p> </td> 
   <td> <p>Invio una richiesta (conferma).</p> <p>Il contatto principale sul problema riceve una notifica e-mail quando invia un problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione richiesta al contatto principale del problema</p> </td> 
   <td> <p>Qualcuno è assegnato alla mia richiesta.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un utente viene assegnato al problema, a meno che il contatto principale e l’utente assegnato non siano lo stesso utente.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Richiesta chiusa al contatto principale del problema</p> </td> 
   <td> <p>La mia richiesta è chiusa (conferma).</p> <p>Il contatto principale del problema riceve una notifica e-mail quando la richiesta viene chiusa.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> <p>Se le notifiche di "completamento del problema" sono abilitate, verranno sempre attivate al posto di "Richiesta chiusa al contatto principale del problema". Se desideri attivare questa notifica, devi disattivare le notifiche di "completamento del problema".</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta richiesta documento al contatto principale del problema</p> </td> 
   <td> <p>Documento modificato o caricato su un problema per il quale sono il contatto principale.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un documento viene caricato o modificato sul problema, a meno che l’utente che ha caricato o modificato il documento non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se per il progetto è abilitata l'opzione "Pubblica come coda richieste di aiuto" nella scheda Impostazione coda.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica stato richiesta al contatto principale del problema</p> </td> 
   <td> <p>Lo stato della mia richiesta viene modificato.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando lo stato del problema cambia, a meno che l’utente che ha modificato lo stato non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Comunicazione

Vedi anche [Notifiche: comunicazione](../../../workfront-basics/using-notifications/notifications-communication.md).

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
   <td> <p>Commento su documento a proprietario documento</p> </td> 
   <td> <p>È stato aggiunto un commento sul mio documento.</p> <p>Il proprietario di un documento in Workfront riceve una notifica e-mail quando un commento viene pubblicato sul documento, a meno che l'utente che lo ha pubblicato non sia anche il proprietario del documento.</p> <p>Anche tutti gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente. </p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Commenta su &lt;request name=""&gt; il &lt;project name=""&gt; (rif. &lt;request reference="" number=""&gt;)</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è:<em> Digest di comunicazione &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Attiva </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Aggiunta nota richiesta al contatto principale del problema</p> </td> 
   <td> <p>Quando un commento viene pubblicato su una richiesta, invia un’e-mail al contatto principale del problema.</p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta, a meno che l’utente che lo ha pubblicato non sia anche il contatto principale per il problema.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento riceveranno una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td>Aggiornamento diretto all'utente</td> 
   <td> <p>Qualcuno mi include in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegna tag ad altri utenti in caso di aggiornamenti</a>.</p> <p>In questo caso, l’utente incluso nell’aggiornamento diretto riceve una notifica e-mail relativo all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo se l’utente dispone dei diritti di accesso all’oggetto e se lo mantiene abilitato nel suo profilo.  </p> <p>Questa notifica di evento è attivata per impostazione predefinita e non può essere disattivata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Aggiornamento diretto al team</p> </td> 
   <td> <p>Qualcuno include il mio team in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegna tag ad altri utenti in caso di aggiornamenti</a>.</p> <p>In questo caso, qualsiasi membro del team incluso nell’aggiornamento diretto riceve una notifica e-mail relativa all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo agli utenti che dispongono dei diritti di accesso all’oggetto dell’aggiornamento.</p> <p>Se l’utente che invia l’aggiornamento diretto è un membro del team incluso, l’utente che invia l’aggiornamento non riceve una notifica e-mail.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento elemento lavoro a Partecipanti argomento</p> </td> 
   <td> <p>Qualcuno ha commentato su un argomento che mi interessa.</p> <p>I partecipanti al thread e gli utenti inclusi in un messaggio diretto ricevono una notifica e-mail quando un utente aggiunge un commento al thread.</p> <p>Per ricevere una notifica, gli utenti devono disporre dell'accesso in visualizzazione.</p> <p>I seguenti utenti non ricevono una notifica:</p> 
    <ul> 
     <li> <p>Team inclusi in un messaggio diretto</p> </li> 
     <li> <p>Proprietario della nota</p> </li> 
     <li> <p>Il contatto principale</p> </li> 
    </ul> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento sull'elemento di lavoro ad assegnatario elemento di lavoro</p> </td> 
   <td> <p>Qualcuno ha commentato uno degli elementi del mio lavoro.</p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail ogni volta che un utente aggiunge un aggiornamento a un elemento di lavoro, a meno che l’utente che aggiunge l’aggiornamento non sia anche l’assegnatario.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Risposta alla richiesta di lavoro a Richiedente lavoro</p> </td> 
   <td> <p>Qualcuno ha risposto alla mia richiesta.</p> <p>Dopo che un utente invia una richiesta e un altro utente risponde a tale richiesta, l’utente che ha inviato la richiesta riceve una notifica e-mail.</p> <p>Una notifica e-mail non viene inviata se:</p> 
    <ul> 
     <li> <p>L'utente che risponde è lo stesso utente che ha effettuato la richiesta</p> </li> 
     <li> <p>L’utente non ha accesso alla visualizzazione della nota</p> </li> 
    </ul> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Informazioni sull&#39;approvazione

Vedi anche [Notifiche: informazioni sull’approvazione](../../../workfront-basics/using-notifications/notifications-approval-information.md).

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
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica dello stato di approvazione del problema delegato</p> </td> 
   <td> <p>Una richiesta di approvazione del problema delegato è stata completata. </p> <p>Quando deleghi un’approvazione del problema a un altro utente, al termine dell’approvazione riceverai una notifica e-mail (che indica se l’approvazione del problema è stata approvata o rifiutata). </p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica dello stato di approvazione del progetto delegata</p> </td> 
   <td> <p>Una richiesta di approvazione del progetto delegato è stata completata.</p> <p>Quando deleghi l’approvazione di un progetto a un altro utente, al termine dell’approvazione riceverai una notifica e-mail, indicando se l’approvazione è stata approvata o rifiutata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica dello stato di approvazione dell'attività delegata</p> </td> 
   <td> <p>Lo stato di approvazione di un'attività delegata è completato.</p> <p>Quando si delega l'approvazione di un'attività a un altro utente, al termine dell'approvazione viene inviata una notifica e-mail, a prescindere dal fatto che l'approvazione venga approvata o rifiutata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento approvazione documento all'approvatore</p> </td> 
   <td> <p>Annullata una richiesta di approvazione documento.</p> <p>L’approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Approvazione della scheda orario all'utente</p> </td> 
   <td> <p>La mia scheda oraria è stata approvata.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sul lavoro assegnato a me

Vedi anche [Notifiche: informazioni sul lavoro assegnato a me](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

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
   <td> <p>Tutti i predecessori delle attività del team sono completati.</p> <p>Gli assegnatari dell’attività (tutti i membri del team) ricevono una notifica e-mail.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td>Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Il completamento di tutte le Attività Predecessore ad Attività Dipendenti</p> </td> 
   <td> <p>Tutti i predecessori delle mie attività sono state completate.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisione di approvazione su Problema assegnato a</p> </td> 
   <td> <p>Un problema che io risolvo è approvato o rifiutato.</p> <p>L’assegnatario di un problema riceve una notifica e-mail quando viene presa una decisione di approvazione (approvata o rifiutata).</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Decisione di approvazione dell'attività assegnata a</p> </td> 
   <td> <p>Un'attività che ho completato è stata approvata o respinta.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando l’attività viene approvata o rifiutata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento del problema al problema assegnato a</p> </td> 
   <td> <p>Un problema a cui sono stato assegnato è completo.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Data di completamento problema pianificata cambiata</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un problema al quale sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando cambia la Data di completamento pianificata, a meno che l’utente che ha modificato la Data di completamento pianificata non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è diverso da Pianificazione.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica stato del problema a Problema assegnato a</p> </td> 
   <td> <p>Modifica dello stato di uno degli elementi del mio lavoro.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando lo stato cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento richiesta a Problema assegnato a</p> </td> 
   <td> <p>I documenti vengono caricati o modificati sulle richieste alle quali sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando i documenti vengono caricati o modificati in seguito a un problema da lui aggiunto.</p> <p>Una notifica e-mail non viene inviata se l’utente che ha inserito il problema è l’assegnatario del problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se per il progetto è abilitata l'opzione "Pubblica come coda richieste di aiuto" nella scheda Impostazione coda.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività ad attività assegnata a</p> </td> 
   <td> <p>Un'attività a cui sono assegnato è stata completata.</p> <p>L’Assegnatario dell’attività riceve una notifica e-mail quando l’attività viene completata. Le notifiche non vengono inviate al completamento di un'attività personale.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Revisione o Richiedente non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività ai dipendenti delle attività</p> </td> 
   <td> <p>Il predecessore di una delle mie attività è stato completato.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando uno dei predecessori dell’attività è stato completato.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Data di completamento attività pianificata modificata</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un'attività a cui sono assegnato.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail quando cambia la data di completamento pianificata dell'attività, a meno che l'utente che ha modificato la data di completamento pianificata non sia anche l'assegnatario dell'attività.</p> <p>Una notifica viene inviata solo se lo stato del progetto è diverso da Pianificazione.</p> <p>Non viene inviata alcuna notifica relativa alle attività personali.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica stato dell'attività a Attività assegnata a</p> </td> 
   <td> <p>Modifica dello stato per un attività a cui sono stato assegnato.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando lo stato dell’attività cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informazioni sui progetti a cui collaboro

Vedi anche [Notifiche: informazioni sui progetti a cui collaboro](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

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
   <td> <p>Modifica dello stato attuale del progetto al team di progetto</p> </td> 
   <td> <p>Un progetto a cui partecipo diventa attivo.</p> <p>Gli utenti del progetto ricevono una notifica e-mail quando il progetto diventa attivo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento al team di progetto</p> </td> 
   <td> <p>Viene aggiunto un documento a un progetto a cui collavoro.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando un documento viene aggiunto al progetto, ad eccezione dell’utente che ha aggiunto il documento.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta problema al team di progetto</p> </td> 
   <td> <p>Viene aggiunto un problema a un progetto a cui collaboro.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento del problema al team di progetto</p> </td> 
   <td> <p>Viene completato un problema su un progetto a cui partecipo.</p> <p>Qualsiasi utente del progetto riceve una notifica.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività principale al team di progetto</p> </td> 
   <td> <p>Un'attività principale è stata completata su un progetto a cui collaboro.</p> <p>Tutti gli utenti del team di progetto ricevono una notifica al completamento di un'attività cardine. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Completamento del progetto al team di progetto</p> </td> 
   <td> <p>Un progetto a cui partecipo è stato completato.</p> <p>Gli utenti di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è Completo.</p> <p>Suggerimento: se i progetti vengono completati regolarmente, l’abilitazione di questa opzione può creare molti messaggi e-mail per gli utenti che hanno un numero limitato di attività su molti progetti. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica dello stato di progetto al team di progetto</p> </td> 
   <td> <p>Lo stato di un progetto a cui partecipo viene modificato.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando lo stato del progetto cambia. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Aggiunta di un utente al progetto all'utente del progetto</p> </td> 
   <td> <p>Sono aggiunto a un progetto.</p> <p>L’utente che è stato aggiunto al progetto riceve una notifica e-mail quando viene aggiunto, a meno che non sia stato aggiunto autonomamente al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività completata al team di progetto</p> </td> 
   <td> <p>Viene completata un'attività su un progetto a cui partecipo.</p> <p>I membri del team di progetto ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema non assegnato aggiunto al team di progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto a cui partecipo.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui progetti di mia proprietà

Vedi anche [Notifiche: informazioni sui progetti di mia proprietà](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

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
   <td> <p>Aggiunta documento al proprietario del progetto</p> </td> 
   <td> <p>Viene aggiunto un documento a un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che lo ha aggiunto non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta di un problema al proprietario del progetto</p> </td> 
   <td> <p>Viene aggiunto un problema a un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica della data di conferma del problema al proprietario del progetto</p> </td> 
   <td> <p>Modifiche della data di conferma per un problema su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un problema sul progetto, a meno che l’utente che modifica la data di conferma sia lo stesso del proprietario del progetto.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento del problema al proprietario del proprietario</p> </td> 
   <td> <p>Un problema è stato completato in un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività principale al proprietario del progetto</p> </td> 
   <td> <p>Un'attività principale è stata completata su un progetto di cui sono proprietario.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Assegnazione del proprietario di progetto al proprietario di progetto</p> </td> 
   <td> <p>Sono nominato proprietario di un unovo progetto.</p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica avanzamewnto di progetto al proprietario del progetto</p> </td> 
   <td> <p>Un progettodi mia proprietà è in ritardo.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo rispetto alla pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica data di conferma attività a proprietario progetto</p> </td> 
   <td> <p>Modifiche della data di conferma per un'attività su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un’attività del progetto, a meno che l’utente che ha modificato la data di conferma non sia anche il proprietario del progetto.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività al proprietario di progetto</p> </td> 
   <td> <p>Un'attività viene completata su un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica avanzamento dell'attività al proprietario di progetto</p> </td> 
   <td> <p>Un'attività di mia proprietà è in ritardo.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta problema non assegnato al proprietario di progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto di cui sono proprietario.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui progetti di cui sono sponsor

Vedi anche [Notifiche: informazioni sui progetti di cui sono sponsor](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

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
   <td> <p>Aggiunta documento allo sposnsor di progetto</p> </td> 
   <td> <p>Viene aggiunto un documento a un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che il documento non venga aggiunto dallo sponsor del progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente e se il documento non è Privato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Agiunta problema a sponsore del progetto</p> </td> 
   <td> <p>Viene aggiunto un problema a un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema allo sponsor del progetto</p> </td> 
   <td> <p>Viene completato un problema su un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività principale allo sposnsor del progetto</p> </td> 
   <td> <p>Un'attività principale viene completata in un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando completa un’attività cardine su un progetto di cui è sponsor.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica avanzamento dell'attività allo sponsor di progetto</p> </td> 
   <td> <p>Un progetto di cui sono sponsor è in ritardo.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto è in ritardo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Assegnazione nuovo sponsor allo sponsor di progetto</p> </td> 
   <td> <p>Sono scelto come sponsor di un progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene impostato come sponsor di un progetto.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento dell'attività allo sponsor del progetto</p> </td> 
   <td> <p>Un'attità viene completata su un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica dell'avanzamento del progetto allo sponsor del progetto</p> </td> 
   <td> <p>Un'attività su un progetto di cui sono sponsor è in ritardo.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta problema non assegnato allo sponsor di progetto</p> </td> 
   <td> <p>Un problema non assegnato viene aggiunto a un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un problema non assegnato viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni varie

Vedi anche [Notifiche: informazioni varie](../../../workfront-basics/using-notifications/notifications-misc-information.md).

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
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento di richiesta documento al richiedente</p> </td> 
   <td> <p>Annulla una richiesta di caricamento documento da parte mia.</p> <p>Il richiedente del documento riceve una notifica e-mail quando viene annullata una richiesta di documento.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Avviso errore</p> </td> 
   <td> <p>È stato rilevato un errore che richiede la tua attenzione.</p> <p>Una notifica e-mail viene generata dopo che Workfront tenta di connettersi a un account POP. Dopo 25 tentativi, Workfront disattiva la connessione all’account POP per preservare le risorse e invia una notifica. </p> <p>La notifica e-mail viene inviata al proprietario del progetto, se l’e-mail POP è associata a una coda di richieste, o agli amministratori di Workfront, se l’account POP è associato alla funzione "Posta in arrivo" in Email Setup.
   </p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione problema al proprietario della risorsa</p> </td> 
   <td> <p>La modifica dell'assegnazione di un problema interessa una mia risorsa.</p> <p>L’Assegnatario del problema riceve una notifica e-mail quando una modifica interessa un utente che gestisce.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Nuovo utente a utente</p> </td> 
   <td> <p>Quando si crea un utente in Workfront, invia una Email all'utente.</p> <p>Dopo la creazione del nuovo utente, l'utente riceve un invito e-mail, che notifica la creazione di un account Workfront e richiede di impostare la password.</p> <p>Durante la creazione di un nuovo utente, gli utenti possono selezionare l’opzione "Send an invite email to this person" (Invia un’e-mail di invito a questa persona) (come descritto in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a><span style="font-weight: 400;">). Tuttavia, quando l’opzione "Nuovo utente all’utente" è abilitata a livello globale, tutti i nuovi utenti ricevono l’invito e-mail indipendentemente dal fatto che sia selezionata l’opzione "Invia un’e-mail di invito a questa persona".</span></p> </td> 
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
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Aggiunta utente progetto al proprietario della risorsa</p> </td> 
   <td> <p>Una delle mie risrse viene aggiunta a un progetto.</p> <p>Un manager riceve una notifica e-mail quando uno dei suoi referenti diretti viene aggiunto a un progetto.</p> <p>Gli utenti con una licenza Review (Revisione) non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto aggiunto a un portfolio o programma</p> </td> 
   <td> <p>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Assegnazione attività al proprietario della risorsa</p> </td> 
   <td> <p>La modifica dell'assegnazione di un problema interessa una mia risorsa.</p> <p>Il Manager dell'assegnatario dell'attività riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> Progetto <br>Attività <br>Problema</td> 
   <td>Nuovo aggiornamento per l'iscritto </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Un messaggio e-mail viene inviato quando viene effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono abbonato.</span> </p> </td> 
   <td>Attiva</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delega

Vedi anche [Notifiche: delega](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Tipo Oggetto | Evento | Descrizione | Stato predefinito |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Attività e problemi | Delega di attività e problemi all’assegnatario | Delego le mie attività e i miei problemi (conferma) | Attiva |
| Attività e problemi | Revoca la delega di attività e problemi all’assegnatario | Revoco la delega delle mie attività e dei miei problemi (conferma) | Attiva |
| Attività e problemi | Delega di attività e problemi al delegato | Qualcuno mi delega le sue attività e i suoi problemi | Attiva |
| Attività e problemi | Revoca le attività e delega dei problemi al delegato | Qualcuno mi revoca la delega delle sue attività e dei suoi problemi | Attiva |

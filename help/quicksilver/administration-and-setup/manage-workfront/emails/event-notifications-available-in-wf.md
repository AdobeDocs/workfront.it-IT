---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Tipi di notifica degli eventi
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività e problemi. Questo articolo elenca e descrive i tipi disponibili di notifiche di eventi.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 7%

---

# Tipi di notifica degli eventi

<!-- Audited: 1/2024 -->

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti quali progetti, attività e problemi, come spiegato in [Notifiche degli eventi](../../../workfront-basics/using-notifications/event-notifications.md).

Queste notifiche possono essere configurate a livello di sistema e di gruppo:

* Per informazioni sulla configurazione delle notifiche degli eventi a livello di sistema, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Per informazioni sulla configurazione delle notifiche degli eventi a livello di gruppo, vedere [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

I singoli utenti possono anche attivare e disattivare le notifiche dei singoli eventi nel loro profilo individuale. Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Nelle tabelle seguenti sono elencate tutte le notifiche degli eventi di Adobe Workfront, una breve descrizione dell’evento e se l’evento è attivo o inattivo per impostazione predefinita.

>[!NOTE]
>
>Le notifiche con il valore &quot;Attivo&quot; nella colonna Stato predefinito sono attive sia per le notifiche istantanee che per quelle giornaliere per impostazione predefinita, salvo diversa indicazione.

## Azione richiesta

Vedi anche [Notifiche: azione richiesta](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th>Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Richiesta di accesso</p> </td> 
   <td> <p>Utente</p> </td> 
   <td> <p>Qualcuno mi ha richiesto l'accesso.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> <p> </p> </td> 
   <td> <p>Aggiunta richiesta documento</p> </td> 
   <td> <p>Utente a cui è richiesto il documento</p> </td> 
   <td> <p>Qualcuno mi ha richiesto di caricare i documenti.</p> <p>Il richiedente del documento riceve una notifica e-mail quando riceve una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Documento in attesa di approvazione</p> </td> 
   <td> <p>Approvatori</p> </td> 
   <td> <p>Devo approvare un documento.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione problema</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>Quando si cambia l'incaricato di una Issue, invia una Email al nuovo incaricato.</p> <p>L’assegnatario del problema riceve una notifica e-mail solo se lo stato del progetto è Corrente e lo stato del problema non è Chiuso o se è equivalente a Chiuso.</p> <p>Gli utenti con una licenza Light, Contributor, Review o Request non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione</p> </td> 
   <td> <p>Approvatori</p> </td> 
   <td> <p>Devo approvare un problema.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione "Approvatore non deve necessariamente essere nel team di progetto (per i processi di approvazione che includono un ruolo)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il Ruolo "Approvatore" riceveranno una notifica e-mail.</p> <p>Se il progetto è nello stato Pianificazione o Corrente, viene inviata una notifica. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema in attesa di approvazione</p> </td> 
   <td> <p>Approvatore delegato</p> </td> 
   <td> <p>Devo rivedere l'approvazione di un problema per il quale ho una delega.</p> <p>Quando un utente delega un’approvazione del problema a un altro utente, riceve una notifica. </p> <p>Una notifica viene inviata solo quando il progetto è nello stato Corrente.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto in attesa di approvazione</p> </td> 
   <td> <p>Approvatori</p> </td> 
   <td> <p>Devo approvare un progetto.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione "Approvatore non deve necessariamente essere nel team di progetto (per i processi di approvazione che includono una mansione)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>).</p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il Ruolo "Approvatore" riceveranno una notifica e-mail.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Progetto in attesa di approvazione</td> 
   <td>Approvatore delegato</td> 
   <td> <p>Devo rivedere l'approvazione di un progetto per il quale ho una delega.</p> </td> 
   <td> Attiva</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Assegnazione attività</p> </td> 
   <td> <p>Utente a cui è assegnata l’attività</p> </td> 
   <td> <p>Quando viene impostato l'assegnatario principale di un'attività,</p> <p>L'assegnatario dell'attività riceve una notifica e-mail se viene designato come assegnatario principale dell'attività, a meno che l'assegnatario non sia l'utente che ha effettuato l'assegnazione.</p> <p>Se lo stato del progetto è Corrente e l'attività non è contrassegnata come Completa, viene inviata una notifica.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione</p> </td> 
   <td> <p>Approvatori</p> </td> 
   <td> <p>Devo approvare un'attività.</p> <p>Gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione "Approvatore non deve necessariamente essere nel team di progetto (per i processi di approvazione che includono un ruolo)" sia abilitata (come descritto in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con il Ruolo "Approvatore".</p> <p>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con il Ruolo "Approvatore" riceveranno una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Attività in attesa di approvazione</p> </td> 
   <td> <p>Approvatore delegato</p> </td> 
   <td> <p>Devo rivedere l'approvazione di un'attività per la quale ho una delega.</p> <p>Quando un utente delega un’approvazione del problema a un altro utente, riceve una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Scheda orario riaperta</p> </td> 
   <td> <p>Utente a cui appartiene la scheda orario</p> </td> 
   <td> <p>La mia scheda orario è stata riaperta.</p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene riaperta, a meno che l’utente che ha riaperto la scheda non sia anche il proprietario della scheda orario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è Aperto.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Rifiuto scheda orario</p> </td> 
   <td> <p>Utente a cui appartiene la scheda orario</p> </td> 
   <td> <p>La mia scheda orario è stata rifiutata.</p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene rifiutata, a meno che l’utente che ha rifiutato la scheda orario non sia anche il proprietario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è Rifiutato.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Invio scheda orario</p> </td> 
   <td> <p>Approvatore</p> </td> 
   <td> <p>Devo approvare una scheda orario.</p> <p>L'approvatore della scheda orario riceve una notifica e-mail quando viene inviata una scheda orario da approvare, a meno che l'utente che ha inviato la scheda non sia anche l'approvatore della scheda orario.</p> <p>Una notifica viene inviata solo se lo stato della scheda orario è Inviato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro</p> </td> 
   <td> <p>Membri del team per cui è richiesto l'elemento</p> </td> 
   <td> <p>Il mio team riceve una nuova richiesta di lavoro.</p> <p>I membri del team ricevono una notifica e-mail quando ricevono una nuova richiesta di lavoro. L’utente che ha inviato la richiesta non riceve una notifica se è membro del team.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta di lavoro e lo stato della richiesta di lavoro è Nuovo.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione</p> </td> 
   <td> <p>Richiesta elemento di lavoro</p> </td> 
   <td> <p>Utente per cui è richiesto l'elemento di lavoro</p> </td> 
   <td> <p>Ricevo una nuova richiesta di lavoro.</p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail, a meno che l’utente che effettua la richiesta non sia anche l’assegnatario. </p> <p>Non viene inviata una notifica se lo stato dell’attività è Completo o se lo stato del problema è Chiuso.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente al momento della richiesta.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
 </tbody> 
</table>

## Richieste che ho effettuato

Vedi anche [Notifiche: richieste effettuate](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Modifica stato approvazione documento</p> </td> 
   <td> <p>Richiedente</p> </td> 
   <td> <p>Richiesta di approvazione documento completata.</p> <p>Il richiedente del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene completata.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Richiesta documento completata</p> </td> 
   <td> <p>Richiedente</p> </td> 
   <td> <p>Richiesta di caricamento documento completata.</p> <p>Il richiedente del documento riceve una notifica e-mail quando viene soddisfatta una richiesta di caricamento di un documento.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email alla squadra.</p> <p>Il contatto principale per un problema riceve una notifica quando aggiunge un problema in un progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Assegnazione problema</td> 
   <td>Contatto principale problema</td> 
   <td> <p>Qualcuno è assegnato a un problema per il quale sono il contatto principale.</p> <p>Il contatto principale per un problema riceve una notifica quando il problema viene assegnato a un utente. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email all'autore.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica stato progetto</p> </td> 
   <td> <p>Utente che ha creato il progetto (Inserito da)</p> </td> 
   <td> <p>Lo stato cambia in un progetto creato.</p> <p>L’utente che ha creato il progetto riceve una notifica e-mail quando lo stato del progetto cambia.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Aggiunta richiesta</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Invio una richiesta (conferma).</p> <p>Il contatto principale sul problema riceve una notifica e-mail quando invia un problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione richiesta</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Qualcuno è assegnato alla mia richiesta.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un utente viene assegnato al problema, a meno che il contatto principale e l’utente assegnato non siano lo stesso utente.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Richiesta chiusa</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>La mia richiesta è chiusa (conferma).</p> <p>Il contatto principale del problema riceve una notifica e-mail quando la richiesta viene chiusa.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto utilizza una visualizzazione Help Desk.</p> <p>Se le notifiche di "completamento del problema" sono abilitate, verranno sempre attivate al posto di "Richiesta chiusa al contatto principale del problema". Se desideri attivare questa notifica, devi disattivare le notifiche di "completamento del problema".</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiungi documento richiesta</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Un documento viene modificato o caricato su un problema per il quale sono il contatto principale.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando un documento viene caricato o modificato sul problema, a meno che l’utente che ha caricato o modificato il documento non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se nel progetto è abilitata l'opzione "Publish as Help Request Queue" nella scheda Queue Setup (Impostazione coda).</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Richiedi modifica stato</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Lo stato cambia su mia richiesta.</p> <p>Il contatto principale del problema riceve una notifica e-mail quando lo stato del problema cambia, a meno che l’utente che ha modificato lo stato non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il progetto utilizza una visualizzazione Help Desk.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Commento sul documento</p> </td> 
   <td> <p>Proprietario documento</p> </td> 
   <td> <p>È stato aggiunto un commento al documento.</p> <p>Il proprietario di un documento in Workfront riceve una notifica e-mail quando un commento viene pubblicato sul documento, a meno che l'utente che lo ha pubblicato non sia anche il proprietario del documento.</p> <p>Anche tutti gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente. </p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Commento su &lt;Nome richiesta&gt; in &lt;Nome progetto&gt; (ref# &lt;Numero di riferimento richiesta&gt;)</em></p> <p> L'oggetto della notifica del riepilogo giornaliero è:<em> Digest di comunicazione &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Aggiunta nota richiesta</p> </td> 
   <td> <p>Contatto principale problema</p> </td> 
   <td> <p>Quando un commento viene pubblicato su una richiesta, invia un’e-mail al contatto principale del problema.</p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta, a meno che l’utente che lo ha pubblicato non sia anche il contatto principale per il problema.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento riceveranno una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td>Aggiornamento diretto</td> 
   <td>Utente</td> 
   <td> <p>Qualcuno mi include in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag ad altri utenti negli aggiornamenti</a>.</p> <p>In questo caso, l’utente incluso nell’aggiornamento diretto riceve una notifica e-mail relativo all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo se l’utente dispone dei diritti di accesso all’oggetto e se lo mantiene abilitato nel suo profilo.  </p> <p>Questa notifica di evento è attivata per impostazione predefinita e non può essere disattivata.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Aggiornamento diretto</p> </td> 
   <td> <p>Membri team</p> </td> 
   <td> <p>Qualcuno include il mio team in un aggiornamento diretto.</p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag ad altri utenti negli aggiornamenti</a>.</p> <p>In questo caso, qualsiasi membro del team incluso nell’aggiornamento diretto riceve una notifica e-mail relativa all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo agli utenti che dispongono dei diritti di accesso all’oggetto dell’aggiornamento.</p> <p>Se l’utente che invia l’aggiornamento diretto è un membro del team incluso, l’utente che invia l’aggiornamento non riceve una notifica e-mail.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento elemento di lavoro</p> </td> 
   <td> <p>Partecipanti thread</p> </td> 
   <td> <p>Qualcuno ha commentato su un argomento in cui mi trovo.</p> <p>I partecipanti al thread e gli utenti inclusi in un messaggio diretto ricevono una notifica e-mail quando un utente aggiunge un commento al thread.</p> <p>Per ricevere una notifica, gli utenti devono disporre dell'accesso in visualizzazione.</p> <p>I seguenti utenti non ricevono una notifica:</p> 
    <ul> 
     <li> <p>Team inclusi in un messaggio diretto</p> </li> 
     <li> <p>Proprietario della nota</p> </li> 
     <li> <p>Il contatto principale</p> </li> 
    </ul> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Commento elemento di lavoro</p> </td> 
   <td> <p>Assegnatario elemento di lavoro</p> </td> 
   <td> <p>Qualcuno ha commentato uno dei miei elementi di lavoro.</p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail ogni volta che un utente aggiunge un aggiornamento a un elemento di lavoro, a meno che l’utente che aggiunge l’aggiornamento non sia anche l’assegnatario.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nota</p> </td> 
   <td> <p>Risposta richiesta di lavoro</p> </td> 
   <td> <p> Richiedente lavoro</p> </td> 
   <td> <p>Qualcuno ha risposto alla mia richiesta.</p> <p>Dopo che un utente invia una richiesta e un altro utente risponde a tale richiesta, l’utente che ha inviato la richiesta riceve una notifica e-mail.</p> <p>Una notifica e-mail non viene inviata se:</p> 
    <ul> 
     <li> <p>L'utente che risponde è lo stesso utente che ha effettuato la richiesta</p> </li> 
     <li> <p>L’utente non ha accesso alla visualizzazione della nota</p> </li> 
    </ul> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Informazioni sull&#39;approvazione

Vedi anche [Notifiche: informazioni sull&#39;approvazione](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo Oggetto</th> 
   <th>Evento</th> 
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Delega approvazione</p> </td> 
   <td> <p>Utente</p> </td> 
   <td> <p>Sono delegato come approvatore.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica dello stato di approvazione del problema delegato</p> </td> 
   <td> <p>Utente che ha delegato l'approvazione</p> </td> 
   <td> <p>Una richiesta di approvazione del problema delegata è stata completata. </p> <p>Quando deleghi un’approvazione del problema a un altro utente, al termine dell’approvazione riceverai una notifica e-mail (che indica se l’approvazione del problema è stata approvata o rifiutata). </p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica dello stato di approvazione del progetto delegata</p> </td> 
   <td> <p>Utente che ha delegato l'approvazione</p> </td> 
   <td> <p>Una richiesta di approvazione del progetto delegata è stata completata.</p> <p>Quando deleghi l’approvazione di un progetto a un altro utente, al termine dell’approvazione riceverai una notifica e-mail, indicando se l’approvazione è stata approvata o rifiutata.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica dello stato di approvazione dell'attività delegata</p> </td> 
   <td> <p>Utente che ha delegato l'approvazione</p> </td> 
   <td> <p>Lo stato di approvazione di un'attività delegata è completato.</p> <p>Quando si delega l'approvazione di un'attività a un altro utente, al termine dell'approvazione viene inviata una notifica e-mail, a prescindere dal fatto che l'approvazione venga approvata o rifiutata.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento approvazione documento all'approvatore</p> </td> 
   <td> <p>Utente che ha delegato l'approvazione</p> </td> 
   <td> <p>Richiesta di approvazione documento annullata.</p> <p>L’approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scheda orario</p> </td> 
   <td> <p>Approvazione scheda orario</p> </td> 
   <td> <p>Utente a cui appartiene la scheda orario</p> </td> 
   <td> <p>La mia scheda orario è approvata.</p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Attività</td> 
   <td>Completamento di tutte le attività predecessore</td> 
   <td>Membri del team assegnati ad attività dipendenti</td> 
   <td> <p>Tutti i predecessori delle attività del team sono completati.</p> <p>Gli assegnatari dell’attività (tutti i membri del team) ricevono una notifica e-mail.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td>Inattiva</td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento di tutte le attività predecessore</p> </td> 
   <td> <p>Utente assegnato ad attività dipendenti</p> </td> 
   <td> <p>Tutti i predecessori delle mie attività sono completati.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Decisione di approvazione</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>Un problema che io risolvo è approvato o rifiutato.</p> <p>L’assegnatario di un problema riceve una notifica e-mail quando viene presa una decisione di approvazione (approvata o rifiutata).</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Decisione di approvazione</p> </td> 
   <td> <p>Utente a cui è assegnata l’attività</p> </td> 
   <td> <p>Quando si completa un'attività, questa viene approvata o rifiutata.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando l’attività viene approvata o rifiutata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email alla squadra.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Data di completamento problema pianificata cambiata</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un problema a cui sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando cambia la Data di completamento pianificata, a meno che l’utente che ha modificato la Data di completamento pianificata non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è diverso da Pianificazione.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica stato problema</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>Lo stato cambia su uno degli elementi del mio lavoro.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando lo stato cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiungi documento richiesta</p> </td> 
   <td> <p>Utente a cui è assegnato il problema</p> </td> 
   <td> <p>I documenti vengono caricati o modificati sulle richieste a cui sono assegnato.</p> <p>L’assegnatario del problema riceve una notifica e-mail quando i documenti vengono caricati o modificati in seguito a un problema da lui aggiunto.</p> <p>Una notifica e-mail non viene inviata se l’utente che ha inserito il problema è l’assegnatario del problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se nel progetto è abilitata l'opzione "Publish as Help Request Queue" nella scheda Queue Setup (Impostazione coda).</p> </td> 
   <td> <p>Attivo (solo giornaliero)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività</p> </td> 
   <td> <p>Utente a cui è assegnata l’attività</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email all'incaricato.</p> <p>L’Assegnatario dell’attività riceve una notifica e-mail quando l’attività viene completata. Le notifiche non vengono inviate al completamento di un'attività personale.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Light, Contributor, Review o Requestor non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività</p> </td> 
   <td> <p>Utente assegnato all'attività dipendente</p> </td> 
   <td> <p>Un predecessore di una delle mie attività è completato.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando uno dei predecessori dell’attività è stato completato.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Data di completamento attività pianificata modificata</p> </td> 
   <td> <p>Utente a cui è assegnata l’attività</p> </td> 
   <td> <p>Le modifiche della data di scadenza su un'attività a cui sono assegnato.</p> <p>L'assegnatario dell'attività riceve una notifica e-mail quando cambia la data di completamento pianificata dell'attività, a meno che l'utente che ha modificato la data di completamento pianificata non sia anche l'assegnatario dell'attività.</p> <p>Una notifica viene inviata solo se lo stato del progetto è diverso da Pianificazione.</p> <p>Non viene inviata alcuna notifica relativa alle attività personali.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica stato attività</p> </td> 
   <td> <p>Utente a cui è assegnata l’attività</p> </td> 
   <td> <p>Lo stato cambia su un'attività a cui sono assegnato.</p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando lo stato dell’attività cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica. </p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Stato progetto corrente</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Un progetto al quale collaboro diventa attivo.</p> <p>Gli utenti del progetto ricevono una notifica e-mail quando il progetto diventa attivo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si aggiunge un documento, invia una Email alla squadra.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando un documento viene aggiunto al progetto, ad eccezione dell’utente che ha aggiunto il documento.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email alla squadra.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email alla squadra.</p> <p>Qualsiasi utente del progetto riceve una notifica.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività milestone</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email alla squadra.</p> <p>Tutti gli utenti del team di progetto ricevono una notifica al completamento di un'attività cardine. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Completamento progetto</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si completa un progetto, invia una Email alla squadra.</p> <p>Gli utenti di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è Completo.</p> <p>Suggerimento: se i progetti vengono completati regolarmente, l’abilitazione di questa opzione può creare molti messaggi e-mail per gli utenti che hanno un numero limitato di attività su molti progetti. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Modifica stato progetto</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Lo stato cambia su un progetto a cui collaboro.</p> <p>Gli utenti del team di progetto ricevono una notifica e-mail quando lo stato del progetto cambia. </p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Aggiunta utente progetto</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si aggiunge un utente a un progetto, invia una Email all'utente</p> <p>L’utente che è stato aggiunto al progetto riceve una notifica e-mail quando viene aggiunto, a meno che non sia stato aggiunto autonomamente al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email alla squadra.</p> <p>I membri del team di progetto ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Problema non assegnato aggiunto</p> </td> 
   <td> <p>Membri del team di progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue non assegnata, invia una Email alla squadra.</p> <p>Gli utenti di un progetto ricevono una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Un documento viene aggiunto a un progetto di mia proprietà.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che lo ha aggiunto non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il documento non è Privato.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Modifica data conferma problema</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Le modifiche della data di conferma per un problema su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un problema sul progetto, a meno che l’utente che modifica la data di conferma sia lo stesso del proprietario del progetto.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività milestone</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email al Proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Assegnazione proprietario progetto</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si cambia il proprietario, invia una Email al nuovo Proprietario.</p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Cambia Stato di Avanzamento Progetto</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Un progetto che possiedo sta dietro.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo rispetto alla pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Modifica data conferma attività</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Modifiche alla data di conferma per un'attività su uno dei miei progetti.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un’attività del progetto, a meno che l’utente che ha modificato la data di conferma non sia anche il proprietario del progetto.</p> </td> 
   <td> <p>Attiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Cambiamento Avanzamento Attività</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Un'attività su un progetto di mia proprietà sta per essere abbandonata.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue non Assegnato</p> </td> 
   <td> <p>Proprietario progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue non assegnata, invia una Email al Proprietario del progetto.</p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Aggiunta documento</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Un documento viene aggiunto a un progetto di cui sono sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che il documento non venga aggiunto dallo sponsor del progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente e se il documento non è Privato.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Issue Add</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Completamento problema</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si completa una Issue, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività milestone</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si completa un'attività principale, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando completa un’attività cardine su un progetto di cui è sponsor.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Cambia Stato di Avanzamento Progetto</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Un progetto di cui sono sponsor è dietro di me.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto è in ritardo.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Assegnazione Sponsor Progetto</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si cambia lo sponsor, invia una Email al nuovo sponsor.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene impostato come sponsor di un progetto.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Completamento attività</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si completa un'attività, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Cambiamento Avanzamento Attività</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Un'attività su un progetto di cui sono sponsor è sostenuta.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Invia per Email l'Avviso della Issue non Assegnato</p> </td> 
   <td> <p>Sponsor del progetto</p> </td> 
   <td> <p>Quando si aggiunge una Issue non assegnata, invia una Email allo sponsor del progetto.</p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un problema non assegnato viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
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
   <th>Destinatario</th> 
   <th>Descrizione</th> 
   <th> Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Notifica</td> 
   <td> <p>Notifica aggiunta</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Viene inviato un messaggio al Centro notifiche.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Documento</p> </td> 
   <td> <p>Annullamento richiesta documento</p> </td> 
   <td> <p>Utente a cui è richiesto il documento</p> </td> 
   <td> <p>Annulla una richiesta di caricamento documento da parte mia.</p> <p>Il richiedente del documento riceve una notifica e-mail quando viene annullata una richiesta di documento.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Avviso errore</p> </td> 
   <td> <p></p> </td> 
   <td> <p>È stato rilevato un errore che richiede la tua attenzione.</p> <p>Una notifica e-mail viene generata dopo che Workfront tenta di connettersi a un account POP. Dopo 25 tentativi, Workfront disattiva la connessione all’account POP per preservare le risorse e invia una notifica. </p> <p>La notifica e-mail viene inviata al proprietario del progetto, se l’e-mail POP è associata a una coda di richieste, o agli amministratori di Workfront, se l’account POP è associato alla funzione "Posta in arrivo" in Email Setup.
   </p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problema</p> </td> 
   <td> <p>Assegnazione problema</p> </td> 
   <td> <p>Proprietario risorsa</p> </td> 
   <td> <p>Quando si cambia l'incaricato di una Issue, invia una Email all'incaricato</p> <p>L’Assegnatario del problema riceve una notifica e-mail quando una modifica interessa un utente che gestisce.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Nuovo utente</p> </td> 
   <td> <p>Utente</p> </td> 
   <td> <p>Quando viene creato un nuovo utente in Workfront, invia un messaggio e-mail all’utente.</p> <p>Dopo la creazione del nuovo utente, l'utente riceve un invito e-mail, che notifica la creazione di un account Workfront e richiede di impostare la password.</p> <p>Durante la creazione di un nuovo utente, gli utenti possono selezionare l'opzione "Invia un'e-mail di invito a questa persona" (come descritto in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a><span style="font-weight: 400;">). Tuttavia, quando l'opzione "Nuovo utente all'utente" è attivata a livello globale, tutti i nuovi utenti ricevono l'invito tramite e-mail indipendentemente dal fatto che sia selezionata l'opzione "Invia un'e-mail di invito a questa persona".</span></p> </td> 
   <td> Inattiva </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Condivisione oggetto</p> </td> 
   <td> <p>Membri del team con cui è stato condiviso l'oggetto</p> </td> 
   <td> <p>Qualcuno condivide un oggetto con il mio team.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente</p> </td> 
   <td> <p>Condivisione oggetto</p> </td> 
   <td> <p>Utente con cui l'oggetto è stato condiviso</p> </td> 
   <td> <p>Qualcuno condivide un oggetto con me.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente Progetto</p> </td> 
   <td> <p>Aggiunta utente progetto</p> </td> 
   <td> <p>Proprietario risorsa</p> </td> 
   <td> <p>Una delle mie persone viene aggiunta a un progetto.</p> <p>Un manager riceve una notifica e-mail quando uno dei suoi referenti diretti viene aggiunto a un progetto.</p> <p>Gli utenti con una licenza Light o Review non ricevono una notifica.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>Progetto aggiunto a un portfolio o programma</p> </td> 
   <td> <p>Proprietario Portfolio o programma</p> </td> 
   <td> <p>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà.</p> </td> 
   <td> <p>Attivo (solo istantaneo)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività</p> </td> 
   <td> <p>Assegnazione attività</p> </td> 
   <td> <p>Proprietario risorsa</p> </td> 
   <td> <p>Una modifica nell'assegnazione di un'attività ha effetto su uno dei miei dipendenti.</p> <p>Il Manager dell'assegnatario dell'attività riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> </td> 
   <td> <p>Inattiva</p> </td> 
  </tr> 
  <tr> 
   <td> Progetto <br>Attività <br>Problema</td> 
   <td>Nuovo aggiornamento</td> 
   <td>Abbonato </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Viene inviata un'e-mail quando viene effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono abbonato.</span> </p> </td> 
   <td>Attivo (solo istantaneo)</td> 
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

| Tipo Oggetto | Evento | Destinatario | Descrizione | Stato predefinito |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Attività e problemi | Delega di attività e problemi | Assegnatario | Delego le mie attività e i miei problemi (conferma) | Attivo (solo istantaneo) |
| Attività e problemi | Revoca la delega di attività e problemi | Assegnatario | Revoco la delega delle mie attività e dei miei problemi (conferma) | Attivo (solo istantaneo) |
| Attività e problemi | Delega di attività e problemi | Delega | Qualcuno mi delega le sue attività e i suoi problemi | Attivo (solo istantaneo) |
| Attività e problemi | Revoca attività e delega problemi | Delega | Qualcuno mi revoca la delega delle sue attività e dei suoi problemi | Attivo (solo istantaneo) |

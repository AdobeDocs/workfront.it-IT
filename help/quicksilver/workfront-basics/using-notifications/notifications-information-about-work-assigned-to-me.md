---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni sul lavoro assegnato a me"
description: Le notifiche seguenti ti avvisano delle attività che si verificano su un elemento di lavoro assegnato.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 6%

---

# Notifiche: informazioni sul lavoro assegnato a me

Le notifiche seguenti ti avvisano delle attività che si verificano su un elemento di lavoro assegnato.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th> <p>Campi inclusi </p> <p> *Solo campi riepilogo giornalieri</p> </th> 
   <th>Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Un predecessore di un'attività assegnata al mio team è completato</strong> </p> <p>Il team assegnato riceve una notifica e-mail quando viene completato un predecessore di una delle sue attività. </p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Completato: &lt;task name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività predecessore<br>Progetto attività predecessore<br>Numero di riferimento attività predecessore<br>Nome dell'utente che ha completato l'attività predecessore<br>Stato dell'attività predecessore<br>Data e ora di completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>Vedi altri dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di predecessori completati<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </p> </td> 
   <td><strong>Giornaliera</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Il predecessore di una delle mie attività è stato completato</strong> </p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando viene completato un predecessore di una delle sue attività. </p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività predecessore<br>Progetto attività predecessore<br>Numero di riferimento attività predecessore<br>Nome dell'utente che ha completato l'attività predecessore<br>Stato dell'attività predecessore<br>Data e ora di completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di predecessori completati<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Un'attività che ho completato è stata approvata o respinta</strong> </p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando l’attività viene approvata o rifiutata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha concesso l’approvazione<br>Nuovo stato attività<br>Data e ora in cui l'attività è stata approvata o rifiutata<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni approvate o rifiutate<br>*Nome attività<br>*Nome dell'utente che ha approvato o rifiutato l'operazione<br>*Decisione di approvazione ([!UICONTROL Approvato]/ [!UICONTROL Rifiutato])<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Un'attività a cui sono assegnato è stata completata</strong> </p> <p>L’Assegnatario dell’attività riceve una notifica e-mail quando l’attività viene completata.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in [!UICONTROL Complete], l'oggetto dell'e-mail continua a essere visualizzato come "Complete" (Completato).</p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Tutti i predecessori di un'attività assegnata al mio team sono completati</strong> </p> <p>Quando un predecessore di una delle loro attività viene contrassegnato come completato, il team assegnato riceve una notifica e-mail.</p> <p>Gli utenti con una licenza Revisione o Richiedente non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Attività completata: &lt;name&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> Digest di lavoro assegnato a te &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Progetto attività<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività predecessore<br>Stato dell'attività predecessore<br>Data e ora di completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>Vedi altri dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </td>
   <td><strong>Istantanea</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Tutti i predecessori delle mie attività sono state completate</strong> </p> <p>L’assegnatario dell’attività riceve una notifica e-mail per ogni predecessore completato.</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em><br></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Progetto attività<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività predecessore<br>Stato dell'attività predecessore<br>Data e ora di completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Un problema che io risolvo è approvato o rifiutato</strong> </p> <p>L’assegnatario di un problema riceve una notifica e-mail quando viene presa una decisione di approvazione (approvata o rifiutata).</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Problema in attesa di approvazione: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> Digest di lavoro assegnato a te &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell’utente che ha approvato o rifiutato il problema<br>Decisione di approvazione (approvata o rifiutata)<br>Stato problema<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi approvati o rifiutati<br>*Nome problema<br>*Nome dell'utente che ha approvato o rifiutato il problema<br>*Decisione di approvazione (approvata o rifiutata)<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Un problema a cui sono stato assegnato è completo</strong> </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Completato: &lt;issue name=""&gt; il &lt;project name=""&gt;</em></p> <p><em> L’oggetto della notifica con riepilogo giornaliero è: Digest di lavoro assegnato a te &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell’utente che ha completato il problema<br>Nuovo stato problema<br>Data e ora in cui è stato completato il problema<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente che ha completato il problema<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>I documenti vengono caricati o modificati sulle richieste alle quali sono assegnato</strong> </p> <p>L’assegnatario del problema riceve una notifica e-mail quando i documenti vengono caricati o i dettagli del documento vengono modificati in relazione a un problema che ha aggiunto.</p> <p>Una notifica e-mail non viene inviata se l’utente che ha attivato il problema è l’assegnatario del problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e se il progetto è impostato come Help Request Queue (Coda di richieste di aiuto) (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richieste</a>).</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Documento aggiunto a] &lt;request name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome richiesta<br>Nome progetto (nome coda richieste)<br>Numero di riferimento del documento <br>Nome dell'utente che ha caricato il documento<br>Nome documento <br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>Anteprima [!UICONTROL]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti caricati o modificati<br>*Nome documento<br>*Nome oggetto<br>*Nome dell'utente che ha caricato il documento<br>*Data del riepilogo giornaliero</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche della data di scadenza su un'attività a cui sono assegnato</strong> </p> <p>L'assegnatario dell'attività riceve una notifica e-mail quando cambia la [!UICONTROL Planned Completion Date] dell'attività, a meno che l'utente che ha modificato la Planned Completion Date non sia anche l'assegnatario dell'attività.</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da [!UICONTROL Planning].</p> <p>Non viene inviata alcuna notifica relativa alle attività personali.</p> <p> Gli utenti con una licenza Revisione o Richiedente non ricevono una notifica. </p> <p> L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL La data di scadenza è stata modificata.]</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nuova data di scadenza ([!UICONTROL Data di completamento pianificata])<br>Data e ora in cui la data di scadenza è stata modificata<br>Nome dell'utente che ha modificato la data di scadenza<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in cui la data di scadenza (data di completamento pianificata) è cambiata<br>*Nome attività<br>*Nuova data di completamento pianificata<br>*Nome dell'utente che ha modificato la data di scadenza<br>*Data del riepilogo giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e ogni giorno</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche della data di scadenza su un problema al quale sono assegnato</strong> </p> <p>L'assegnatario del problema riceve una notifica e-mail quando [!UICONTROL Planned Completion Date] (Data di completamento pianificata) cambia, a meno che l'utente che ha modificato [!UICONTROL Planned Completion Date] non sia anche l'assegnatario.</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da [!UICONTROL Planning].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL La data di scadenza è stata modificata]</em></p> <p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nuova data di scadenza ([!UICONTROL Data di completamento pianificata])<br>Data e ora in cui la data di scadenza è stata modificata<br>Nome dell'utente che ha modificato la data di scadenza<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi in cui la data di scadenza ([!UICONTROL Planned Completion Date]) è cambiata<br>*Nome problema<br>*Nuova [!UICONTROL Data di completamento Pianificata]<br>*Nome dell'utente che ha modificato la data di scadenza<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e ogni giorno</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Modifica dello stato per un attività a cui sono stato assegnato</strong> <p>L’assegnatario dell’attività riceve una notifica e-mail quando lo stato dell’attività cambia, a meno che l’utente che ha modificato lo stato non sia anche l’assegnatario.</p> <p>Nota: questa notifica non viene inviata quando lo stato dell'attività cambia in completato. Per le attività completate viene utilizzata una notifica separata. Consulta <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Quando si completa un'attività, invia una Email all'incaricato</a>, sopra.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>&lt;task name=""&gt; da &lt;project name=""&gt; è &lt;new status=""&gt;</em></p> <p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora in cui lo stato è stato modificato<br>Stato anteprima<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni in cui lo stato è cambiato<br>*Nome attività<br>*Stato operazione precedente<br>*Nuovo stato operazione<br>*Nome dell'utente che ha cambiato lo stato<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifica dello stato di uno degli elementi del mio lavoro</strong> </p> <p>Ricevi una notifica e-mail quando lo stato cambia su un problema a cui sei assegnato, a meno che tu stesso non cambi lo stato. </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>&lt;issue name=""&gt; da &lt;project name=""&gt; è &lt;new status=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest del lavoro assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora in cui lo stato è stato modificato<br>Stato problema precedente<br><strong>Vedi altri dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi in cui lo stato è cambiato<br>*Nome attività<br>*Stato problema precedente<br>*Nuovo stato problema<br>*Nome dell'utente che ha cambiato lo stato<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Informazioni sul lavoro assegnato a me"
description: Le seguenti notifiche ti avvisano di attività che si verificano su un elemento di lavoro assegnato.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 39ba9e93a8597d4354472a19b1ac1c5f530f4398
workflow-type: tm+mt
source-wordcount: '2092'
ht-degree: 6%

---

# Notifiche: Informazioni sul lavoro assegnato

Le seguenti notifiche ti avvisano di attività che si verificano su un elemento di lavoro assegnato.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th> <p>Campi inclusi </p> <p> *Solo campi digeriti giornalieri</p> </th> 
   <th>Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Un predecessore di un'attività assegnata al mio team è completato</strong> </p> <p>Il team assegnato riceve una notifica e-mail quando viene completato un predecessore di una delle attività. </p> <p>Gli utenti con una licenza del richiedente di [!UICONTROL Review] o Re[!UICONTROL Requestor]non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Completa: &lt;task name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività predecessore<br>Progetto attività predecessore<br>Numero di riferimento attività predecessore<br>Nome dell’utente che ha completato l’attività predecessore<br>Stato dell'attività predecessore<br>Data e ora del completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di predecessori completati<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </p> </td> 
   <td><strong>Giornaliera</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Quando si completa un'attività, invia una Email a tutti gli incaricati di attività dipendenti</strong> </p> <p>L’assegnatario dell’attività riceve una notifica e-mail quando viene completato un predecessore di una delle attività. </p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività predecessore<br>Progetto attività predecessore<br>Numero di riferimento attività predecessore<br>Nome dell’utente che ha completato l’attività predecessore<br>Stato dell'attività predecessore<br>Data e ora del completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di predecessori completati<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </p> </td> 
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
   <td> <p><strong>Quando viene approvata o respinta un'Attività che va approvata, invia una Email all'incaricato</strong> </p> <p>L'assegnatario dell'attività riceve una notifica e-mail quando l'attività viene approvata o rifiutata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha concesso l’approvazione<br>Nuovo stato attività<br>Data e ora in cui l'attività è stata approvata o rifiutata<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni approvate o rifiutate<br>*Nome attività<br>*Nome dell'utente che ha approvato o rifiutato l'attività<br>*Decisione di approvazione ([!UICONTROL Approvato]/ [!UICONTROL Rifiutato])<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Quando si completa un'attività, invia una Email all'incaricato</strong> </p> <p>Al completamento dell’attività, l’Assegnatario dell’attività riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail continua a essere visualizzato come "Completato".</p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome del progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Data e ora del completamento dell’attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Tutti i predecessori di un'attività assegnata al mio team sono completati</strong> </p> <p>Il team assegnato riceve una notifica e-mail quando un predecessore di una delle attività viene contrassegnato come completato.</p> <p>Gli utenti con una licenza Revisore o Richiedente non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Attività completata: &lt;name&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> Digest di lavoro assegnato all'utente &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Progetto attività<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività predecessore<br>Stato dell'attività predecessore<br>Data e ora del completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </td>
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
   <td> <p><strong>Quando sono completate tutte le attività predecessori, invia una Email a tutti i principali utenti incaricati alle attività dipendenti</strong> </p> <p>L’assegnatario dell’attività riceve una notifica e-mail per ogni predecessore completato.</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt;</em><br></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Progetto attività<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività predecessore<br>Stato dell'attività predecessore<br>Data e ora del completamento del predecessore<br>Stato precedente dell'attività predecessore<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </td> 
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
   <td> <p><strong>Un problema che io risolvo è approvato o rifiutato</strong> </p> <p>L’assegnatario di un problema riceve una notifica e-mail quando viene presa una decisione di approvazione (approvata o rifiutata).</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Problema in attesa di approvazione: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> Digest di lavoro assegnato all'utente &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha approvato o rifiutato il problema<br>Decisione di approvazione (approvata o rifiutata)<br>Stato del problema<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi approvati o rifiutati<br>*Nome problema<br>*Nome dell'utente che ha approvato o rifiutato il problema<br>*Decisione di approvazione (approvata o rifiutata)<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Quando si completa una Issue, invia una Email all'incaricato</strong> </p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Completa: &lt;issue name=""&gt; su &lt;project name=""&gt;</em></p> <p><em> Oggetto della notifica giornaliera del riassunto: Digest di lavoro assegnato all'utente &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha completato il problema<br>Nuovo stato del problema<br>Data e ora di completamento del problema<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente che ha completato il problema<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>I documenti vengono caricati o modificati sulle richieste alle quali sono assegnato</strong> </p> <p>L’assegnatario del problema riceve una notifica e-mail quando i documenti vengono caricati o i dettagli del documento vengono modificati in un problema che ha aggiunto.</p> <p>Non viene inviata una notifica e-mail se l’utente che ha attivato il problema è l’assegnatario del problema.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] e se il progetto è impostato come coda di richiesta della Guida (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Documento aggiunto a] &lt;request name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome richiesta<br>Nome progetto (nome coda richieste)<br>Numero di riferimento documento <br>Nome dell’utente che ha caricato il documento<br>Nome documento <br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti caricati o modificati<br>*Nome documento<br>*Nome oggetto<br>*Nome dell'utente che ha caricato il documento<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche della data di scadenza su un'attività a cui sono assegnato</strong> </p> <p>L'Assegnatario dell'attività riceve una notifica e-mail quando cambia la [!UICONTROL Planned Completion Date] dell'attività, a meno che l'utente che ha modificato la Data di completamento pianificata non sia anche l'Assegnatario dell'attività.</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da [!UICONTROL Planning].</p> <p>Non viene inviata alcuna notifica relativa alle attività personali.</p> <p> Gli utenti con una licenza Revisore o Richiedente non ricevono una notifica. </p> <p> L’oggetto dell’e-mail di notifica istantanea è: <em>La data di scadenza è stata modificata.]</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nuova data di scadenza ([!UICONTROL Data di completamento pianificata])<br>Data e ora in cui è stata modificata la Data di scadenza<br>Nome dell'utente che ha modificato la data di scadenza<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in cui la data di scadenza (data di completamento pianificata) è cambiata<br>*Nome attività<br>*Nuova data di completamento pianificata<br>*Nome dell'utente che ha modificato la data di scadenza<br>*Data del digest giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche della data di scadenza su un problema al quale sono assegnato</strong> </p> <p>L’assegnatario del problema riceve una notifica e-mail quando cambia la [!UICONTROL Planned Completion Date] (Data completamento pianificata), a meno che l’assegnatario non sia l’utente che ha modificato la [!UICONTROL Planned Completion Date] (Data completamento pianificato).</p> <p>Viene inviata una notifica solo se lo stato del progetto è diverso da [!UICONTROL Planning].</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Data di scadenza è stata modificata]</em></p> <p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nuova data di scadenza ([!UICONTROL Data di completamento pianificata])<br>Data e ora in cui è stata modificata la data di scadenza<br>Nome dell’utente che ha modificato la data di scadenza<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi in cui è cambiata la data di scadenza ([!UICONTROL Pianificato data di completamento])<br>*Nome problema<br>*Nuova [!UICONTROL data di completamento pianificata]<br>*Nome dell'utente che ha modificato la data di scadenza<br>*Data del digest giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Le modifiche stato su un'attività a cui sono assegnato</strong> <p>L'Assegnatario dell'attività riceve una notifica e-mail quando lo stato dell'attività cambia, a meno che l'utente che ha modificato lo stato non sia anche l'assegnatario.</p> <p>Nota: Questa notifica non viene inviata quando lo stato dell'attività diventa completo. Per le attività completate viene utilizzata una notifica separata. Vedi <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Un'attività a cui sono assegnato viene completata</a>sopra.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;task name=""&gt; da &lt;project name=""&gt; è &lt;new status=""&gt;</em></p> <p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora della modifica dello stato<br>Stato anteprima<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni in cui lo stato è cambiato<br>*Nome attività<br>*Stato precedente attività<br>*Nuovo stato attività<br>*Nome dell'utente che ha modificato lo stato<br>*Data del digest giornaliero<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche dello stato su uno degli elementi del mio lavoro</strong> </p> <p>Ricevi una notifica e-mail quando lo stato cambia in un problema a cui sei assegnato, a meno che tu non cambi tu stesso lo stato. </p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>Gli utenti con una licenza [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono alcuna notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;issue name=""&gt; da &lt;project name=""&gt; è &lt;new status=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Work Assegnato a te] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora della modifica dello stato<br>Stato problema precedente<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi in cui lo stato è cambiato<br>*Nome attività<br>*Stato problema precedente<br>*Nuovo stato problema<br>*Nome dell'utente che ha modificato lo stato<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Richieste che ho fatto"
description: Le seguenti notifiche ti informano sulle richieste effettuate in Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# Notifiche: Richieste che ho presentato

Le seguenti notifiche ti informano sulle richieste effettuate in [!DNL Adobe Workfront].

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Richieste che ho inviato</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Completata una richiesta di approvazione documento</strong> </p> <p>L’utente che ha richiesto un’approvazione su un documento riceve una notifica e-mail al completamento della richiesta di approvazione del documento.</p> <p>L’oggetto dell’e-mail di notifica istantanea è:<em> &lt;approver name=""&gt; ha &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; presente documento.</em></p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </td> 
   <td> Nome documento<br>Nome approvatore </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documento modificato o caricato su un problema per il quale sono il contatto principale</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando un documento viene caricato o modificato sul problema, a meno che l'utente che ha caricato o modificato il documento non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se il progetto è configurato come coda di richiesta della Guida in linea (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Creare una coda di richiesta]</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Documento aggiunto a &lt;issue name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto: <em>Riepilogo delle richieste &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome oggetto in cui è stato caricato il documento<br>Nome oggetto padre<br>Numero di riferimento documento<br>Nome dell’utente che ha caricato il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti caricati<br>*Nome del documento<br>*Nome oggetto padre<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Richiesta di caricamento documento completata</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando viene soddisfatta una richiesta di caricamento del documento.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Richiesta documento da] &lt;user name=""&gt; è stato realizzato</em></p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </td> 
   <td> <p>Nome dell’utente che ha caricato il documento<br>Nome oggetto in cui è stato caricato il documento<br>Nome documento<br><br></p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività personale che ho assegnato a qualcun altro è completata</strong> </p> <p>Viene inviata una notifica all’utente che ha assegnato un’attività ad hoc a un altro utente al completamento di tale attività. </p> <p>Per ulteriori informazioni sulle attività ad hoc, consulta <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Creare elementi di lavoro dall'area [!UICONTROL Home]</a>.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Completamento attività: &lt;task name=""&gt;</em></p> <p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </p> </td> 
   <td> Nome attività<br>Nome progetto predefinito (Progetto personale dell’utente che ha ricevuto l’attività personale)<br>Numero di riferimento attività<br>Nome proprietario attività<br>Nuovo stato attività<br>Data e ora del completamento dell’attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br><br><br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa una Issue, invia una Email all'autore</strong> </p> <p>Il contatto principale su un problema riceve una notifica quando il problema viene completato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Completamento del problema: &lt;issue name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Riepilogo delle richieste &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha completato il problema<br>Nuovo stato<br>Data e ora del completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente che ha completato il problema<br>*Data del digest giornaliero </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue, invia una Email all'autore</strong> </p> <p>Il contatto principale su un problema riceve una notifica quando aggiunge un problema in un progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Problema inviato]: &lt;issue name=""&gt; su &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Riepilogo delle richieste &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome<br>Nome problema<br>Data di inserimento<br>Priorità del problema<br>Stato del problema<br>Assegnato al nome<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Data del digest giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Invio una richiesta (conferma)</strong> </p> <p>Il contatto principale sul problema riceve una notifica e-mail quando invia un problema.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] e se il progetto è impostato come Coda di richiesta della Guida in linea (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Creare una coda di richiesta]</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Richiesta inviata]: &lt;request name=""&gt; su &lt;project request="" queue="" name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Riepilogo delle richieste &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome progetto (nome coda richieste)<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome problema<br>Data di inserimento<br>Priorità del problema<br>Stato del problema<br>Assegnato al nome<br>Contatto principale<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di richieste inviate<br>*Nome richiesta<br>*Priorità richiesta<br>*Data del digest giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia richiesta è chiusa (conferma)</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando la richiesta viene chiusa.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e se il progetto è configurato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL La tua richiesta è stata chiusa]:"&lt;request name=""&gt;"</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento della richiesta<br>Nome dell’utente che ha chiuso la richiesta<br>Stato del problema<br>Data e ora di chiusura della richiesta<br>Stato della richiesta precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di richieste chiuse<br>*Nome richiesta<br>*Nome dell'utente che ha chiuso la richiesta<br>*Data del digest giornaliero </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno è assegnato alla mia richiesta</strong> </p> <p>Il contatto principale per il problema riceve una notifica e-mail quando un utente viene assegnato al problema, a meno che il contatto principale e l’utente assegnato siano lo stesso utente.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e se il progetto è configurato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Creare una coda di richiesta]</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL è stato assegnato alla tua richiesta]: "&lt;request name=""&gt;"</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome richiesta<br>Tipo di richiesta<br>Data di inserimento<br>Priorità del problema<br>Contatto principale<br>Data completamento pianificata<br>Stato del problema<br><strong>Vedi Maggiori dettagli</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di richieste assegnate<br>*Nome richiesta<br>*Assegnato al nome<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato del progetto, invia una Email all'utente che ha inserito il progetto</strong> </p> <p>L’utente che ha creato il progetto riceve una notifica e-mail quando cambia lo stato del progetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Modifica dello stato del progetto: &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora della modifica dello stato del progetto<br>Stato precedente del progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Nuovo stato progetto<br>*Nome dell'utente che ha modificato lo stato del progetto<br>*Data del digest giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche di stato cambia su mia richiesta</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando lo stato del problema cambia, a meno che l’utente che ha modificato lo stato non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Current e il progetto è impostato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Creare una coda di richiesta]</a>).</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;request name=""&gt; è &lt;new status=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Riepilogo delle richieste &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento della richiesta<br>Nome dell’utente che ha modificato lo stato della richiesta<br>Nuovo stato<br>Data e ora in cui è stato modificato lo stato della richiesta<br>Stato della richiesta precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di richieste con stato modificato<br>*Nome richiesta<br>*Stato richiesta precedente<br>*Nuovo stato della richiesta<br>*Nome dell'utente che ha modificato lo stato<br>*Data del digest giornaliero<br></td> 
   <td> <p><strong>Giornaliera</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

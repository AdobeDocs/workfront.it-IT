---
content-type: reference
navigation-topic: notifications
title: "Notifiche: richieste effettuate"
description: Le notifiche seguenti ti informano delle richieste effettuate in Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---

# Notifiche: richieste che ho effettuato

Le notifiche seguenti ti informano delle richieste che hai effettuato in [!DNL Adobe Workfront].

Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche evento](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Richieste effettuate</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Richiesta di approvazione documento completata</strong> </p> <p>L'utente che ha richiesto un'approvazione per un documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene completata.</p> <p>L'oggetto dell'e-mail di notifica immediata è:<em> &lt;Nome approvatore&gt; ha &lt;Decisione di approvazione ([!UICONTROL Approvato], [!UICONTROL Approvato con Modifiche], [!UICONTROL Rifiutato])&gt; questo documento.</em></p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </td> 
   <td> Nome documento<br>Nome approvatore </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un documento è stato modificato o caricato su un problema per il quale sono il contatto principale</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando un documento viene caricato o modificato sul problema, a meno che l’utente che ha caricato o modificato il documento non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se il progetto è configurato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Documento aggiunto a &lt;Nome problema&gt;</em></p> <p>L'oggetto della notifica del digest giornaliero è: <em>Digest of Your Requests &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> Nome oggetto in cui è stato caricato il documento<br>Nome oggetto padre<br>Numero di riferimento documento<br>Nome dell'utente che ha caricato il documento<br>Nome documento<br>Aggiunto in data<br>Dettagli documento (formato, dimensione, numero versione)<br>Miniatura documento<br><strong>[!Anteprima UICONTROL]</strong> e <strong>[!Download UICONTROL]</strong>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti caricati<br>*Nome documento<br>*Nome oggetto padre{1 6}*Nome dell'utente che ha aggiunto il documento<br>*Data del riepilogo giornaliero<br><br> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Richiesta di caricamento documento completata</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando viene soddisfatta una richiesta di caricamento del documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL La richiesta del documento da] &lt;Nome utente&gt; è stata soddisfatta</em></p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </td> 
   <td> <p>Nome dell'utente che ha caricato il documento<br>Nome oggetto in cui è stato caricato il documento<br>Nome documento<br><br></p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività personale che ho assegnato a qualcun altro è stata completata</strong> </p> <p>Viene inviata una notifica all’utente che ha assegnato un’attività ad hoc a un altro utente al completamento dell’attività. </p> <p>Per ulteriori informazioni sulle attività ad hoc, vedere <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Creare elementi di lavoro dall'area [!UICONTROL Home]</a>.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Completamento attività: &lt;Nome attività&gt;</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome attività<br>Nome progetto predefinito (progetto personale dell'utente che ha ricevuto l'attività personale)<br>Numero di riferimento attività<br>Nome proprietario attività<br>Nuovo stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br><br><br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problema per il quale sono il contatto principale è stato completato</strong> </p> <p>Il contatto principale per un problema riceve una notifica al completamento del problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Issue Completion]: &lt;Nome problema&gt;</em></p> <p>L'oggetto della notifica del digest giornaliero è:<em> Digest of your Requests &lt;Data del digest giornaliero&gt;</em></p> <p> </p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha completato il problema<br>Nuovo stato<br>Data e ora di completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente che ha completato il problema<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ho aggiunto un problema a un progetto</strong> </p> <p>Il contatto principale per un problema riceve una notifica quando aggiunge un problema in un progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Issue mitted]: &lt;Nome problema&gt; in &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica del digest giornaliero è:<em> Digest of your Requests &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome problema<br>Nome problema<br>Data immessa<br>Priorità problema<br>Stato problema<br>Assegnato al nome<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Data riepilogo giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Invio una richiesta (conferma)</strong> </p> <p>Il contatto principale sul problema riceve una notifica e-mail quando invia un problema.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e se il progetto è impostato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Richiesta inviata]: &lt;Nome richiesta&gt; nel nome &lt;Progetto (coda richieste)&gt;</em></p> <p>L'oggetto della notifica del digest giornaliero è:<em> Digest of your Requests &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> <p>Nome progetto (nome coda richieste)<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome problema<br>Data immessa<br>Priorità problema<br>Stato problema<br>Assegnato al nome<br>Contatto principale<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di richieste inviate<br>*Nome richiesta<br>*Priorità richiesta<br>*Data riepilogo giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia richiesta è chiusa (conferma)</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando la richiesta viene chiusa.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto è impostato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>).</p> <p>Oggetto dell'e-mail di notifica immediata: <em>[!UICONTROL La richiesta è stata chiusa]:"&lt;Nome richiesta&gt;"</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of your Requests] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento richiesta<br>Nome dell'utente che ha chiuso la richiesta<br>Stato problema<br>Data e ora di chiusura della richiesta<br>Stato richiesta precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di richieste chiuse<br>*Nome richiesta<br>*Nome dell'utente che ha chiuso la richiesta<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno è assegnato alla mia richiesta</strong> </p> <p>Il contatto principale per il problema riceve una notifica e-mail quando un utente viene assegnato al problema, a meno che il contatto principale e l’utente assegnato non siano lo stesso utente.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e se il progetto è impostato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome dell'utente assegnato alla richiesta&gt; [!UICONTROL è stato assegnato alla richiesta]: "&lt;Nome richiesta&gt;"</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of your Requests] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome richiesta<br>Tipo richiesta<br>Data immessa<br>Priorità problema<br>Contatto principale<br>Data di completamento pianificata<br>Stato problema<br><strong>Visualizza ulteriori dettagli</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di richieste assegnate<br>*Nome richiesta<br>*Assegnato al nome<br>*Data riepilogo giornaliero</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche di stato su un progetto creato</strong> </p> <p>L’utente che ha creato il progetto riceve una notifica e-mail quando lo stato del progetto cambia.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Project Status Change]: &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of your Requests] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha modificato lo stato<br>Nuovo stato<br>Data e ora di modifica dello stato del progetto<br>Stato progetto precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Nuovo stato progetto<br>*Nome dell'utente che ha modificato lo stato del progetto<br>*Data del riepilogo giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lo stato cambia su mia richiesta</strong> </p> <p>Il contatto principale del problema riceve una notifica e-mail quando lo stato del problema cambia, a meno che l’utente che ha modificato lo stato non sia anche il contatto principale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente e il progetto è impostato come [!UICONTROL Help Request Queue] (come descritto in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome richiesta&gt; è &lt;Nuovo stato&gt;</em></p> <p>L'oggetto della notifica del digest giornaliero è:<em> Digest of your Requests &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento richiesta<br>Nome dell'utente che ha modificato lo stato della richiesta<br>Nuovo stato<br>Data e ora di modifica dello stato della richiesta<br>Stato richiesta precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero riferimento progetto<br>*Numero totale di richieste il cui stato è cambiato<br>*Nome richiesta<br>*Stato richiesta precedente<br>*Nuovo stato richiesta<br>*Nome dell'utente che ha modificato lo stato<br>*Data del riepilogo giornaliero<br></td> 
   <td> <p><strong>Giornaliera</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Informazioni varie"
description: Le seguenti notifiche ti avvisano di attività che si verificano su un progetto che stai sponsorizzando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# Notifiche: Informazioni varie

Le seguenti notifiche ti avvisano di attività che si verificano su un progetto che stai sponsorizzando.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Non puoi abilitare o disabilitare le notifiche giornaliere e non ricevi e-mail digest giornaliere per gli eventi di questa categoria. Puoi abilitare o disabilitare le singole notifiche istantanee per [!UICONTROL Varie] categoria.

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
   <td> <p><strong>Viene inviato un messaggio al [!UICONTROL Announcement Center]</strong> </p> <p>Ricevi una notifica e-mail quando un nuovo messaggio è stato inviato al Centro annunci . </p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL [!DNL Adobe Workfront] Annuncio]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Oggetto dell'annuncio<br>Testo del messaggio incluso nell'annuncio<br>Documenti allegati<br>Nome dell’utente che ha inviato l’annuncio<br>Data e ora dell’invio dell’annuncio </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando viene cambiato l'incaricato primario di un'attività, invia una Email al Proprietario della risorsa</strong> </p> <p>Quando uno dei Rapporti diretti di un utente designato come manager viene assegnato a una nuova attività, il manager riceve un'e-mail sull'assegnazione. </p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Assegnazione risorsa attività: &lt;task name=""&gt;</em></p> </td> 
   <td>Nome progetto<br>Nome attività<br>Data e ora di creazione dell'attività<br>Nome dell’utente che ha creato l’attività<br>Nomi assegnazione<br>Data di scadenza (data di completamento pianificata)<br>Stato attività<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dopo aver ricevuto una richiesta di caricamento di un documento, la richiesta viene annullata</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando una richiesta di documento viene annullata.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; richiesta del documento annullata. </em></p> <p>Il seguente testo è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL non richiede più di caricare nulla riguardo alla richiesta ricevuta in precedenza. Volevamo solo farti sapere.]</em> </p> </td> 
   <td>Nome dell’utente che ha annullato la richiesta<br>Testo della richiesta di caricamento del documento originale<br>Banner "[!UICONTROL CANCELED]" sulla richiesta di documento originale<br>Data e ora della richiesta del documento originale<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato rilevato un errore che richiede la mia attenzione</strong> </p> <p>L’utente che risponde a un commento tramite e-mail riceve una notifica e-mail quando la risposta non viene recapitata.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Impossibile elaborare in] &lt;subject of="" original="" message=""&gt;</em></p> <p>Per informazioni sull’utilizzo dell’e-mail per rispondere ai commenti, consulta .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia l'incaricato di una Issue, invia una email al Proprietario della risorsa</strong> </p> <p>Il gestore di un utente assegnato a un problema riceve una notifica e-mail quando l’utente viene rimosso da o assegnato a un problema. </p> <p>Una notifica viene inviata solo se lo stato del progetto è Current o Planning.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Assegnazione problema: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell'utente che ha effettuato l'assegnazione<br>Tipo di problema<br>Nome dell’utente assegnato al problema<br>Data di emissione inserita<br>Priorità del problema<br>Contatto principale<br>Problema [!UICONTROL Data di completamento pianificata]<br>Stato del problema<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge un utente alla squadra di progetto, invia una Email al Proprietario della risorsa.</strong> </p> <p>Un manager riceve una notifica e-mail quando uno dei suoi utenti viene aggiunto a un progetto. Questa notifica viene inviata indipendentemente dallo stato del progetto. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail è: <em>Assegnazione progetto: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto la persona al progetto<br>Nome dell’utente aggiunto al progetto<br>Progetto [!UICONTROL Pianificazione della data di inizio]<br>Data completamento pianificato progetto [!UICONTROL]<br>Percentuale progetto completata<br>Nomi degli altri sul progetto<br>Stato del progetto<br>Proprietario progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br><br><br></p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà</strong> </p> <p>Il portfolio e/o il proprietario del programma ricevono una notifica quando un nuovo progetto viene aggiunto a un portfolio o a un programma.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Project aggiunto a] &lt;portfolio name=""&gt;[GUID progetto]</em></p> </td> 
   <td> Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto il progetto al portfolio/programma<br><br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con me</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno ti aggiunge all'elenco [!UICONTROL Sharing] di autorizzazioni su un oggetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Accesso concesso: &lt;object name=""&gt;</em></p> <p>Una notifica viene inviata solo se il progetto è in stato [!UICONTROL Current] (Corrente corrente).</p> </td> 
   <td> Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Accesso originale all'oggetto<br>Nuovo accesso concesso all'oggetto<br>Data e ora in cui è stato concesso l’accesso <br>Nome dell’utente che ha concesso l’accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con il mio team</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno aggiunge il tuo team all'elenco di condivisione delle autorizzazioni su un oggetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Accesso concesso: &lt;object name=""&gt; [GUID regola di accesso]</em></p> </td> 
   <td> Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Accesso precedente<br>Nuovo accesso<br>Data e ora in cui è stato concesso l’accesso<br>Nome del team<br>Nome dell’utente che ha concesso l’accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono iscritto</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno commenta un elemento a cui sei iscritto.</p> <p>L’oggetto del messaggio e-mail di abbonamento è: <em>[!UICONTROL È stato effettuato un aggiornamento al] &lt;object type=""&gt; ti sei iscritto a: &lt;object name=""&gt;</em></p> </td> 
   <td> Nome oggetto<br> Numero di riferimento oggetto<br> Nome dell’utente che ha fatto un commento sull’elemento iscritto<br> Data del commento<br> Commento aggiunto all’elemento iscritto  </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

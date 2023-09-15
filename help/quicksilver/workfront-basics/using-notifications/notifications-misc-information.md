---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni varie"
description: Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 8%

---

# Notifiche: informazioni varie

Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Non puoi abilitare o disabilitare le notifiche giornaliere e non ricevi e-mail di riepilogo giornaliero per gli eventi in questa categoria. Puoi abilitare o disabilitare singole notifiche istantanee per [!UICONTROL Varie] categoria.

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
   <td> <p><strong>Viene inviato un messaggio al Centro notifiche [!UICONTROL]</strong> </p> <p>Riceverai una notifica e-mail quando un nuovo messaggio viene inviato al [!UICONTROL Announcement Center]. </p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL [!DNL Adobe Workfront] Notifica]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Oggetto dell'annuncio<br>Testo del messaggio incluso nell’annuncio<br>Documenti allegati<br>Nome dell’utente che ha inviato la notifica<br>Data e ora di invio della notifica </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La modifica dell'assegnazione di un problema interessa una mia risorsa</strong> </p> <p>Quando uno dei referenti diretti di un utente designato come responsabile viene assegnato a una nuova attività, il responsabile riceve un'e-mail relativa all'assegnazione. </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Assegnazione risorsa attività]: &lt;task name=""&gt;</em></p> </td> 
   <td>Nome progetto<br>Nome attività<br>Data e ora di creazione dell'attività<br>Nome dell'utente che ha creato l'attività<br>Nomi assegnazioni<br>Data di scadenza (data di completamento pianificata)<br>Stato attività<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dopo aver ricevuto una richiesta di caricamento di un documento, la richiesta viene annullata</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando viene annullata una richiesta di documento.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; ha annullato la richiesta del documento. </em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL non ha più bisogno che tu carichi nulla in merito alla richiesta che hai ricevuto in precedenza. Volevamo solo che tu lo sapessi.]</em> </p> </td> 
   <td>Nome dell’utente che ha annullato la richiesta<br>Testo della richiesta di caricamento documento originale<br>Un banner "[!UICONTROL ANNULLATO]" sulla richiesta del documento originale<br>Data e ora della richiesta del documento originale<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato rilevato un errore che richiede la mia attenzione</strong> </p> <p>L’utente che risponde a un commento tramite e-mail riceve una notifica e-mail quando la risposta non viene consegnata.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Non è riuscito a elaborare su] &lt;subject of="" original="" message=""&gt;</em></p> <p>Per informazioni sull'utilizzo delle e-mail per rispondere ai commenti, vedere .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La modifica dell'assegnazione di un problema interessa una mia risorsa</strong> </p> <p>Il manager di un utente assegnato a un problema riceve una notifica e-mail quando l'utente viene rimosso o assegnato a un problema. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Assegnazione problema: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha effettuato l'assegnazione<br>Tipo di problema<br>Nome dell'utente assegnato al problema<br>Data problema immessa<br>Priorità problema<br>Contatto principale<br>Problema [!UICONTROL Planned Completion Date]<br>Stato problema<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una delle mie risrse viene aggiunta a un progetto</strong> </p> <p>Un manager riceve una notifica e-mail quando uno dei suoi utenti viene aggiunto a un progetto. Questa notifica viene inviata indipendentemente dallo stato del progetto. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail è: <em>Assegnazione progetto: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto la persona al progetto<br>Nome dell’utente aggiunto al progetto<br>Progetto [!UICONTROL Data Inizio Pianificata]<br>Progetto [!UICONTROL Data di completamento Pianificata]<br>Percentuale completamento progetto<br>Nomi di altri nel progetto<br>Stato progetto<br>Proprietario progetto<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br><br><br></p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà</strong> </p> <p>Il portfolio e/o il proprietario del programma ricevono una notifica quando un nuovo progetto viene aggiunto a un portfolio o a un programma.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Progetto aggiunto a] &lt;portfolio name=""&gt;[GUID progetto]</em></p> </td> 
   <td> Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto il progetto al portfolio/programma<br><br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con me</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno ti aggiunge all'elenco [!UICONTROL Sharing] di autorizzazioni su un oggetto.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Accesso [!UICONTROL Concesso]: &lt;object name=""&gt;</em></p> <p>Viene inviata una notifica solo se il progetto è nello stato [!UICONTROL Current].</p> </td> 
   <td> Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Accesso originale all'oggetto<br>Nuovo accesso concesso all'oggetto<br>Data e ora in cui è stato concesso l’accesso <br>Nome dell'utente che ha concesso l'accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con il mio team</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno aggiunge il tuo team all’elenco di condivisione delle autorizzazioni su un oggetto.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>Accesso [!UICONTROL Concesso]: &lt;object name=""&gt; [GUID regola di accesso]</em></p> </td> 
   <td> Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Accesso precedente<br>Nuovo accesso<br>Data e ora in cui è stato concesso l’accesso<br>Nome del team<br>Nome dell'utente che ha concesso l'accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono abbonato</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno commenta un elemento a cui sei abbonato.</p> <p>L’oggetto dell’e-mail di abbonamento è: <em>[!UICONTROL È stato effettuato un aggiornamento a] &lt;object type=""&gt; sei abbonato a: &lt;object name=""&gt;</em></p> </td> 
   <td> Nome oggetto<br> Numero di riferimento oggetto<br> Nome dell'utente che ha fatto un commento sull'elemento sottoscritto<br> Data in cui è stato fatto il commento<br> Commento aggiunto all'elemento sottoscritto  </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni varie"
description: Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# Notifiche: informazioni varie

Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.

Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vedi anche [Notifiche evento](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Non puoi abilitare o disabilitare le notifiche giornaliere e non ricevi e-mail di riepilogo giornaliero per gli eventi in questa categoria. Puoi abilitare o disabilitare singole notifiche istantanee per la categoria [!UICONTROL Varie].

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
   <td> <p><strong>Messaggio inviato al Centro notifiche [!UICONTROL]</strong> </p> <p>Riceverai una notifica e-mail quando un nuovo messaggio viene inviato al [!UICONTROL Announcement Center]. </p> <p>Oggetto dell'e-mail di notifica immediata: <em>[!UICONTROL [!DNL Adobe Workfront] notifica]: &lt;Oggetto della notifica&gt;</em></p> </td> 
   <td> Oggetto della notifica<br>Testo del messaggio incluso nella notifica<br>Documenti allegati<br>Nome dell'utente che ha inviato la notifica<br>Data e ora di invio della notifica </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una modifica dell'assegnazione di un'attività interessa uno dei miei contatti</strong> </p> <p>Quando uno dei referenti diretti di un utente designato come responsabile viene assegnato a una nuova attività, il responsabile riceve un'e-mail relativa all'assegnazione. </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Assegnazione risorsa attività]: &lt;Nome attività&gt;</em></p> </td> 
   <td>Nome progetto<br>Nome attività<br>Data e ora di creazione dell'attività<br>Nome dell'utente che ha creato l'attività<br>Nomi assegnazione<br>Data scadenza (data di completamento pianificata)<br>Stato attività<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dopo aver ricevuto una richiesta di caricamento documento, la richiesta è stata annullata</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando viene annullata una richiesta di documento.</p> <p>Oggetto dell'e-mail di notifica immediata: <em>&lt;Nome dell'utente che ha annullato la richiesta&gt; ha annullato la richiesta del documento. </em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;Nome&gt;, <br><br>&lt;Nome dell'utente che ha annullato la richiesta&gt;[!UICONTROL non ha più bisogno che tu carichi nulla in merito alla richiesta ricevuta in precedenza. Volevamo solo che tu lo sapessi.]</em> </p> </td> 
   <td>Nome dell'utente che ha annullato la richiesta<br>Testo della richiesta di caricamento documento originale<br>Banner "[!UICONTROL ANNULLATO]" sulla richiesta documento originale<br>Data e ora della richiesta documento originale<br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Errore che richiede la mia attenzione</strong> </p> <p>L’utente che risponde a un commento tramite e-mail riceve una notifica e-mail quando la risposta non viene consegnata.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Non è stato possibile elaborare su] &lt;oggetto del messaggio originale&gt;</em></p> <p>Per informazioni sull'utilizzo delle e-mail per rispondere ai commenti, vedere <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Risposta alle notifiche e-mail</a>.</p> </td>
   <td> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una modifica dell'assegnazione di un problema riguarda un utente</strong> </p> <p>Il manager di un utente assegnato a un problema riceve una notifica e-mail quando l'utente viene rimosso o assegnato a un problema. </p> <p>Viene inviata una notifica solo se lo stato del progetto è Corrente o Pianificazione.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Assegnazione problema: &lt;Nome problema&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha effettuato l'assegnazione<br>Tipo problema<br>Nome dell'utente assegnato al problema<br>Data problema inserita<br>Priorità problema<br>Contatto principale<br>Problema [!UICONTROL Data completamento pianificata]<br>Stato problema<br><strong>[!UICONTROL Visualizza ulteriori dettagli]</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un utente è stato aggiunto a un progetto</strong> </p> <p>Un manager riceve una notifica e-mail quando uno dei suoi utenti viene aggiunto a un progetto. Questa notifica viene inviata indipendentemente dallo stato del progetto. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L'oggetto dell'e-mail è: <em>Assegnazione progetto: &lt;Nome utente&gt;[&lt;GUID progetto&gt;_ &lt;GUID utente&gt;]</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha aggiunto la persona al progetto<br>Nome dell'utente che è stato aggiunto al progetto<br>Progetto [!UICONTROL Data inizio pianificata]<br>Progetto [!UICONTROL Data completamento pianificata]<br>Percentuale progetto completata<br>Nomi di altri utenti nel progetto<br>Stato progetto<br>Proprietario progetto<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br><br><br></p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno aggiunge un progetto a un portfolio o programma di mia proprietà</strong> </p> <p>Il portfolio e/o il proprietario del programma ricevono una notifica quando un nuovo progetto viene aggiunto a un portfolio o a un programma.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Progetto aggiunto a] &lt;Nome Portfolio&gt;[GUID progetto]</em></p> </td> 
   <td> Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha aggiunto il progetto al portfolio/programma<br><br></td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con me</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno ti aggiunge all'elenco [!UICONTROL Sharing] di autorizzazioni su un oggetto.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Accesso concesso]: &lt;Nome oggetto&gt;</em></p> <p>Viene inviata una notifica solo se il progetto è nello stato [!UICONTROL Current].</p> </td> 
   <td> Nome oggetto<br>Nome oggetto principale<br>Numero di riferimento oggetto<br>Accesso originale all'oggetto<br>Nuovo accesso concesso all'oggetto<br>Data e ora in cui è stato concesso l'accesso <br>Nome dell'utente che ha concesso l'accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno condivide un oggetto con il mio team</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno aggiunge il tuo team all’elenco di condivisione delle autorizzazioni su un oggetto.</p> <p>Oggetto dell'e-mail di notifica immediata: <em>[!UICONTROL Accesso concesso]: &lt;Nome oggetto&gt; [GUID regola di accesso]</em></p> </td> 
   <td> Nome oggetto<br>Nome oggetto principale<br>Numero di riferimento oggetto<br>Accesso precedente<br>Nuovo accesso<br>Data e ora di concessione dell'accesso<br>Nome del team<br>Nome dell'utente che ha concesso l'accesso </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato effettuato un aggiornamento a un'attività, un problema o un progetto a cui sono abbonato</strong> </p> <p>Ricevi una notifica e-mail quando qualcuno commenta un elemento a cui sei abbonato.</p> <p>L'oggetto dell'e-mail di sottoscrizione è: <em>[!UICONTROL È stato effettuato un aggiornamento a] &lt;Tipo di oggetto&gt; a cui si è iscritti: &lt;Nome oggetto&gt;</em></p> </td> 
   <td> Nome oggetto<br> Numero di riferimento oggetto<br> Nome dell'utente che ha aggiunto un commento all'elemento sottoscritto<br> Data di creazione del commento<br> Commento aggiunto all'elemento sottoscritto  </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

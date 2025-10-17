---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: comunicazione'
description: Le notifiche seguenti ti avvisano della comunicazione, ad esempio un commento di aggiornamento, che avviene su un elemento di lavoro a cui sei associato. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# Notifiche: comunicazione

Le notifiche seguenti ti avvisano della comunicazione, ad esempio un commento di aggiornamento, che avviene su un elemento di lavoro a cui sei associato. Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Queste notifiche ti avvisano di tutti i commenti che sono stati pubblicati su un elemento specifico. Per questo motivo, devi selezionare o deselezionare tutte le notifiche contemporaneamente per essere consegnate in un’e-mail di riepilogo giornaliero. Se desideri ricevere notifiche su determinati commenti solo nel momento in cui si verificano, puoi specificare le singole notifiche da inviare immediatamente.

Vedi anche [Notifiche evento](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>Qualcuno mi include in un aggiornamento diretto</strong> </p> <p>Un aggiornamento diretto si verifica quando un utente include in modo specifico un altro utente in un aggiornamento, come descritto in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag other on] aggiornamenti</a>.</p> <p>In questo caso, l’utente incluso nell’aggiornamento diretto riceve una notifica e-mail relativo all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo se l’utente dispone dei diritti di accesso all’oggetto.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome dell'utente che ti ha incluso nell'aggiornamento&gt; [!UICONTROL voleva che tu sapessi]</em></p> <p>L'oggetto della notifica del digest giornaliero è: <em>[!UICONTROL Digest of Communication] &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> Nome oggetto in cui è stato effettuato l'aggiornamento<br>Nome oggetto principale<br>Numero di riferimento oggetto<br>Nomi di tutti gli utenti e i team inclusi nell'aggiornamento diretto<br>Data e ora di esecuzione dell'aggiornamento<br>Testo dell'aggiornamento diretto<br><strong>[!UICONTROL Comment]</strong> pulsante<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni oggetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data del riepilogo giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha risposto alla mia richiesta</strong> </p> <p>Dopo che un utente invia una richiesta di lavoro e un altro utente risponde a tale richiesta, l’utente che ha inviato la richiesta riceve una notifica e-mail.</p> <p>Una notifica e-mail non viene inviata se:</p> 
    <ul> 
     <li> <p>L'utente che risponde è lo stesso utente che ha effettuato la richiesta</p> </li> 
     <li> <p>L’utente non ha accesso alla visualizzazione della nota</p> </li> 
    </ul><strong>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Comment on] &lt;Nome richiesta&gt; il &lt;Nome progetto&gt; (ref# &lt;Numero di riferimento richiesta&gt;)</em></strong> L'oggetto della notifica del digest giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del digest giornaliero&gt;</em></td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento<br>Nome dell'utente che ha risposto alla richiesta<br>Data e ora di creazione del commento<br>Testo del commento nella richiesta<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni richiesta<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato pubblicato un commento alla mia richiesta</strong> </p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta dell'helpdesk [!UICONTROL], a meno che l'utente che ha pubblicato il commento non sia anche il contatto principale per il problema.</p> <p>Anche tutti gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Comment on] &lt;Nome richiesta&gt; in &lt;Nome progetto&gt; (ref# &lt;Numero di riferimento richiesta&gt;)</em></p> <p>L'oggetto della notifica del riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome progetto<br>Numero di riferimento<br>Nome dell'utente che ha risposto alla richiesta<br>Data e ora di creazione del commento<br>Testo del commento nella richiesta<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni richiesta<br>*Nome progetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data del riepilogo giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un commento al mio documento</strong> </p> <p>Il proprietario di un documento in [!DNL Adobe Workfront] riceve una notifica e-mail quando un commento viene pubblicato sul documento, a meno che l'utente che ha pubblicato il commento non sia anche il proprietario del documento.</p> <p>Anche tutti gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current]. </p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Comment on] &lt;Nome richiesta&gt; in &lt;Nome progetto&gt; (ref# &lt;Numero di riferimento richiesta&gt;)</em></p> <p> L'oggetto della notifica del riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td>Nome documento<br>Nome progetto, attività o problema<br>Numero di riferimento<br>Nome dell'utente che ha risposto alla richiesta<br>Data e ora di creazione del commento<br>Testo del commento nel documento</td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha commentato un thread in cui sono presente</strong> </p> <p>I partecipanti al thread e gli utenti inclusi in un messaggio diretto ricevono una notifica e-mail quando un utente aggiunge un commento al thread.</p> <p>Gli utenti devono disporre dell'accesso [!UICONTROL View] per ricevere una notifica.</p> <p>I seguenti utenti non ricevono una notifica:</p> 
    <ul> 
     <li>Team inclusi in un messaggio diretto</li> 
     <li>Proprietario della nota</li> 
     <li>Il contatto principale</li> 
    </ul> <p><strong>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL RE: Comment on] &lt;Nome oggetto&gt;&lt;Tipo oggetto&gt; in &lt;Nome progetto&gt;(ref# &lt;Numero di riferimento oggetto&gt;</em>)</strong> </p> <p><strong> L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></strong> </p> </td> 
   <td> Nome oggetto<br>Nome oggetto principale<br>Nome dell'utente che ha aggiunto un commento al thread<br>Testo del commento nel thread<br>Data e ora di creazione del commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data riepilogo giornaliero </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha commentato uno dei miei elementi di lavoro</strong> </p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail ogni volta che un utente aggiunge un aggiornamento a un elemento di lavoro, a meno che l’utente che aggiunge l’aggiornamento non sia anche l’assegnatario. </p> <p>Quando un commento viene pubblicato su una richiesta, invia un’e-mail al contatto principale del problema.</p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta, a meno che l’utente che lo ha pubblicato non sia anche il contatto principale per il problema.</p> <p>Anche tutti gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Comment on] &lt;Nome elemento di lavoro&gt; in &lt;Nome progetto (ref# &lt;Numero di riferimento elemento di lavoro&gt;)</em></p> <p> L'oggetto della notifica del riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome elemento di lavoro<br>Nome progetto<br>Numero di riferimento elemento di lavoro<br>Nome dell'utente che ha commentato l'elemento di lavoro<br>Testo del commento sull'elemento di lavoro<br>Data e ora di creazione del commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno include il mio team in un aggiornamento diretto</strong> </p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag ad altri utenti negli aggiornamenti</a>.</p> <p>In questo caso, qualsiasi membro del team incluso nell’aggiornamento diretto riceve una notifica e-mail relativa all’aggiornamento.</p> <p>La notifica e-mail viene inviata solo agli utenti con diritti di accesso all’oggetto.</p> <p>Se l’utente che invia l’aggiornamento diretto è un membro del team incluso, l’utente che invia l’aggiornamento non riceve una notifica e-mail.</p> <p>L'oggetto dell'e-mail di notifica immediata è: [!UICONTROL Comment on] &lt;Nome oggetto&gt; on &lt;Nome oggetto padre&gt; (ref# &lt;Numero di riferimento oggetto&gt;)</p> <p> L'oggetto della notifica del riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome oggetto<br>Nome oggetto principale<br>Numero di riferimento oggetto<br>Nome dell'utente che ha eseguito l'aggiornamento diretto<br>Nome di tutti i team e gli utenti inclusi nell'aggiornamento diretto<br>Data e ora dell'aggiornamento diretto<br>Testo dell'aggiornamento diretto<br><strong>[!UICONTROL Comment]</strong> pulsante<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data del riepilogo giornaliero </p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge un commento all'utente</strong> </p> <p>È possibile aggiungere un commento a un utente nella scheda [!UICONTROL Aggiornamenti] dell'oggetto utente. È inoltre possibile aggiungere un commento a un utente quando si modificano le impostazioni dell'utente. L’utente contro cui viene inserito il commento riceve un’e-mail per informarlo di questo. </p> <p>Per immettere un aggiornamento nella scheda [!UICONTROL Updates] dell'utente, è necessario disporre delle autorizzazioni per almeno [!UICONTROL View]. Per modificare le impostazioni dell'utente, è necessario disporre delle autorizzazioni di [!UICONTROL Edit] per l'utente. </p> <p>Per ulteriori informazioni sull'inserimento di commenti sugli utenti nella scheda Aggiornamenti, vedere <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</p> <p>Per ulteriori informazioni sull'immissione di un commento su un utente quando si modificano le impostazioni dell'utente, vedere <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome utente&gt; [!UICONTROL voleva che tu sapessi]</em></p> <p>L'oggetto della notifica del riepilogo giornaliero è:<em> [!UICONTROL Digest of Communication] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome utente<br>Nome dell'utente che ha aggiunto il commento<br>Testo del commento<br>Data e ora di creazione del commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni oggetto<br>*<strong>[!UICONTROL Visualizza tutte le notifiche]</strong> pulsante<br>*Data riepilogo giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>

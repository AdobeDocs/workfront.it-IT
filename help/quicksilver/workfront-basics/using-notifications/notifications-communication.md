---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Comunicazione"
description: Le seguenti notifiche ti avvisano della comunicazione, ad esempio un commento di aggiornamento, che si verifica su un elemento di lavoro con cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta Attivare o disattivare le notifiche degli eventi personali.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 2af2a1f7d1a4d0b06cf4e7bfd2b9997ff8b9a6bf
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Notifiche: Comunicazione

Le seguenti notifiche ti avvisano della comunicazione, ad esempio un commento di aggiornamento, che si verifica su un elemento di lavoro con cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Queste notifiche ti avvisano di tutti i commenti che sono stati pubblicati su un elemento specifico. Per questo motivo, devi selezionare o deselezionare tutte le notifiche contemporaneamente da inviare in un messaggio e-mail digest giornaliero. Se desideri ricevere notifiche solo su determinati commenti nel momento in cui si verificano, puoi specificare che le singole notifiche devono essere inviate all’istante.

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
   <td> <p><strong>Qualcuno mi include in un aggiornamento diretto</strong> </p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Aggiornamenti di [!UICONTROL Assegna tag ad altri utenti]</a>.</p> <p>In questo caso, l’utente incluso nell’aggiornamento diretto riceve una notifica e-mail sull’aggiornamento.</p> <p>La notifica e-mail viene inviata solo se l’utente dispone dei diritti di accesso all’oggetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL volevo che sapessi]</em></p> <p>Oggetto della notifica giornaliera del riassunto: <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome dell’oggetto in cui è stato effettuato l’aggiornamento<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Nomi di tutti gli utenti e i team inclusi nell'aggiornamento diretto<br>Data e ora dell’aggiornamento<br>Testo dell'aggiornamento diretto<br><strong>[!UICONTROL Commento]</strong> pulsante<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha risposto alla mia richiesta</strong> </p> <p>Dopo che un utente invia una richiesta di lavoro e un altro utente risponde a tale richiesta di lavoro, l’utente che ha inviato la richiesta riceve una notifica e-mail.</p> <p>Una notifica e-mail non viene inviata se:</p> 
    <ul> 
     <li> <p>L’utente che risponde è lo stesso utente che ha effettuato la richiesta</p> </li> 
     <li> <p>L'utente non ha accesso per visualizzare la nota</p> </li> 
    </ul><strong>L’oggetto dell’e-mail di notifica istantanea è: <em>Commento su &lt;request name=""&gt; su &lt;project name=""&gt; (rif.# &lt;request reference="" number=""&gt;)</em></strong> Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Nome richiesta<br>Nome del progetto<br>Numero di riferimento<br>Nome dell’utente che ha risposto alla richiesta<br>Data e ora in cui è stato effettuato il commento<br>Testo del commento sulla richiesta<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni richiesta<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato pubblicato un commento alla mia richiesta</strong> </p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta di un help desk, a meno che l'utente che ha pubblicato il commento non sia anche il contatto principale per il problema.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Commento su &lt;request name=""&gt; su &lt;project name=""&gt; (rif.# &lt;request reference="" number=""&gt;)</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome richiesta<br>Nome del progetto<br>Numero di riferimento<br>Nome dell’utente che ha risposto alla richiesta<br>Data e ora in cui è stato effettuato il commento<br>Testo del commento sulla richiesta<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ogni richiesta<br>*Nome progetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un commento sul mio documento</strong> </p> <p>Il proprietario di un documento in [!DNL Adobe Workfront] riceve una notifica e-mail quando un commento viene pubblicato sul documento, a meno che l'utente che ha pubblicato il commento non sia anche il proprietario del documento.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current]. </p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Commento su &lt;request name=""&gt; su &lt;project name=""&gt; (rif.# &lt;request reference="" number=""&gt;)</em></p> <p> Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Nome documento<br>Nome progetto, attività o problema<br>Numero di riferimento<br>Nome dell’utente che ha risposto alla richiesta<br>Data e ora in cui è stato effettuato il commento<br>Testo del commento al documento</td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha commentato su un argomento che mi interessa</strong> </p> <p>I partecipanti al thread e gli utenti inclusi in un messaggio diretto ricevono una notifica e-mail quando un utente fa un commento nel thread.</p> <p>Per ricevere una notifica, gli utenti devono disporre dell’accesso a [!UICONTROL View] .</p> <p>I seguenti utenti non ricevono una notifica:</p> 
    <ul> 
     <li>Team inclusi in un messaggio diretto</li> 
     <li>Proprietario della nota</li> 
     <li>Contatto principale</li> 
    </ul> <p><strong>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL RE: Commento su] &lt;object name=""&gt;&lt;object type=""&gt; su &lt;project name=""&gt;(rif.# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Nome oggetto<br>Nome oggetto padre<br>Nome dell’utente che ha commentato il thread<br>Testo del commento sul thread<br>Data e ora in cui è stato effettuato il commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha commentato uno degli elementi del mio lavoro</strong> </p> <p>L'assegnatario dell'elemento di lavoro riceve una notifica e-mail ogni volta che un utente aggiunge un aggiornamento a un elemento di lavoro, a meno che l'utente che aggiunge l'aggiornamento non sia anche l'assegnatario. </p> <p>Quando un commento viene pubblicato su una richiesta, invia un'e-mail al contatto principale del problema.</p> <p>Il contatto principale per un problema riceve una notifica e-mail quando un commento viene pubblicato su una richiesta, a meno che l'utente che ha pubblicato il commento non sia anche il contatto principale per il problema.</p> <p>Anche gli utenti che sono inclusi direttamente nel commento ricevono una notifica e-mail.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Commento su &lt;work item="" name=""&gt; su &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome elemento di lavoro<br>Nome progetto<br>Numero di riferimento dell'elemento di lavoro<br>Nome dell’utente che ha commentato l’elemento di lavoro<br>Testo del commento sull’elemento di lavoro<br>Data e ora in cui è stato effettuato il commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno include il mio team in un aggiornamento diretto</strong> </p> <p>Un aggiornamento diretto si verifica quando un utente include specificatamente un altro utente in un aggiornamento, come descritto in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag agli altri utenti in caso di aggiornamenti</a>.</p> <p>In questo caso, qualsiasi membro del team incluso nell'aggiornamento diretto riceve una notifica e-mail sull'aggiornamento.</p> <p>La notifica e-mail viene inviata solo agli utenti che dispongono dei diritti di accesso all’oggetto.</p> <p>Se l’utente che invia l’aggiornamento diretto è membro del team incluso, l’utente che invia l’aggiornamento non riceve una notifica e-mail.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: Commento su &lt;object name=""&gt; su &lt;parent object="" name=""&gt; (rif.# &lt;object reference="" number=""&gt;)</p> <p> Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Nome dell'utente che ha effettuato l'aggiornamento diretto<br>Nome di tutti i team e gli utenti inclusi nell'aggiornamento diretto<br>Data e ora in cui è stato effettuato l'aggiornamento diretto<br>Testo dell'aggiornamento diretto<br><strong>[!UICONTROL Commento]</strong> pulsante<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*Nome progetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero </p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando un commento viene aggiunto sull'utente</strong> </p> <p>È possibile commentare un utente nella scheda [!UICONTROL Updates] dell’oggetto utente. Puoi anche fare un commento su un utente quando modifichi le impostazioni dell’utente. L'utente in cui viene effettuato il commento riceve un'e-mail per inviare loro il commento. </p> <p>Per inserire un aggiornamento nella scheda [!UICONTROL Updates] dell’utente, è necessario disporre delle autorizzazioni per almeno [!UICONTROL View] l’utente. Per modificare le impostazioni dell’utente, è necessario disporre di autorizzazioni di modifica per l’utente. </p> <p>Per ulteriori informazioni sull’esecuzione di commenti sugli utenti nella scheda Aggiornamenti, consulta <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a>.</p> <p>Per ulteriori informazioni sull'immissione di un commento su un utente quando si modificano le impostazioni dell'utente, consulta <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;user name=""&gt; [!UICONTROL volevo che sapessi]</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome utente<br>Nome dell’utente che ha aggiunto il commento<br>Testo del commento<br>Data e ora del commento<br>*Numero totale di commenti ricevuti<br>*Numero di commenti ricevuti per ciascun oggetto<br>*<strong>[!UICONTROL Vedi tutte le notifiche]</strong> pulsante<br>*Data del digest giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: informazioni sull’approvazione'
description: Le notifiche seguenti ti avvisano delle attività di approvazione che si verificano su un elemento di lavoro a cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Notifiche: informazioni sull’approvazione

Le notifiche seguenti ti avvisano delle attività di approvazione che si verificano su un elemento di lavoro a cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Una richiesta di approvazione del problema delegata è stata completata</strong> </p> <p>Un'approvazione del problema delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Approvazione/Rifiuto effettuato per conto dell'utente da] &lt;Nome utente&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Approval Information] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha approvato/rifiutato il problema a tuo nome<br>Decisione approvazione<br>Stato problema<br>Nome dell'utente che ha richiesto l'approvazione<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di approvazioni problemi delegate<br>*Nome problema<br>*Nome approvatore<br>*Data del riepilogo giornaliero<br><br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Richiesta di approvazione progetto delegata completata</strong> </p> <p>Un'approvazione di progetto delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Approvazione progetto/Rifiuto effettuato per conto dell'utente da] &lt;Nome utente&gt;</em></p> <p><em>L'oggetto della notifica del riepilogo giornaliero è: [!UICONTROL Digest of Approval Information] &lt;Data del riepilogo giornaliero&gt;</em> </p> </td> 
   <td> Nome progetto<br>[!UICONTROL Nome Portfolio]<br>[!UICONTROL Numero di riferimento progetto]<br>Nome dell'utente che ha approvato/rifiutato il progetto per tuo conto<br>[!UICONTROL Decisione di approvazione]<br>[!UICONTROL Stato progetto]<br>Nome dell'utente che ha richiesto l'approvazione<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Nome approvatore<br>[!UICONTROL *Data del riepilogo giornaliero]<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una richiesta di approvazione attività delegata è stata completata</strong> </p> <p>Un'approvazione dell'attività delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Approvazione attività/ Rifiuto effettuato per conto dell'utente] &lt;Nome utente&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Approval Information] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha approvato/rifiutato l'attività per tuo conto<br>Decisione di approvazione<br>Stato attività<br>Nome dell'utente che ha richiesto l'approvazione<br><strong>Ulteriori dettagli</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di approvazioni attività delegate<br>*Nome attività<br>*Nome approvatore<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Richiesta di approvazione documento annullata</strong> </p> <p>L’approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome utente&gt; [!UICONTROL ha annullato la richiesta di approvazione del documento]</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome dell'utente che ha annullato la richiesta di approvazione<br>[!UICONTROL Nome documento] </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono delegato come approvatore</strong> </p> <p>Se qualcuno ti ha delegato un'approvazione, riceverai una notifica e-mail. </p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Delegated] &lt;Tipo oggetto&gt; [!UICONTROL Approval - Please Review] &lt;Nome oggetto&gt;</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Nome dell'utente che ha inviato l'oggetto per l'approvazione<br>Nome dell'utente per conto del quale si sta approvando l'oggetto<br>Stato oggetto<br>Data e ora di richiesta dell'approvazione<br>Priorità oggetto<br>Nome passaggio approvazione<br>[!UICONTROL Planned Completion Date] dell'oggetto<br><strong>[!UICONTROL Make Approval Decision]</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia scheda orario è approvata</strong> </p> <p>Quando la scheda orario viene approvata, si riceve una notifica e-mail.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Timesheet Approved]: &lt;Data inizio scheda orario&gt; - &lt;Data fine scheda orario&gt;</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome dell'utente che ha approvato la scheda orario<br>Data e ora di approvazione della scheda orario<br>Stato della scheda orario ([!UICONTROL Approvato])<br>Data di inizio e data di fine della scheda orario<br>Ore totali registrate nella scheda orario<br>Ore di straordinario registrate nella scheda orario </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

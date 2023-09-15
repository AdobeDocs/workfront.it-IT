---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni sull’approvazione"
description: Le notifiche seguenti ti avvisano delle attività di approvazione che si verificano su un elemento di lavoro a cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 6%

---

# Notifiche: informazioni sull’approvazione

Le notifiche seguenti ti avvisano delle attività di approvazione che si verificano su un elemento di lavoro a cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Una richiesta di approvazione del problema delegato è stata completata</strong> </p> <p>Un'approvazione del problema delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Approvazione/Rifiuto del problema effettuato per conto dell'utente] &lt;user name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha approvato/rifiutato il problema per tuo conto<br>Decisione di approvazione<br>Stato problema<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di approvazioni di problemi delegate<br>*Nome problema<br>*Nome approvatore<br>*Data del riepilogo giornaliero<br><br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una richiesta di approvazione del progetto delegato è stata completata</strong> </p> <p>Un'approvazione di progetto delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Approvazione/Rifiuto del progetto effettuato per conto dell'utente da] &lt;user name=""&gt;</em></p> <p><em>L'oggetto della notifica di riepilogo giornaliero è: [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nome progetto<br>[!UICONTROL Nome Portfolio]<br>[!UICONTROL Numero di riferimento progetto]<br>Nome dell’utente che ha approvato/rifiutato il progetto per tuo conto<br>[!UICONTROL Decisione Approvazione]<br>[!UICONTROL Stato progetto]<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Nome approvatore<br>[!UICONTROL *Data del riepilogo giornaliero]<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una richiesta di approvazione dell'attività delegata è stata completata</strong> </p> <p>Un'approvazione dell'attività delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Approvazione/Rifiuto attività effettuato per conto dell'utente da] &lt;user name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha approvato/rifiutato l'attività per tuo conto<br>Decisione di approvazione<br>Stato attività<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>Vedi altri dettagli</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di approvazioni attività delegate<br>*Nome attività<br>*Nome approvatore<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Annullata una richiesta di approvazione documento</strong> </p> <p>L’approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>&lt;user name=""&gt; [!UICONTROL ha annullato la richiesta di approvazione documento]</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome dell’utente che ha annullato la richiesta di approvazione<br>[!UICONTROL Nome Documento] </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono delegato come approvatore</strong> </p> <p>Se qualcuno ti ha delegato un'approvazione, riceverai una notifica e-mail. </p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Delegato] &lt;object type=""&gt; [!UICONTROL Approval - Rivedi] &lt;object name=""&gt;</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> <p>[!UICONTROL Nome Oggetto]<br>Nome oggetto padre [!UICONTROL]<br>[!UICONTROL Object Reference Number]<br>Nome dell'utente che ha inviato l'oggetto per l'approvazione<br>Nome dell'utente per conto del quale si sta approvando l'oggetto<br>Stato oggetto<br>Data e ora in cui è stata richiesta l’approvazione<br>Priorità oggetto<br>Nome fase di approvazione<br>[!UICONTROL Planned Completion Date] (Data di completamento pianificata) dell'oggetto<br><strong>[!UICONTROL Prende La Decisione Di Approvazione]</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia scheda oraria è stata approvata</strong> </p> <p>Quando la scheda orario viene approvata, si riceve una notifica e-mail.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Timesheet Approved]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome dell’utente che ha approvato la scheda orario<br>Data e ora di approvazione della scheda orario<br>Stato della scheda orario ([!UICONTROL Approvato])<br>Data di inizio e data di fine della scheda orario<br>Ore totali registrate nella scheda orario<br>Le ore di straordinario registrate nella scheda orario </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

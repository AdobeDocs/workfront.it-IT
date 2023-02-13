---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Informazioni di approvazione"
description: Le seguenti notifiche ti avvisano di attività di approvazione in corso su un elemento di lavoro con cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta Attivare o disattivare le notifiche degli eventi personali.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Notifiche: Informazioni di omologazione

Le seguenti notifiche ti avvisano di attività di approvazione in corso su un elemento di lavoro con cui sei coinvolto. Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Una richiesta di approvazione del problema delegata è stata completata</strong> </p> <p>Un'approvazione del problema delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Rilascio approvazione/rifiuto effettuato per tuo conto da] &lt;user name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest delle informazioni di approvazione] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell'utente che ha approvato/rifiutato il problema per tuo conto<br>Decisione di approvazione<br>Stato del problema<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di omologazioni di emissioni delegate<br>*Nome problema<br>*Nome approvatore<br>*Data del digest giornaliero<br><br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una richiesta di approvazione del progetto delegata è stata completata</strong> </p> <p>Un'approvazione del progetto delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Approvazione/rifiuto del progetto effettuato per tuo conto da] &lt;user name=""&gt;</em></p> <p><em>Oggetto della notifica giornaliera del riassunto: [!UICONTROL Digest delle informazioni di approvazione] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nome progetto<br>[!UICONTROL Nome Portfolio]<br>[!UICONTROL Project Reference Number]<br>Nome dell’utente che ha approvato/rifiutato il progetto per suo conto<br>Decisione di approvazione<br>[!UICONTROL Stato del progetto]<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Nome approvatore<br>[!UICONTROL *Data del digest giornaliero]<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Una richiesta di approvazione dell'attività delegata è stata completata</strong> </p> <p>L'approvazione di un'attività delegata a un altro utente è stata approvata o rifiutata da tale utente.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Attività Approvazione / Rifiuto fatto per tuo conto da] &lt;user name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest delle informazioni di approvazione] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha approvato/rifiutato l'attività per suo conto<br>Decisione di approvazione<br>Stato attività<br>Nome dell’utente che ha richiesto l’approvazione<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Numero di riferimento progetto<br>*Nome progetto<br>*Numero totale di approvazioni dei compiti delegati<br>*Nome attività<br>*Nome approvatore<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Annullata una richiesta di approvazione documento</strong> </p> <p>L'approvatore del documento riceve una notifica e-mail quando la richiesta di approvazione del documento viene annullata.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>&lt;user name=""&gt; [!UICONTROL ha annullato la richiesta di approvazione del documento]</em></p> <p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </p> </td> 
   <td> Nome dell'utente che ha annullato la richiesta di approvazione<br>[!UICONTROL Document Name] </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono delegato come approvatore</strong> </p> <p>Se qualcuno ti ha delegato un'approvazione, riceverai una notifica e-mail. </p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Delegato] &lt;object type=""&gt; [!UICONTROL Approvazione - Rivedi] &lt;object name=""&gt;</em></p> <p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Nome Oggetto Padre]<br>[!UICONTROL Object Reference Number]<br>Nome dell'utente che ha inviato l'oggetto per l'approvazione<br>Nome dell’utente per conto del quale si sta approvando l’oggetto<br>Stato dell'oggetto<br>Data e ora della richiesta di approvazione<br>Priorità oggetto<br>Nome passaggio di approvazione<br>Data di completamento pianificata dell'oggetto<br><strong>Prendere decisioni di approvazione</strong> pulsante</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si approva e si chiude un Timesheet, invia una Email all'utente</strong> </p> <p>Quando la scheda attività viene approvata, viene inviata una notifica e-mail.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Scheda attività approvata]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Nota: Non puoi configurare questa notifica per un messaggio e-mail digest giornaliero.</p> </p> </td> 
   <td> Nome dell'utente che ha approvato la scheda attività<br>Data e ora dell'approvazione della scheda attività<br>Stato della scheda attività ([!UICONTROL approvato])<br>Data di inizio e data di fine della scheda attività<br>Totale ore registrate nella scheda attività<br>Ore di lavoro straordinario registrate nella scheda attività </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

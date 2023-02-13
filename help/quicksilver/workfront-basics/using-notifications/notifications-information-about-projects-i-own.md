---
content-type: reference
navigation-topic: notifications
title: '"Notifiche: Informazioni sui progetti che possiedo'
description: Le seguenti notifiche ti avvisano delle attività in corso su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, consulta Attivare o disattivare le notifiche degli eventi personali.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# Notifiche: Informazioni sui progetti che possiedo

Le seguenti notifiche ti avvisano delle attività in corso su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Quando si aggiunge un documento, invia una Email al Proprietario del progetto.</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che ha aggiunto il documento non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e il documento non è Privato.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Documento aggiunto a] &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività principale, invia una Email al Proprietario del progetto</strong> </p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail visualizza ancora "[!UICONTROL Complete]".</p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Nuovo stato attività<br>Data e ora del completamento dell’attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato di avanzamento di un progetto da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email al Proprietario del progetto.</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo. Un progetto è in ritardo quando lo stato di avanzamento è "[!UICONTROL A rischio]," "[!UICONTROL Behind]" o "[!UICONTROL In ritardo]".</p> <p>La best practice prevede l’attivazione di questa notifica. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Modifica dell’avanzamento del progetto: &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato di avanzamento del progetto<br>Progetto [!UICONTROL Pianificazione della data di inizio]<br>Data completamento pianificato progetto [!UICONTROL]<br>Data di inizio prevista del progetto<br>Data completamento progetto [!UICONTROL progetto]<br>Percentuale progetto completata<br>Stato del progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato avanzamento progetto<br>*Data del digest giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue, invia email al Proprietario del progetto</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Problema aggiunto a] &lt;project name=""&gt;</em></p> <p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato al nome <br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del digest giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività, invia una Email al Proprietario del progetto</strong> </p> <p>Il proprietario del progetto riceve una notifica al completamento di un'attività nel progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail visualizza ancora "[!UICONTROL Complete]".</p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività <br>Stato attività<br>Data e ora del completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate <br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato di avanzamento di un'attività da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email al Proprietario del progetto</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo. Un'attività è in ritardo quando lo stato di avanzamento è "[!UICONTROL A Rischio]" o "[!UICONTROL Behind]" o "[!UICONTROL In ritardo]".</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Modifica dell'avanzamento dell'attività: &lt;task name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nuovo stato di avanzamento attività<br>Attività [!UICONTROL Pianificazione della data di inizio]<br>Attività [!UICONTROL Pianificazione della data di completamento]<br>Attività [!UICONTROL Data inizio prevista]<br>Attività [!UICONTROL Data completamento previsto]<br>Percentuale attività completata<br>Stato attività<br>Assegnato al nome<br>Inserito per nome<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in ritardo rispetto alla pianificazione<br>*Nome attività<br>*Assegnato al nome<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa una Issue, invia una Email al Proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail al completamento di un problema relativo al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica. </p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;issue name=""&gt; su &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha completato il problema<br>Stato del problema<br>Data e ora del completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue non assegnata, invia una Email al Proprietario del progetto.</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema in] &lt;project name=""&gt;?</em></p> <p> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> Digest of Projects you own &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato a nome (vuoto)<br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del digest giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia il Proprietario del progetto, invia una Email al nuovo Proprietario</strong> </p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail.</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>Accendi questo perché viene assegnato a qualcosa. </p> <p> Assegnare qualcosa, condividere qualcosa, avere accesso a qualcosa.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Ora sei il proprietario del progetto di] &lt;project name=""&gt;</em></p> <p>Il seguente testo è incluso nel corpo della notifica e-mail:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL ti ha reso proprietario di] &lt;project name=""&gt;. In qualità di proprietario del progetto, potresti ricevere notifiche e-mail aggiuntive sull’attività del progetto, essere tenuto ad approvare le ore del progetto o essere coinvolto nell’approvazione del lavoro relativo al progetto. È tutto tuo.]</em> </p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Data completamento progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche della data di conferma per un'attività su uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando la data di commit cambia per un'attività del progetto, a meno che l'utente che ha modificato la data di commit sia anche il proprietario del progetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Data del commit per] &lt;task name=""&gt; [!UICONTROL è ora] &lt;new commit="" date=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> Digest of Projects you own &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha modificato la data di commit<br>Nuova data di conferma<br>Attività [!UICONTROL Pianificazione della data di completamento]<br>Informazioni su come la Timeline del progetto è interessata da questa modifica<br>Assegnato al nome<br>Inserito per nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività la cui data di commit è cambiata<br>*Nome attività<br>*Data del digest giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche della data di conferma per un problema su uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando la data di commit cambia per un problema del progetto, a meno che l’utente che modifica la data di commit sia lo stesso utente del proprietario del progetto.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Data del commit per] &lt;issue name=""&gt; [!UICONTROL è ora] &lt;new commit="" date=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto: <em> [!UICONTROL Digest of Projects you own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha modificato la data di commit<br>Nuova data di conferma<br>Data completamento pianificato problema<br>Assegnato al nome<br>Inserito per nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi la cui data di commit è cambiata<br>*Nome problema<br>*Data del digest giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>

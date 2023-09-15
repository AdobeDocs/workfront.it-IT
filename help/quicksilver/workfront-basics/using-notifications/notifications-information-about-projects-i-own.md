---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni sui progetti di mia proprietà"
description: Le notifiche seguenti ti avvisano delle attività che si svolgono su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 6%

---

# Notifiche: informazioni sui progetti di mia proprietà

Le notifiche seguenti ti avvisano delle attività che si svolgono su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Viene aggiunto un documento a un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che lo ha aggiunto non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e il documento non è Private.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Documento aggiunto a] &lt;project name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell'utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br><strong>Anteprima [!UICONTROL]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività principale è stata completata su un progetto di cui sono proprietario</strong> </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Nuovo stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progettodi mia proprietà è in ritardo</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo rispetto alla pianificazione. Un progetto è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]", "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>La best practice prevede di mantenere attiva questa notifica. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Cambio Avanzamento Progetto]: &lt;project name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato avanzamento progetto<br>Progetto [!UICONTROL Data Inizio Pianificata]<br>Progetto [!UICONTROL Data di completamento Pianificata]<br>Progetto [!UICONTROL Data Inizio Prevista]<br>Progetto [!UICONTROL Data di completamento Prevista]<br>Percentuale completamento progetto<br>Stato progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato avanzamento progetto<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene aggiunto un problema a un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Problema aggiunto a] &lt;project name=""&gt;</em></p> <p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data immessa<br>Priorità problema<br>Assegnato a Nome <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e ogni giorno</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività viene completata su un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica quando un'attività viene completata sul suo progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività <br>Stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate <br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività di mia proprietà è in ritardo</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione. Un'attività è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Cambio Avanzamento Attività]: &lt;task name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Stato di avanzamento nuova attività<br>Attività [!UICONTROL Data inizio pianificata]<br>Attività [!UICONTROL Data di completamento Pianificata]<br>Attività [!UICONTROL Data di inizio prevista]<br>Attività [!UICONTROL Data di completamento Prevista]<br>Percentuale completamento attività<br>Stato attività<br>Assegnato a Nome<br>Inserito per nome<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in ritardo sulla programmazione<br>*Nome attività<br>*Assegnato al nome<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problema è stato completato in un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene completato un problema relativo al proprio progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica. </p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; il &lt;project name=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell’utente che ha completato il problema<br>Stato problema<br>Data e ora in cui è stato completato il problema<br>Stato problema precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problema non assegnato viene aggiunto a un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Per chi deve essere assegnato a questo nuovo problema] &lt;project name=""&gt;?</em></p> <p> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> Digest di progetti di cui sei proprietario &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data immessa<br>Priorità problema<br>Assegnato a nome (vuoto)<br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e ogni giorno</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono nominato proprietario di un unovo progetto</strong> </p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail.</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>Attivate questa opzione perché sono assegnati a qualcosa. </p> <p> Assegnazione di qualcosa, condivisione di qualcosa, accesso a qualcosa.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Ora sei il proprietario del progetto di] &lt;project name=""&gt;</em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL ti ha reso proprietario di] &lt;project name=""&gt;. [!UICONTROL In qualità di proprietario del progetto, è possibile che tu riceva notifiche e-mail aggiuntive sull'attività del progetto, che ti venga richiesto di approvare le ore per il progetto o che tu venga coinvolto nell'approvazione di lavoro correlato al progetto. È tutto vostro.]</em> </p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Data di completamento Progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data del riepilogo giornaliero</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche della data di conferma per un'attività su uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un’attività del progetto, a meno che l’utente che ha modificato la data di conferma non sia anche il proprietario del progetto.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Data di conferma per] &lt;task name=""&gt; [!UICONTROL è ora] &lt;new commit="" date=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> Digest di progetti di cui sei proprietario &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha modificato la data di conferma<br>Nuova data di conferma<br>Attività [!UICONTROL Data di completamento Pianificata]<br>Informazioni su come la sequenza temporale del progetto è interessata da questa modifica<br>Assegnato a Nome<br>Inserito per nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività la cui data di conferma è stata modificata<br>*Nome attività<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche della data di conferma per un problema su uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un problema sul progetto, a meno che l’utente che modifica la data di conferma sia lo stesso del proprietario del progetto.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Data di conferma per] &lt;issue name=""&gt; [!UICONTROL è ora] &lt;new commit="" date=""&gt;</em></p> <p> L’oggetto della notifica con riepilogo giornaliero è: <em> [!UICONTROL Digest dei progetti di cui sei proprietario] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha modificato la data di conferma<br>Nuova data di conferma<br>Data di completamento problema pianificata<br>Assegnato a Nome<br>Inserito per nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi la cui data di conferma è stata modificata<br>*Nome problema<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>

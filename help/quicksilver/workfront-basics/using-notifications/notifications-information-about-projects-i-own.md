---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: informazioni sui progetti di mia proprietà'
description: Le notifiche seguenti ti avvisano delle attività che si svolgono su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 1%

---

# Notifiche: informazioni sui progetti di mia proprietà

Le notifiche seguenti ti avvisano delle attività che si svolgono su un progetto che possiedi. Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Un documento è stato aggiunto a un progetto di mia proprietà</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto, a meno che l’utente che lo ha aggiunto non sia anche il proprietario del progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e il documento non è Private.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Documento aggiunto a] &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto in data<br>Dettagli documento (formato, dimensione, numero di versione)<br><strong>[!UICONTROL Anteprima]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività milestone è stata completata in un progetto di mia proprietà</strong> </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Nuovo stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progettodi mia proprietà è in ritardo</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando il progetto è in ritardo rispetto alla pianificazione. Un progetto è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]", "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>La best practice prevede di mantenere attiva questa notifica. </p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>Oggetto dell'e-mail di notifica immediata: <em>[!UICONTROL Project Progress Change]: &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> <p>Portfolio Nome progetto<br>Nome progetto<br>Numero di riferimento progetto<br>Stato avanzamento progetto<br>Progetto [!UICONTROL Data inizio pianificata]<br>Progetto [!UICONTROL Data completamento pianificata]<br>Progetto [!UICONTROL Data inizio prevista]<br>Progetto [!UICONTROL Data completamento prevista]<br>Percentuale progetto completata<br>Stato progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero riferimento progetto<br>*Stato avanzamento progetto<br>*Data riepilogo giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene aggiunto un problema a un progetto di cui sono proprietario</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Issue aggiunto a] &lt;Nome progetto&gt;</em></p> <p> </p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Nome problema<br>Tipo problema<br>Data immessa<br>Priorità problema<br>Assegnato al nome <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data riepilogo giornaliero</p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività è stata completata in un progetto di mia proprietà</strong> </p> <p>Il proprietario del progetto riceve una notifica quando un'attività viene completata sul suo progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> </p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività <br>Stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate <br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività di un progetto di mia proprietà è indietro</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione. Un'attività è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Task Progress Change]: &lt;Nome attività&gt;</em></p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> Nome Attività<br>Nome Progetto<br>Numero Di Riferimento Attività<br>Stato Avanzamento Attività<br>Attività [!UICONTROL Data Inizio Pianificata]<br>Attività [!UICONTROL Data Completamento Pianificata]<br>Attività [!UICONTROL Data Inizio Prevista]<br>Attività [!UICONTROL Data Completamento Prevista]<br>Percentuale Attività Completata<br>Stato Attività<br>Assegnata Al Nome<br>Immessa Per Nome<br>*Nome Progetto<br>*Numero Riferimento Progetto<br>*Numero Totale Attività Indietro schedule<br>*Nome attività<br>*Nome assegnazione<br>*Data riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato completato un problema in un progetto di mia proprietà</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene completato un problema relativo al proprio progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica. </p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome problema&gt; in &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha completato il problema<br>Stato problema<br>Data e ora di completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un problema non assegnato a un progetto di mia proprietà</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando viene aggiunto al progetto un problema non assegnato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema il] &lt;Nome progetto&gt;?</em></p> <p> </p> <p> L'oggetto della notifica del riepilogo giornaliero è: <em> Digest di progetti di cui sei proprietario &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Nome problema<br>Tipo problema<br>Data immessa<br>Priorità problema<br>Assegnato a nome (vuoto)<br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono impostato come proprietario di un nuovo progetto</strong> </p> <p>Quando un utente viene assegnato come proprietario di un progetto, riceve una notifica e-mail.</p> <p>Se il proprietario del progetto è lo stesso utente che ha effettuato l'assegnazione, non viene inviata una notifica e-mail.</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>Attivate questa opzione perché sono assegnati a qualcosa. </p> <p> Assegnazione di qualcosa, condivisione di qualcosa, accesso a qualcosa.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Ora sei il proprietario del progetto di] &lt;Nome progetto&gt;</em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Nome&gt;,<br></em><em>&lt;Nome dell'utente che ti ha assegnato come proprietario del progetto&gt; [!UICONTROL ti ha reso proprietario di] &lt;Nome progetto&gt;. [!UICONTROL In qualità di proprietario del progetto, è possibile che tu riceva notifiche e-mail aggiuntive sull'attività del progetto, che ti venga richiesto di approvare le ore per il progetto o che tu venga coinvolto nell'approvazione di lavoro correlato al progetto. È tutto tuo.]</em> </p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> <p> </p> </td> 
   <td> <p>Portfolio Nome progetto<br>Nome progetto<br>Numero di riferimento progetto<br>Data di completamento progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data riepilogo giornaliera</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche alla data di conferma per un'attività in uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un’attività del progetto, a meno che l’utente che ha modificato la data di conferma non sia anche il proprietario del progetto.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Data commit per] &lt;Nome attività&gt; [!UICONTROL è ora] &lt;Data nuovo commit&gt;</em></p> <p> L'oggetto della notifica del riepilogo giornaliero è: <em> Digest di progetti di cui sei proprietario &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha modificato la data di conferma<br>Nuova data conferma<br>Attività [!UICONTROL Data completamento pianificata]<br>Informazioni su come la sequenza temporale del progetto è interessata da questa modifica<br>Assegnato al nome<br>Inserito dal nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero riferimento progetto<br>*Numero totale di attività la cui data conferma è cambiata<br>*Attività Nome<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modifiche alla data di conferma per un problema su uno dei miei progetti</strong> </p> <p>Il proprietario del progetto riceve una notifica e-mail quando cambia la data di conferma per un problema sul progetto, a meno che l’utente che modifica la data di conferma sia lo stesso del proprietario del progetto.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Data di conferma per] &lt;Nome problema&gt; [!UICONTROL è ora] &lt;Data nuovo commit&gt;</em></p> <p> L'oggetto della notifica del digest giornaliero è: <em> [!UICONTROL Digest of Projects You Own] &lt;Data del digest giornaliero&gt; </em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha modificato la data di conferma<br>Nuova data conferma<br>Data completamento problema pianificata<br>Assegnato al nome<br>Inserito per nome<br>Proprietario progetto<br><strong>[!UICONTROL Vedi ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi la cui data conferma è cambiata<br>*Nome problema<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>

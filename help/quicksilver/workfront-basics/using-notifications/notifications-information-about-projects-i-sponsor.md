---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: informazioni sui progetti di cui sono sponsor'
description: Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.
author: Courtney
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

---

# Notifiche: informazioni sui progetti di cui sono sponsor

Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.

Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Un documento è stato aggiunto a un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e se il documento non è [!UICONTROL Private].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Documento aggiunto a] &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento documento<br>Nome dell'utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto in data<br>Dettagli documento (formato, dimensione, numero versione)<br>Miniatura documento<br><strong>[!Anteprima UICONTROL]</strong> e <strong>[!Download UICONTROL]</strong>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data digest<br> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività milestone è stata completata in un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando completa un’attività cardine su un progetto di cui è sponsor.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".<br></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> Digest di progetti di cui si è sponsor &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Nuovo stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progetto che lo sponsor è in ritardo</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto è in ritardo. Un progetto è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In difficoltà]"."</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>Oggetto dell'e-mail di notifica immediata: <em>[!UICONTROL Project Progress Change]: &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Portfolio Nome progetto<br>Nome progetto<br>Numero di riferimento progetto<br>Stato avanzamento progetto<br>Progetto [!UICONTROL Data inizio pianificata]<br>Progetto [!UICONTROL Data completamento pianificata]<br>Progetto [!UICONTROL Data inizio prevista]<br>Progetto [!UICONTROL Data completamento prevista]<br>Percentuale progetto completata<br>Stato progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero riferimento progetto<br>*Stato avanzamento progetto<br>*Data riepilogo giornaliera </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività è stata completata in un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> </p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> Digest di progetti di cui si è sponsor &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Stato attività<br>Data e ora in cui lo stato dell'attività è stato modificato<br>Stato attività precedente<br><strong>Ulteriori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività su un progetto che sono sponsor è in ritardo</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione. Un'attività è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Task Progress Change]: &lt;Nome attività&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome Attività<br>Nome Progetto<br>Numero Di Riferimento Attività<br>Stato Avanzamento Attività<br>Attività [!UICONTROL Data Inizio Pianificata]<br>Attività [!UICONTROL Data Completamento Pianificata]<br>Attività [!UICONTROL Data Inizio Prevista]<br>Attività [!UICONTROL Data Completamento Prevista]<br>Percentuale Attività Completata<br>Stato Attività<br>Assegnata Al Nome<br>Immessa Per Nome<br>*Nome Progetto<br>*Numero Riferimento Progetto<br>*Numero Totale Attività Indietro schedule<br>*Nome attività<br>*Nome dell'utente che ha immesso l'attività<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un problema a un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Issue aggiunto a] &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Nome problema<br>Tipo problema<br>Data immessa<br>Priorità problema<br>Assegnato al nome <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero<br><br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato completato un problema in un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;Nome problema&gt; in &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> Digest di progetti di cui si è sponsor &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha completato il problema<br>Stato problema<br>Data e ora di completamento del problema<br>Stato problema precedente<br><strong>Ulteriori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>A un progetto di cui sono sponsor è stato aggiunto un problema non assegnato</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un problema non assegnato viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema il] &lt;Nome progetto&gt;?</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Nome problema<br>Tipo problema<br>Data immessa<br>Priorità problema<br>Assegnato a nome (vuoto)<br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono impostato come sponsor di un progetto</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene impostato come sponsor di un progetto.<br></p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Project Sponsor]: &lt;Nome progetto&gt;</em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;Nome Utente&gt;,</em> </p> <p><em>&lt;Nome dell'utente che ti ha assegnato come sponsor del progetto&gt; [!UICONTROL ti ha reso sponsor di] &lt;Nome del progetto&gt;. [!UICONTROL In qualità di sponsor del progetto, potresti ricevere notifiche e-mail aggiuntive sull'attività del progetto o potresti venire coinvolto nell'approvazione di lavoro correlato al progetto. Buon lavoro.]</em> </p> <p>L'oggetto della notifica del digest giornaliero è: <em>Digest di progetti di cui sei sponsor &lt;Data del digest giornaliero&gt;</em></p> </td> 
   <td> <p>Portfolio Nome progetto<br>Nome progetto<br>Numero di riferimento progetto<br>Data di completamento progetto pianificata<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data riepilogo giornaliera</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

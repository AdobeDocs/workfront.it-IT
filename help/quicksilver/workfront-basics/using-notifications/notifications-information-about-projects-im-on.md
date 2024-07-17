---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni sui progetti a cui collaboro"
description: Le notifiche seguenti ti avvisano delle attività che si verificano nei progetti su cui stai lavorando.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 0%

---

# Notifiche: informazioni sui progetti a cui collaboro

Le notifiche seguenti ti avvisano delle attività che si verificano nei progetti su cui stai lavorando.

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
   <td> <p><strong>Un documento è stato aggiunto a un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando un documento viene aggiunto al progetto, ad eccezione dell’utente che lo ha aggiunto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e il documento non è Private.</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Documento aggiunto a] &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è <em>[!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento documento<br>Nome dell'utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto in data<br>Dettagli documento (formato, dimensione, numero versione)<br>Miniatura documento<br><strong>[!Anteprima UICONTROL]</strong> e <strong>[!Download UICONTROL]</strong>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha caricato il documento<br>*Data riepilogo giornaliero<br> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività milestone è stata completata in un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica quando viene completata un'attività cardine del progetto. Le notifiche non vengono inviate al completamento di un'attività personale.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto è <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progetto a cui partecipo diventa attivo</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è impostato su [!UICONTROL Current].</p> <p>Nota: gli utenti devono essere elencati nella scheda Gestione del personale di un progetto per ricevere una notifica quando lo stato di un progetto è impostato su [!UICONTROL Current]. Per informazioni sull'aggiunta di utenti a un team di progetto, vedere <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gestione del team di progetto</a>.</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>&lt;Nome progetto&gt; [!UICONTROL è Corrente - Accedi al progetto e visualizza le attività!]</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Stato progetto<br>Progetto [!UICONTROL Data di completamento pianificata]<br>Proprietario progetto<br>Elenco di attività assegnate a te, a una delle tue mansioni o a uno dei tuoi team<br><strong>[!UICONTROL Vedi ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato progetto<br>*Data riepilogo giornaliera</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Un progetto in cui si trova il team diventa attivo</strong> <p>I membri di un team ricevono una notifica e-mail quando un progetto diventa attivo. Il team deve essere assegnato ad almeno un'attività per ricevere la notifica.</p><p>Se un singolo utente e un team sono entrambi assegnati a un’attività sul progetto. il team non riceverà alcuna notifica.</p><p>L'oggetto dell'e-mail di notifica immediata è <i>&lt;Nome progetto&gt; [!UICONTROL è attivo - Accedi al progetto e visualizza le attività!]</i></p><p>L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p></td> 
   <td>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Stato progetto<br>Progetto [!UICONTROL Data di completamento pianificata]<br>Proprietario progetto<br>Elenco di attività assegnate al team<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato progetto<br>*Data riepilogo giornaliera</td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progetto al quale collaboro è stato completato</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è [!UICONTROL Complete].</p> <p>Suggerimento: se i progetti vengono completati regolarmente, l’abilitazione di questa opzione può creare molti messaggi e-mail per gli utenti che hanno un numero limitato di attività su molti progetti.</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Project Status Change]: &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha completato il progetto<br>Stato progetto<br>Data e ora di completamento del progetto<br>Stato progetto precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato progetto<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività è stata completata in un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando un’attività viene completata sul loro progetto. <br>Per ulteriori informazioni sul team del progetto, vedere <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team del progetto</a>.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Complete]: &lt;Nome attività&gt; in &lt;Nome progetto&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> </p> <p><em> L'oggetto della notifica del riepilogo giornaliero è: [!UICONTROL Digest of Projects You're On] &lt;Data del riepilogo giornaliero&gt; </em> </p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Stato attività<br>Data e ora di modifica dello stato dell'attività<br>Stato attività precedente<br><strong>Ulteriori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del riepilogo giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un problema a un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Corrente.</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Issue aggiunto a] &lt;Nome progetto&gt;</em></p> <p> </p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Tipo problema<br>Nome problema<br>Data inserita<br>Priorità problema<br>Assegnato al nome <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data riepilogo giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato completato un problema in un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando viene completato un problema sul loro progetto.<br>Per ulteriori informazioni sul team del progetto, vedere <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team del progetto</a>.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Complete]: &lt;Nome problema&gt; in &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Nome dell'utente che ha completato il problema<br>Stato problema<br>Data e ora di completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>È stato aggiunto un problema non assegnato a un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema il] &lt;Nome progetto&gt;?</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell'utente che ha aggiunto il problema<br>Nome problema<br>Tipo problema<br>Data immessa<br>Priorità problema<br>Assegnato a nome (vuoto) <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono stato aggiunto a un progetto</strong> </p> <p>L’utente che è stato aggiunto al progetto riceve una notifica e-mail quando viene aggiunto, a meno che non si sia aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Sei stato aggiunto al progetto] &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ti ha aggiunto al progetto<br>Progetto [!UICONTROL Data inizio pianificata]<br>Progetto [!UICONTROL Data completamento pianificata]<br>Percentuale progetto completata<br>Nomi di altri utenti nel progetto <br>Proprietario progetto<br><strong>Ulteriori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data riepilogo giornaliera</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le modifiche di stato su un progetto al quale collaboro</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando lo stato del progetto cambia. <br>Per ulteriori informazioni sul team del progetto, vedere <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team del progetto</a>.</p> <p>L'oggetto dell'e-mail di notifica immediata è <em>[!UICONTROL Project Status Change]: &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è <em> [!UICONTROL Digest of Projects You're On] &lt;Data di riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha modificato lo stato del progetto<br>Nuovo stato progetto<br>Data e ora di modifica dello stato del progetto<br>Stato progetto precedente<br><strong>[!UICONTROL Ulteriori dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato progetto<br>*Data riepilogo giornaliera </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
 </tbody> 
</table>

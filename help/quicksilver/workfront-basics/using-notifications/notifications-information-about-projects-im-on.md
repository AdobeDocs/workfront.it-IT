---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Informazioni sui progetti su cui mi trovo"
description: Le seguenti notifiche ti avvisano delle attività che si verificano nei progetti su cui stai lavorando.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# Notifiche: Informazioni sui progetti su cui mi trovo

Le seguenti notifiche ti avvisano delle attività che si verificano nei progetti su cui stai lavorando.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Quando si aggiunge un documento, invia una Email alla squadra.</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando un documento viene aggiunto al progetto, fatta eccezione per l’utente che ha aggiunto il documento.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e il documento non è Privato.</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Documento aggiunto a] &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto è <em>[!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento documento<br>Nome dell’utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha caricato il documento<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività principale, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica al completamento di un’attività cardine sul progetto. Le notifiche non vengono inviate quando un’attività personale viene completata.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L'oggetto è <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Stato attività<br>Data e ora del completamento dell’attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato del progetto da Idea/Approvato/Richiesta/Pianificazione ad Attuale, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è impostato su [!UICONTROL Current].</p> <p>Nota: Gli utenti devono essere elencati nella scheda Gestione risorse di un progetto per ricevere una notifica quando lo stato di un progetto è impostato su [!UICONTROL Current]. Per informazioni sull’aggiunta di utenti a un team di progetto, consulta <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gestione del team del progetto</a>.</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>&lt;project name=""&gt; [!UICONTROL è attuale - Vai al tuo progetto e guarda le tue attività!]</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato del progetto<br>Data completamento pianificato progetto [!UICONTROL]<br>Proprietario progetto<br>Elenco delle attività assegnate a te, a uno dei tuoi ruoli o a uno dei tuoi team<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato del progetto<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Un progetto su cui lavora il team diventa attivo</strong> <p>I membri di un team ricevono una notifica e-mail quando un progetto diventa attivo. Il team deve essere assegnato ad almeno un'attività per ricevere la notifica.</p><p>Se un singolo utente e un team sono entrambi assegnati a un’attività del progetto. il team non riceverà una notifica.</p><p>L’oggetto dell’e-mail di notifica istantanea è <i>&lt;project name=""&gt; [!UICONTROL è attivo - Vai al tuo progetto e guarda le tue attività!]</i></p><p>Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato del progetto<br>Data completamento pianificato progetto [!UICONTROL]<br>Proprietario progetto<br>Elenco delle attività assegnate al team<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato del progetto<br>*Data del digest giornaliero</td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un progetto, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando lo stato del progetto è [!UICONTROL Complete].</p> <p>Suggerimento: Se i progetti vengono completati regolarmente, l’abilitazione di questa opzione consente di creare un sacco di e-mail per gli utenti che hanno un numero limitato di attività su molti progetti.</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>Modifica dello stato del progetto: &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha completato il progetto<br>Stato del progetto<br>Data e ora del completamento del progetto<br>Stato precedente del progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato del progetto<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando un’attività viene completata sul loro progetto. <br>Per ulteriori informazioni sul team del progetto, consulta <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team di progetto</a>.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail visualizza ancora "[!UICONTROL Complete]".</p> </p> <p><em> Oggetto della notifica giornaliera del riassunto: [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Stato attività<br>Data e ora in cui è stato modificato lo stato dell'attività<br>Stato attività precedente<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero<br></p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è Current.</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Problema aggiunto a] &lt;project name=""&gt;</em></p> <p> </p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Tipo di problema<br>Nome problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato al nome <br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del digest giornaliero </td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa una Issue, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail al completamento di un problema relativo al progetto.<br>Per ulteriori informazioni sul team del progetto, consulta <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team di progetto</a>.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Completato]: &lt;issue name=""&gt; su &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Nome dell’utente che ha completato il problema<br>Stato del problema<br>Data e ora del completamento del problema<br>Stato problema precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue non assegnata, invia una Email alla Squadra.</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema in] &lt;project name=""&gt;?</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato a nome (vuoto) <br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del digest giornaliero<br></td> 
   <td> <p><strong>Istantanea</strong> </p> <p><strong>e Giornaliero</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge un utente alla squadra di progetto, invia una Email all'utente</strong> </p> <p>L’utente aggiunto al progetto riceve una notifica e-mail quando viene aggiunto, a meno che l’utente non si sia aggiunto al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>[!UICONTROL Sei stato aggiunto al progetto] &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha aggiunto l’utente al progetto<br>Progetto [!UICONTROL Pianificazione della data di inizio]<br>Data completamento pianificato progetto [!UICONTROL]<br>Percentuale progetto completata<br>Nomi degli altri sul progetto <br>Proprietario progetto<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato del progetto, invia una Email alla squadra</strong> </p> <p>I membri di un team di progetto ricevono una notifica e-mail quando cambia lo stato del progetto. <br>Per ulteriori informazioni sul team del progetto, consulta <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team di progetto</a>.</p> <p>L’oggetto dell’e-mail di notifica istantanea è <em>Modifica dello stato del progetto: &lt;project name=""&gt;</em></p> <p> Oggetto della notifica giornaliera del riassunto è <em> [!UICONTROL Digest of Projects you are On] (Riepilogo dei progetti in corso) &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Nome dell’utente che ha modificato lo stato del progetto<br>Nuovo stato del progetto<br>Data e ora in cui lo stato del progetto è cambiato<br>Stato precedente del progetto<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato del progetto<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
 </tbody> 
</table>

---
content-type: reference
navigation-topic: notifications
title: "Notifiche: Informazioni sui progetti che sponsorizzo"
description: Le seguenti notifiche ti avvisano di attività che si verificano su un progetto che stai sponsorizzando.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1316'
ht-degree: 6%

---

# Notifiche: Informazioni sui progetti che sponsorizzo

Le seguenti notifiche ti avvisano di attività che si verificano su un progetto che stai sponsorizzando.

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
   <td> <p><strong>Quando si aggiunge un documento, invia una Email allo sponsor del Progetto.</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un documento al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] e se il documento non è [!UICONTROL Private].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Documento aggiunto a] &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Projects You Sponsor] (Digest dei progetti sponsorizzati) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento documento<br>Nome dell’utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>[!UICONTROL Preview]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività principale, invia una Email allo sponsor del progetto</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un’attività cardine viene completata su un progetto che gli sponsor.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail visualizza ancora "[!UICONTROL Complete]".<br></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Digest of Projects You Sponsor (Digest of Projects You Sponsor) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Nuovo stato attività<br>Data e ora del completamento dell’attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi Maggiori Dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato di avanzamento di un progetto da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email allo sponsor.</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto viene ritardato. Un progetto è in ritardo quando lo stato di avanzamento è "[!UICONTROL At Risk]" o "[!UICONTROL In Trouble]".</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Modifica dell’avanzamento del progetto: &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto: <em>[!UICONTROL Digest of Projects You Sponsor] (Digest dei progetti sponsorizzati) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato di avanzamento del progetto<br>Progetto [!UICONTROL Pianificazione della data di inizio]<br>Data completamento pianificato progetto [!UICONTROL]<br>Data di inizio prevista del progetto<br>Data completamento progetto [!UICONTROL progetto]<br>Percentuale progetto completata<br>Stato del progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato avanzamento progetto<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa un'attività, invia una Email allo sponsor del progetto</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;task name=""&gt; su &lt;project name=""&gt;</em></p> <p> <p>Nota: Se l’attività viene modificata in uno stato che equivale a [!UICONTROL Complete], l’oggetto dell’e-mail visualizza ancora "[!UICONTROL Complete]".</p> </p> <p>Oggetto della notifica giornaliera del riassunto:<em> Digest of Projects You Sponsor (Digest of Projects You Sponsor) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell’utente che ha completato l’attività<br>Stato attività<br>Data e ora in cui è stato modificato lo stato dell'attività<br>Stato attività precedente<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'attività<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo stato di avanzamento di un'attività da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email allo sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo. Un'attività è in ritardo quando lo stato di avanzamento è "[!UICONTROL A Rischio]" o "[!UICONTROL Behind]" o "[!UICONTROL In ritardo]".</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>Modifica dell'avanzamento dell'attività: &lt;task name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Projects You Sponsor] (Digest dei progetti sponsorizzati) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nuovo stato di avanzamento attività<br>Attività [!UICONTROL Pianificazione della data di inizio]<br>Attività [!UICONTROL Pianificazione della data di completamento]<br>Attività [!UICONTROL Data inizio prevista]<br>Attività [!UICONTROL Data completamento previsto]<br>Percentuale attività completata<br>Stato attività<br>Assegnato al nome<br>Inserito per nome<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in ritardo rispetto alla pianificazione<br>*Nome attività<br>*Nome dell'utente che è entrato nell'attività<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue, invia una Email allo sponsor del progetto.</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Problema aggiunto a] &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto: <em>[!UICONTROL Digest of Projects You Sponsor] (Digest dei progetti sponsorizzati) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato al nome <br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del digest giornaliero<br><br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si completa una Issue, invia una Email allo sponsor di Progetto</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Completato]: &lt;issue name=""&gt; su &lt;project name=""&gt;</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> Digest of Projects You Sponsor (Digest of Projects You Sponsor) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento del problema<br>Nome dell’utente che ha completato il problema<br>Stato del problema<br>Data e ora del completamento del problema<br>Stato problema precedente<br><strong>Vedi Maggiori dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del digest giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si aggiunge una Issue non assegnato, invia una Email allo sponsor del progetto.</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando al progetto viene aggiunto un problema non assegnato.</p> <p>Una notifica viene inviata solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Chi deve essere assegnato a questo nuovo problema in] &lt;project name=""&gt;?</em></p> <p>Oggetto della notifica giornaliera del riassunto:<em> [!UICONTROL Digest of Projects You Sponsor] (Digest dei progetti sponsorizzati) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data di inserimento<br>Priorità del problema<br>Assegnato a nome (vuoto)<br>Stato del problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del digest giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quando si cambia lo Sponsor, invia una Email al nuovo sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando è impostato come sponsor di un progetto.<br></p> <p>L’oggetto dell’e-mail di notifica istantanea è: <em>[!UICONTROL Project Sponsor]: &lt;project name=""&gt;</em></p> <p>Il seguente testo è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL ti ha fatto sponsor di] &lt;project name=""&gt;. In qualità di sponsor del progetto, potresti ricevere notifiche e-mail aggiuntive sull’attività del progetto o essere coinvolto nell’approvazione del lavoro relativo al progetto. Godetevi.]</em> </p> <p>Oggetto della notifica giornaliera del riassunto: <em>Digest of Projects You Sponsor (Digest of Projects You Sponsor) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Data completamento progetto pianificato<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data del digest giornaliero</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

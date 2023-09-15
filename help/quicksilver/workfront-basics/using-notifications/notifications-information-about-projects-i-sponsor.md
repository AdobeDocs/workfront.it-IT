---
content-type: reference
navigation-topic: notifications
title: "Notifiche: informazioni sui progetti di cui sono sponsor"
description: Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 6%

---

# Notifiche: informazioni sui progetti di cui sono sponsor

Le notifiche seguenti ti avvisano delle attività che si verificano su un progetto che stai sponsorizzando.

Per informazioni sulla configurazione delle notifiche ricevute, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Viene aggiunto un documento a un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un documento viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e se il documento non è [!UICONTROL Private].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Documento aggiunto a] &lt;project name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del documento<br>Nome dell'utente che ha aggiunto il documento<br>Nome documento<br>Aggiunto alla data<br>Dettagli documento (formato, dimensione, numero di versione)<br>Miniatura documento<br><strong>Anteprima [!UICONTROL]</strong> e <strong>[!UICONTROL Download]</strong> pulsanti<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di documenti aggiunti<br>*Nome documento<br>*Nome dell'utente che ha aggiunto il documento<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività principale viene completata in un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando completa un’attività cardine su un progetto di cui è sponsor.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".<br></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> Digest di progetti di cui sei sponsor &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Nuovo stato attività<br>Data e ora di completamento dell'attività<br>Stato attività precedente<br><strong>[!UICONTROL Vedi altri dettagli]</strong> pulsante <br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un progetto di cui sono sponsor è in ritardo</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando il progetto è in ritardo. Un progetto è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In difficoltà]"."</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Cambio Avanzamento Progetto]: &lt;project name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Stato avanzamento progetto<br>Progetto [!UICONTROL Data Inizio Pianificata]<br>Progetto [!UICONTROL Data di completamento Pianificata]<br>Progetto [!UICONTROL Data Inizio Prevista]<br>Progetto [!UICONTROL Data di completamento Prevista]<br>Percentuale completamento progetto<br>Stato progetto<br>Proprietario progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Stato avanzamento progetto<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attità viene completata su un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;task name=""&gt; il &lt;project name=""&gt;</em></p> <p> <p>Nota: se lo stato dell'attività viene modificato in modo da corrispondere a [!UICONTROL Complete], l'oggetto dell'e-mail visualizza comunque "[!UICONTROL Complete]".</p> </p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> Digest di progetti di cui sei sponsor &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha completato l'attività<br>Stato attività<br>Data e ora in cui lo stato dell'attività è stato modificato<br>Stato attività precedente<br><strong>Vedi altri dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di operazioni completate<br>*Nome attività<br>*Nome dell'utente che ha completato l'operazione<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un'attività su un progetto di cui sono sponsor è in ritardo</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un'attività del progetto è in ritardo rispetto alla pianificazione. Un'attività è in ritardo rispetto alla pianificazione quando lo stato di avanzamento è "[!UICONTROL A rischio]" o "[!UICONTROL In ritardo]" o "[!UICONTROL In ritardo]"."</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Cambio Avanzamento Attività]: &lt;task name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Stato di avanzamento nuova attività<br>Attività [!UICONTROL Data inizio pianificata]<br>Attività [!UICONTROL Data di completamento Pianificata]<br>Attività [!UICONTROL Data di inizio prevista]<br>Attività [!UICONTROL Data di completamento Prevista]<br>Percentuale completamento attività<br>Stato attività<br>Assegnato a Nome<br>Inserito per nome<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di attività in ritardo sulla programmazione<br>*Nome attività<br>*Nome dell'utente che ha inserito l'operazione<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene aggiunto un problema a un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene aggiunto un problema al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Problema aggiunto a] &lt;project name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è: <em>[!UICONTROL Digest of Projects You Sponsor] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data immessa<br>Priorità problema<br>Assegnato a Nome <br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti al progetto<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero<br><br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Viene completato un problema su un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; il &lt;project name=""&gt;</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> Digest di progetti di cui sei sponsor &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell’utente che ha completato il problema<br>Stato problema<br>Data e ora in cui è stato completato il problema<br>Stato problema precedente<br><strong>Vedi altri dettagli</strong> pulsante<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi completati<br>*Nome problema<br>*Nome dell'utente assegnato al problema<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problema non assegnato viene aggiunto a un progetto di cui sono sponsor</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando un problema non assegnato viene aggiunto al progetto.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] o [!UICONTROL Planning].</p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Per chi deve essere assegnato a questo nuovo problema] &lt;project name=""&gt;?</em></p> <p>L’oggetto della notifica con riepilogo giornaliero è:<em> [!UICONTROL Digest of Projects You Sponsor] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento problema<br>Nome dell’utente che ha aggiunto il problema<br>Nome problema<br>Tipo di problema<br>Data immessa<br>Priorità problema<br>Assegnato a nome (vuoto)<br>Stato problema<br>Contatto principale<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Numero totale di problemi aggiunti<br>*Nome problema<br>*Nome dell'utente che ha aggiunto il problema<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono scelto come sponsor di un progetto</strong> </p> <p>Lo sponsor del progetto riceve una notifica e-mail quando viene impostato come sponsor di un progetto.<br></p> <p>L’oggetto dell’e-mail di notifica immediata è: <em>[!UICONTROL Project Sponsor]: &lt;project name=""&gt;</em></p> <p>Il testo seguente è incluso nel corpo della notifica e-mail:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL ti ha reso sponsor di] &lt;project name=""&gt;. [!UICONTROL In qualità di sponsor del progetto, potresti ricevere notifiche e-mail aggiuntive sull'attività del progetto o potresti venire coinvolto nell'approvazione di lavoro correlato al progetto. Buon lavoro.]</em> </p> <p>L’oggetto della notifica con riepilogo giornaliero è: <em>Digest di progetti di cui sei sponsor &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento del progetto<br>Data di completamento pianificata del progetto<br>*Nome progetto<br>*Numero di riferimento progetto<br>*Data del riepilogo giornaliero</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

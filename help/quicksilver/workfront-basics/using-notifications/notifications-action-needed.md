---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: azione necessaria'
description: Le notifiche seguenti ti informano se è necessario intervenire su un elemento di lavoro. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# Notifiche: [!UICONTROL Azione richiesta]

Le notifiche seguenti ti informano se è necessario intervenire su un elemento di lavoro. Per informazioni sulla configurazione delle notifiche ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ricevo una nuova richiesta di lavoro</strong> </p> <p>L’assegnatario dell’elemento di lavoro riceve una notifica e-mail, a meno che l’utente che effettua la richiesta non sia anche l’assegnatario. </p> <p>Non viene inviata una notifica se lo stato dell'attività è [!UICONTROL Complete] o lo stato del problema è [!UICONTROL Closed].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL New Work Request]: &lt;nome richiesta&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è: <em>[!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome attività</p> <p>[!UICONTROL Data di completamento Pianificata]</p> <p>Principali</p> <p>Assegnazione di</p> <p>Assegnazione a</p> <p>[!UICONTROL Stato]</p> <p>[!UICONTROL Descrizione]</p> <p>Pulsante [!UICONTROL View]<br>Opzione da aggiungere al riepilogo giornaliero</p> <br> </td> 
   <td><strong>Istantanea e</strong> <strong>Giornaliera</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo approvare un documento</strong> </p> <p>L'approvatore di un documento riceve una notifica quando viene elencato come l'approvatore.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome dell'utente che ha inviato l'approvazione&gt; [!UICONTROL ti ha chiesto di approvare un documento in [!DNL Adobe Workfront].]</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Nome dell'utente che ha inviato l'approvazione<br>Nome documento<br>Numero di riferimento documento<br>Data e ora di richiesta approvazione<br>Dettagli documento (formato, dimensione, numero versione)<br><strong>[!UICONTROL Decidi l'approvazione]</strong> pulsante<br>*Numero totale di approvazioni documenti in sospeso<br>*Collegamento a <strong>[!UICONTROL Approvazioni documenti</strong>*<strong>Visualizza tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo approvare un progetto</strong> </p> <p>In caso di approvazioni dei ruoli, gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione '[!UICONTROL Approver non debba necessariamente trovarsi nel team di progetto (per i processi di approvazione che includono un ruolo)]' sia abilitata (come descritto in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p><strong>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con la mansione associata all'approvazione. </p> <p><strong>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con la mansione associata al processo di approvazione riceveranno una notifica e-mail.</p> <p>Se l’approvazione è associata a un utente, quest’ultimo riceve la notifica.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Progetto in attesa di approvazione]: &lt;Nome progetto&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è: <em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha inviato l'approvazione<br>Stato approvazione in sospeso<br>Data e ora di richiesta approvazione<br>Priorità progetto<br>Passaggio approvazione in attesa di approvazione<br>Numero di decisioni in attesa di approvazione<br>Nome approvatori (solo utenti)<br>[!UICONTROL Data completamento pianificato progetto] <br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante<br>*Numero totale di approvazioni progetto in sospeso <br>*Collegamento a <strong>[!UICONTROL Approvazioni progetto]</strong><br>*<strong>[!UICONTROL Visualizza tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero</p> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo approvare un'attività</strong> </p> <p>In caso di approvazioni dei ruoli, gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione '[!UICONTROL Approver non debba necessariamente trovarsi nel team di progetto (per i processi di approvazione che includono un ruolo)]' sia abilitata (come descritto in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>). </p> <p><strong>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con la mansione associata all'approvazione. </p> <p><strong>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con la mansione associata al processo di approvazione riceveranno una notifica e-mail.</p> <p>Se l’approvazione è associata a un utente, quest’ultimo riceve la notifica. </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Attività in attesa di approvazione]: &lt;Nome attività&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è: <em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> <p>Nome attività<br>Nome progetto<br>Nome dell'utente che ha inviato l'approvazione<br>Stato approvazione in sospeso<br>Data e ora di richiesta approvazione<br>Priorità attività<br>Nome fase approvazione<br>Nomi approvatori<br>[!UICONTROL Data completamento attività pianificata]<br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante<br>*Numero totale di approvazioni attività in sospeso<br>*Collegamento a<strong>[!UICONTROL Approvazioni attività *Vedi tutte le approvazioni]</strong> button<strong></strong>*Data del riepilogo giornaliero<br></p> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo approvare una scheda orario</strong> </p> <p>L'approvatore della scheda orario riceve una notifica e-mail quando viene inviata una scheda orario da approvare, a meno che l'utente che ha inviato la scheda non sia anche l'approvatore della scheda orario.</p> <p>Viene inviata una notifica solo se lo stato della scheda orario è [!UICONTROL Submitted].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Timesheet Submitted]: &lt;Proprietario scheda orario&gt;, &lt;Data inizio scheda orario&gt; - &lt;Data fine scheda orario&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è: <em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome dell'utente che ha inviato la scheda orario per l'approvazione<br>Data e ora di invio<br>Stato della scheda orario<br>Date di inizio e fine della scheda orario<br>Numero di ore registrate sulla scheda orario<br>Numero di ore di straordinario registrate sulla scheda orario<br><strong>[!UICONTROL Revisione]</strong> e <strong>[!UICONTROL Approva]</strong> pulsanti<br>*Numero totale di approvazioni della scheda orario in sospeso<br>*Collegamento a <strong>![ UICONTROL Scheda orario Approvazioni]</strong><br><strong>[!UICONTROL *Visualizza tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea e</strong> <strong>Giornaliera</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo approvare un problema</strong> </p> <p>In caso di approvazioni dei ruoli, gli utenti che ricevono una notifica e-mail per questo evento dipendono dal fatto che l'impostazione '[!UICONTROL Approver non deve necessariamente trovarsi nel team di progetto (per i processi di approvazione che includono un ruolo)]' sia abilitata (come descritto in <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval] settings</a>). </p> <p><strong>Se questa opzione è abilitata</strong>, viene inviata una notifica e-mail a tutti gli utenti del sistema con la mansione associata all'approvazione. </p> <p><strong>Se questa opzione è disabilitata</strong>, solo i membri del team di progetto con la mansione associata al processo di approvazione riceveranno una notifica e-mail.</p> <p>Se l’approvazione è associata a un utente, quest’ultimo riceve la notifica. </p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Problema in attesa di approvazione]: &lt;Nome problema&gt;</em></p> <p> L'oggetto della notifica di riepilogo giornaliero è: <em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt; </em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha inviato il problema per l'approvazione<br>Stato approvazione in sospeso<br>Data e ora della richiesta di approvazione<br>Priorità problema<br>Fase approvazione<br>Nomi degli approvatori<br>[!UICONTROL Data completamento problema pianificato]<br>[!UICONTROL Contatto principale]<br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante<br>*Numero totale di approvazioni problema in sospeso<br>*Collegamento a <strong>[!UICONTROL Approvazioni problemi]</strong><br><strong>[!UICONTROL *Visualizza tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea e</strong> <strong>Giornaliera</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo rivedere l'approvazione di un progetto per il quale ho una delega</strong> </p> <p>Ti è stata delegata l’approvazione di un progetto, che devi quindi rivedere.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Delegated Project Approval - Please Review] &lt;Nome progetto&gt;</em></p> <p><em>L'oggetto della notifica di riepilogo giornaliero è: [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em> </p> </td> 
   <td> Nome progetto<br>Nome Portfolio<br>Numero di riferimento progetto<br>Nome dell'utente che ha richiesto l'approvazione<br>Nome dell'utente per conto del quale si sta approvando il progetto<br>Stato approvazione in sospeso<br>Data e ora di approvazione richiesta<br>Priorità progetto<br>Passaggio approvazione<br>Nomi approvatori<br>[!UICONTROL Data completamento pianificato progetto]<br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante<br>*Numero totale di approvazioni progetto in sospeso<br>*Collegamento a <strong>[!UICONTROL Approvazioni progetto *Visualizza tutte le approvazioni]</strong> pulsante <br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo rivedere l'approvazione di un'attività per la quale ho una delega</strong> </p> <p>È stata delegata l'approvazione di un'attività ed è necessario rivederla.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Delegated Task Approval - Please Review ]&lt;Nome attività&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente che ha richiesto l'approvazione<br>Nome dell'utente per conto del quale si sta approvando l'attività<br>Stato approvazione in sospeso<br>Data e ora approvazione richiesta<br>Priorità attività<br>Fase approvazione<br>Nomi approvatori<br>[!UICONTROL Data completamento attività pianificata]<br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante <br>*Numero totale di approvazioni attività in sospeso<br>*Collegamento a <strong>[!UICONTROL Approvazioni attività *Vedi tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Devo rivedere l'approvazione di un problema per il quale ho una delega</strong> </p> <p>Hai ricevuto una delega per l'approvazione di un problema ed è necessario rivederla.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;Nome problema&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome problema<br>Nome progetto<br>Numero di riferimento problema<br>Nome dell'utente che ha richiesto l'approvazione<br>Nome dell'utente a nome del quale si sta approvando il problema<br>Stato approvazione in sospeso<br>Data e ora di approvazione richiesta<br>Priorità problema<br>Fase approvazione<br>Nomi degli approvatori<br>Data completamento problema pianificato<br>Contatto principale<br><strong>[!UICONTROL Decisione approvazione]</strong> pulsante<br>*Numero totale di approvazioni problema in sospeso<br>*Collegamento a <strong>[!UICONTROL Approvazioni problemi]</strong><br><strong>[!UICONTROL *Visualizza tutte le approvazioni]</strong> pulsante<br>*Data del riepilogo giornaliero<br></td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono assegnato a un problema</strong> </p> <p>L’assegnatario del problema riceve una notifica e-mail. L'assegnatario del problema non riceve un'e-mail se lo stato del problema è o è uguale a [!UICONTROL Closed].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL New Work Request]: &lt;Nome problema&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome problema<br>Nome progetto<br>[!UICONTROL Numero di riferimento problema]<br>Nome<br>Data scadenza problema ([!UICONTROL Data di completamento pianificata])<br>Nome dell'utente che ha assegnato il problema a te<br><strong>[!UICONTROL Lavoraci]</strong> pulsante<br>*Numero totale di assegnazioni<br>*Numero totale di attività e problemi assegnati a te<br>*Collegamento a <strong>[!UICONTROL Richieste di lavoro]</strong><br>*Data del riepilogo giornaliero<br></p> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sono impostato come assegnatario principale di un'attività</strong> </p> <p>L'assegnatario dell'attività riceve una notifica e-mail se viene nominato assegnatario principale dell'attività, a meno che l'assegnatario non sia l'utente che ha effettuato l'assegnazione.</p> <p>Viene inviata una notifica se lo stato del progetto è [!UICONTROL Current] e l'attività non è contrassegnata [!UICONTROL Complete].</p> <p>Gli utenti con una licenza di [!UICONTROL Review] o [!UICONTROL Requestor] non ricevono una notifica.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL New Work Request]: &lt;Nome attività&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> Nome attività<br>Nome progetto<br>Numero di riferimento attività<br>Nome dell'utente<br>Data di scadenza attività ([!UICONTROL Data di completamento pianificata])<br>Nome dell'utente che ha assegnato l'attività all'utente<br><strong>[!UICONTROL Lavoraci]</strong>*Numero totale di attività e problemi assegnati<br>*Collegamento a <br>[!UICONTROL Richieste di lavoro]<strong>*Data del riepilogo giornaliero</strong> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Il mio team riceve una nuova richiesta di lavoro</strong> </p> <p>I membri del team ricevono una notifica e-mail quando ricevono una nuova richiesta di lavoro. L’utente che ha inviato la richiesta non riceve una notifica se è membro del team.</p> <p>Viene inviata una notifica solo se lo stato del progetto è [!UICONTROL Current] e lo stato della richiesta di lavoro è [!UICONTROL New].</p> <p>Gli utenti con una licenza [!UICONTROL Review] non ricevono una notifica.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL New Work Request]: &lt;nome richiesta&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è: <em>[!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p> Nome problema<br>Nome progetto (nome coda richieste)<br>Numero di riferimento problema<br>Nome team<br>Data scadenza problema (data di completamento pianificata)<br>Nome dell'utente che ha inviato la richiesta<br><strong>[!UICONTROL Lavoraci]</strong> pulsante<br>*Numero totale di richieste assegnate al team</p> <p>*Nome richiesta di lavoro</p> <p>[!UICONTROL *Data di completamento pianificata]</p> <p>*Nome dell'utente che ha inviato la richiesta<br>*Collegamento a <strong>[!UICONTROL Richieste team]</strong><br>*Data del riepilogo giornaliero </p> <p><span class="preview">*Assegnazioni team</span> </p> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia scheda orario è stata riaperta</strong> </p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene riaperta, a meno che l’utente che ha riaperto la scheda non sia anche il proprietario della scheda orario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è [!UICONTROL Open].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Timesheet Reopen]: &lt;Data inizio scheda orario&gt; - &lt;Data fine scheda orario&gt;</em></p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </td> 
   <td> Nome dell'utente che ha riaperto la scheda orario<br>Data e ora di riapertura della scheda orario<br>Stato della scheda orario ([!UICONTROL riaperto])<br>Numero di ore totali registrate sulla scheda orario<br>Numero di ore di straordinario registrate sulla scheda orario<br><strong>[!UICONTROL revisione]</strong> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La mia scheda orario è rifiutata</strong> </p> <p>Il proprietario della scheda orario riceve una notifica e-mail quando la scheda viene rifiutata, a meno che l’utente che ha rifiutato la scheda orario non sia anche il proprietario.</p> <p>Una notifica e-mail viene inviata solo se lo stato della scheda orario è [!UICONTROL Rifiutato].</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>[!UICONTROL Timesheet Rejected]:&lt;Data inizio scheda orario&gt; - &lt;Data fine scheda orario&gt;</em></p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </td> 
   <td> Nome dell'utente che ha rifiutato la scheda orario<br>Stato della scheda orario ([!UICONTROL Rifiutato])<br>Data e ora del rifiuto della scheda orario<br><strong>[!UICONTROL Revisione]</strong> pulsante </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno ha richiesto a me l'accesso</strong> </p> <p>Chiedendomi di fare qualcosa, quindi accendilo.</p> <p>L’utente che crea il progetto vi ha accesso.</p> <p>In questo modo l’utente riceve la notifica quando qualcuno richiede l’accesso.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome dell'utente che ha richiesto l'accesso&gt; [!UICONTROL deve accedere a] &lt;Nome oggetto&gt;</em></p> <p>L'oggetto della notifica di riepilogo giornaliero è:<em> [!UICONTROL Digest of Action Needed] &lt;Data del riepilogo giornaliero&gt;</em></p> </td> 
   <td> <p>Nome oggetto<br>Nome oggetto padre<br>Numero di riferimento oggetto<br>Nome dell'utente che ha richiesto l'accesso<br>Tipo di accesso richiesto dall'utente<br><strong>[!UICONTROL Concedi] &lt;Nome dell'accesso richiesto&gt; Accesso</strong> e <strong>[!UICONTROL Concedi un accesso diverso]</strong> pulsanti<br>*Numero totale di approvazioni richieste di accesso in sospeso<br>*Collegamento a <strong>[!UICONTROL Richiesta di accesso]</strong> Approvazioni<br>*Data riepilogo giornaliero</p> </td> 
   <td><strong>Istantanea e giornaliera</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Qualcuno mi ha richiesto di caricare un documento</strong> </p> <p>Il richiedente del documento riceve una notifica e-mail quando un utente riceve una richiesta di caricamento di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>&lt;Nome dell'utente che richiede il documento&gt; [!UICONTROL richiede un documento in [!DNL Workfront].]</em></p> <p> <p>Nota: non puoi configurare questa notifica per un messaggio e-mail di riepilogo giornaliero.</p> </p> </td> 
   <td> Nome dell'utente che richiede il documento<br>Nome dell'oggetto in cui deve essere caricato il documento<br><strong>[!UICONTROL Collegalo qui]</strong> collegamento </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

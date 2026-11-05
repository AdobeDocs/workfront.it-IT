---
content-type: reference
navigation-topic: notifications
title: 'Notifiche: approvazioni unificate'
description: Le notifiche seguenti ti avvisano sulle attività di approvazione per l’esperienza Approvazioni unificate. Per informazioni sulla configurazione delle notifiche ricevute, consulta Modificare le notifiche e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# Notifiche: approvazioni unificate

{{highlighted-preview}}

Utilizza le seguenti notifiche per rimanere informato sull’attività per la revisione e le approvazioni unificate. Per informazioni sulla configurazione delle notifiche e-mail ricevute, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Queste notifiche sono disponibili solo come notifiche istantanee e non in un riepilogo giornaliero.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>Campi inclusi</th> 
   <th>Stato predefinito</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Approvazione completata - Approvato</strong> </p> <p>L'approvazione di un documento termina con una decisione finale di Approvato.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Decisione finale: (documento) approvata</em></p> </td> 
   <td> <p>Decisione finale<br>Documento<br>Data richiesta approvazione<br>Data di scadenza<br> Pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approvazione completata - Approvato con modifiche</strong> </p> <p>L'approvazione di un documento termina con una decisione finale di Approvato con modifiche.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Decisione finale: (documento) è stato approvato con modifiche</em></p> </td> 
   <td> <p>Decisione finale<br>Documento<br>Data richiesta approvazione<br>Data di scadenza<br> Pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approvazione completata - È necessario lavorare</strong> </p> <p>L'approvazione di un documento termina con una decisione finale sul lavoro necessario.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Decisione finale: (Documento) richiede lavoro</em></p> </td> 
   <td> <p>Decisione finale<br>Documento<br>Data richiesta approvazione<br>Data di scadenza<br> Pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Scadenza prossima</strong> </p> <p>Un'approvazione documento di cui fai parte sta per raggiungere la scadenza.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Scadenza approvazione in arrivo per (documento)</em></p> </td> 
   <td> <p>Richiedente<br>Ruolo<br>Team<br>Data richiesta approvazione<br>Data scadenza<br> Pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Scadenza passata</strong> </p> <p>Un'approvazione di un documento di cui fai parte passa la scadenza senza una decisione finale.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Scadenza approvazione passata per (documento)</em></p> </td> 
   <td> <p>Titolo corretto<br>Data richiesta approvazione<br>Scadenza<br> pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Fase</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisione completata</strong> </p> <p>Un revisore completa la revisione dopo l'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>(Documento) è stato rivisto</em></p> </td> 
   <td> <p>Revisore<br>Documento<br> Pulsante "Vai alla revisione"<br>Blocco dettagli: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Il limite di approvazione video si sta avvicinando (80%)</strong> </p> <p>L'approvazione di un video raggiunge l'80% del limite di approvazione video del piano.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Sei vicino al limite di richieste di approvazione video annuale in Workfront</em></p> </td> 
   <td> Titolo e corpo del testo<br>Approvazioni video richieste (utilizzo corrente)<br>Cap total (the limit)<br>Other recipients<br>"View in Workfront" button<br>"Upgrade to FIO enterprise" button </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limite di approvazione video raggiunto</strong> </p> <p>Un'approvazione video raggiunge il limite di approvazione video del piano.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Hai raggiunto il limite di richieste di approvazione video annuale in Workfront</em></p> </td> 
   <td> Titolo e corpo del testo<br>Approvazioni video richieste (utilizzo corrente)<br>Cap total (the limit)<br>Other recipients<br>"View in Workfront" button<br>"Upgrade to FIO enterprise" button </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisione effettuata - Approvata</strong> </p> <p>Un approvatore prende la decisione Approvato sull'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>(Documento) approvato da (Nome)</em></p> </td> 
   <td> <p>Decisore<br>Decisione<br>Documento e versione<br> pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisione effettuata - Approvata con modifiche</strong> </p> <p>Un approvatore prende una decisione di Approvato con modifiche all'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>(Documento) approvato con modifiche di (Nome)</em></p> </td> 
   <td> <p>Decisore<br>Decisione<br>Documento e versione<br> pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisione presa - Necessità di intervento</strong> </p> <p>Un approvatore prende la decisione di "Deve lavorare all'approvazione di un documento".</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>(Documento) richiede il lavoro di (Nome)</em></p> </td> 
   <td> <p>Decisore<br>Decisione<br>Documento e versione<br> pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documenti aggiunti o rimossi da un'approvazione raggruppata</strong> </p> <p>I documenti vengono aggiunti o rimossi da un'approvazione documento raggruppata di cui fai parte.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Un documento è stato aggiunto o rimosso da un'approvazione di cui fai parte</em></p> </td> 
   <td> <p><strong>Aggiunto:</strong><br>Richiedente<br>Nome gruppo<br>Anteprima miniature<br>Date<br>"Pulsante Vai alla revisione"<br>Blocco dettagli: Nome gruppo, Numero di risorse, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Messaggio personalizzato<br>Progetto</p> <p><strong>Rimosso:</strong><br>Richiedente<br>Nome gruppo<br>Anteprima miniature (nessun pulsante o blocco Dettagli)</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Tutte le revisioni completate</strong> </p> <p>Ogni revisore completa la revisione relativa all'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Tutte le revisioni sono state completate il (documento)</em></p> </td> 
   <td> <p>Documento<br>Data richiesta approvazione<br>Data di scadenza<br> pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Promemoria - 24 ore</strong> </p> <p>Hai 24 ore per rivedere e approvare il documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Promemoria: è necessaria la tua approvazione il (documento)</em></p> </td> 
   <td> <p>Richiedente<br>Ruolo<br>Team<br>Data richiesta approvazione<br>Data scadenza<br> Pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Promemoria - 72 ore</strong> </p> <p>Ti rimangono 72 ore per rivedere e approvare il documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Promemoria: è necessaria la tua approvazione il (documento)</em></p> </td> 
   <td> <p>Richiedente<br>Ruolo<br>Team<br>Data richiesta approvazione<br>Data scadenza<br> Pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aggiunto come approvatore o revisore</strong> </p> <p>L'utente viene aggiunto come approvatore o revisore all'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>È necessaria la tua approvazione il (documento)</em></p> </td> 
   <td> <p>Richiedente<br>Ruolo<br>Team<br>Data richiesta approvazione<br>Data scadenza<br> Pulsante "Vai alla revisione"<br>Blocco dettagli: nome documento, dettagli documento, tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rimosso come approvatore o revisore</strong> </p> <p>L'utente viene rimosso come approvatore o revisore dall'approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>La tua approvazione non è più necessaria il (documento)</em></p> </td> 
   <td> <p>Richiedente<br>Documento e versione<br>Ruolo<br>Team (nessun pulsante o blocco Dettagli)</p> <p><em>Incluso quando fa parte dell'approvazione:</em><br>Anteprima documento<br>Messaggio personalizzato</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ruolo cambiato</strong> </p> <p>Il tuo ruolo di approvatore o revisore cambia in seguito all’approvazione di un documento.</p> <p>L'oggetto dell'e-mail di notifica immediata è: <em>Il tuo ruolo in (Documento) è cambiato</em></p> </td> 
   <td> <p>Richiedente<br>Documento e versione<br>Direzione della modifica del ruolo<br> pulsante "Vai alla revisione"<br>Dettagli blocco: Nome documento, Dettagli documento, Tutti i destinatari</p> <p><em>Incluso se parte dell'approvazione:</em><br>Anteprima documento<br>Fase<br>Progetto</p> </td> 
   <td><strong>Istantanea</strong> </td> 
  </tr> 
 </tbody> 
</table>

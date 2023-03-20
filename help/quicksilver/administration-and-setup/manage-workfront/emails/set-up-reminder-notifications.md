---
title: Impostare le notifiche dei promemoria
description: Impostare le notifiche dei promemoria
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# Impostare le notifiche dei promemoria

Le notifiche dei promemoria inviano e-mail ai destinatari in base a criteri specifici. In qualità di amministratore Adobe Workfront o di utente con un livello di accesso a Planner e accesso amministrativo alle notifiche di promemoria, puoi associare manualmente le notifiche di promemoria con gli elementi di lavoro, ad esempio progetti, attività, problemi e fogli ore di lavoro.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Planner o superiore, con accesso amministrativo alle notifiche di promemoria</p> <p>Per informazioni su come concedere a un utente del piano l'accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Personalizzare l’e-mail del promemoria

Puoi personalizzare la notifica del promemoria con un’e-mail personalizzata che include un oggetto e un corpo dell’e-mail personalizzato. Il corpo dell’e-mail può contenere un HTML personalizzato.

In alternativa, puoi utilizzare l’e-mail predefinita inclusa con la notifica del promemoria. L’e-mail predefinita utilizza il nome della notifica del promemoria come oggetto dell’e-mail e il nome dell’oggetto nel corpo dell’e-mail, incluso l’evento che ha attivato la notifica.

Se desideri personalizzare l’e-mail del promemoria, devi creare un modello e-mail e allegarlo alla notifica del promemoria.

Per informazioni su come creare un modello e-mail, consulta [Configurare i modelli e-mail](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Creare una notifica di promemoria

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **E-mail** > **Notifiche**.

1. Fai clic sul pulsante **Notifiche di promemoria** scheda , quindi fai clic su **Nuova notifica promemoria**.

1. Nell’elenco a discesa, fare clic sul tipo di oggetto che si desidera associare alla notifica del promemoria.

   Ad esempio, se si desidera allegare una notifica di promemoria a una scheda attività, fare clic su **Scheda attività**.

1. In **Nuova notifica promemoria** specificare le seguenti informazioni.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome notifica promemoria</td> 
      <td>Specifica un nome per la notifica del promemoria.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Periodo idoneo</td> 
      <td> <p>Specifica il numero di ore, giorni lavorativi, giorni (giorni di calendario), settimane o mesi prima o dopo la data nel <strong>Tempi</strong> campo .</p> <p><b>NOTA</b>:  
        <ul> 
         <li> <p>Le notifiche dei promemoria iniziano 24 ore dopo la data specificata e una volta soddisfatti tutti i criteri.</p> </li> 
         <li> <p>Le notifiche di promemoria per progetti, attività e problemi si attivano ogni notte a mezzanotte, ora di montagna negli Stati Uniti. Tutti gli oggetti idonei per una notifica di promemoria da quel giorno attivano una notifica agli utenti designati poco dopo quell’ora.</p> </li> 
         <li> <p>Le notifiche dei promemoria per i fogli presenze vengono inviate all'ora specificata in base al fuso orario e alla data di fine, alla data di inizio o alla data dell'ultimo aggiornamento della scheda attività.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Seleziona l’evento che attiva la notifica del promemoria da pianificare.</p> <p>Se la notifica di promemoria è destinata a progetti, attività o problemi, le opzioni disponibili sono correlate alla data di completamento o alla data di inizio. La notifica di promemoria tiene conto della marca temporale relativa alle date di completamento e di inizio dei progetti, delle attività e dei problemi.</p>

   <p>Se la notifica del promemoria è destinata ai fogli presenze, le opzioni disponibili sono correlate alla data di fine, alla data di inizio o alla data dell'ultimo aggiornamento. La notifica di promemoria per i fogli presenze tiene conto dell'indicatore orario della data di fine, inizio e ultimo aggiornamento della scheda attività. La scheda attività inizia a mezzanotte del giorno della data di inizio (ore 12:00) e termina immediatamente prima della mezzanotte della data di fine (ore 11:59).</p>

   <p><b>NOTA</b></p>
      <p>Le notifiche di promemoria della scheda attività vengono distribuite solo una volta ogni 24 ore.</p> <p>Quando imposti più notifiche di promemoria entro un periodo di 24 ore, Workfront invia un’e-mail di notifica con tutti i promemoria inclusi in tale notifica.</p>
      <p>Ad esempio, se configuri tre notifiche di promemoria per l’attivazione di 10 ore prima, 2 ore prima e 1 ora prima di una data di scadenza, i tre promemoria verranno tutti combinati nella stessa notifica se si verificano nello stesso giorno.</p> <p>Tuttavia, se imposti una notifica di promemoria per 26 ore prima e un’altra per 1 ora prima di una data di scadenza, gli utenti riceveranno due notifiche separate. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criteri</td> 
      <td> <p>Selezionare i criteri per qualificare la notifica di promemoria da programmare. Le notifiche di promemoria non sono pianificate a meno che non venga soddisfatta la selezione dei criteri.</p> <p>Sono disponibili le seguenti opzioni relative ai criteri, a seconda del tipo di oggetto selezionato al passaggio 4:</p> 
       <ul> 
        <li><strong>Incompleto nei progetti correnti:</strong> (Disponibile per i promemoria relativi a attività e problemi) È pianificato l'invio della notifica del promemoria solo quando lo stato dell'oggetto a cui è associata la notifica del promemoria non è Completo e lo stato del progetto è Corrente.</li> 
        <li><strong>Tutti i progetti correnti:</strong>(Disponibile per i promemoria relativi a attività e problemi) La notifica del promemoria è pianificata per essere inviata indipendentemente dallo stato dell'oggetto e solo quando lo stato del progetto a cui è associata la notifica del promemoria è Current.</li> 
        <li><strong>Progetti incompleti:</strong> (Disponibile per i promemoria del progetto) La notifica del promemoria è pianificata per essere inviata quando lo stato del progetto è tutt’altro che Completo.</li> 
        <li><strong>Progetti completi:</strong> (Disponibile per i promemoria del progetto) La notifica del promemoria è pianificata per essere inviata quando lo stato del progetto è Completo.</li> 
        <li><strong>Apri fogli presenze:</strong> (Disponibile per i promemoria della scheda attività) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda attività è Aperto.</li> 
        <li><strong>Fogli temporali inviati:</strong> (Disponibile per i promemoria della scheda attività) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda attività viene inviato.</li> 
        <li><strong>Scheda attività aperta o inferiore a 40 ore a settimana:</strong> (Disponibile per i promemoria della scheda attività) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda attività è Aperto o quando la scheda attività ha meno di 40 ore registrate.</li> 
        <li><strong>Modello e-mail:</strong> Dall’elenco a discesa , seleziona un modello e-mail da allegare al promemoria.<br>Per informazioni su come creare un modello e-mail, consulta <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurare i modelli e-mail</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinatari</td> 
      <td>Seleziona i tipi di utenti che desideri ricevere la notifica. Selezionare tra vari soggetti interessati, ad esempio proprietario, approvatore o assegnatario.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
1. Allegare la notifica del promemoria a un elemento di lavoro, come descritto in [Allegare una notifica di promemoria a un oggetto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Ricevere una notifica di promemoria

Quando la condizione viene soddisfatta sull&#39;elemento a cui è collegata la notifica di promemoria, viene attivata una notifica e-mail all&#39;utente definito nella notifica di promemoria.

Per ulteriori informazioni sulla ricezione delle notifiche di promemoria, consulta la [Notifiche di promemoria](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) sezione [Notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Verifica della consegna della notifica del promemoria

Le notifiche di promemoria si attivano ogni notte a mezzanotte, ora di montagna. Tutti gli oggetti idonei per una notifica di promemoria attivano una notifica agli utenti designati poco dopo.

Per attivare manualmente le notifiche di promemoria, è innanzitutto necessario soddisfare la condizione relativa al promemoria.\
Ad esempio, se un promemoria è impostato per essere attivato un&#39;ora dopo la data di completamento pianificato di un progetto, tale ora deve essere trascorsa tra la data di impostazione del promemoria e ora. Eventuali progetti per i quali erano state pianificate date di completamento passate prima dell’attivazione del promemoria non attiveranno una notifica.

Per attivare manualmente una notifica di promemoria:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Diagnostica** nell&#39;angolo in basso a sinistra di Workfront.

1. Fai clic su **Invia notifiche promemoria** e attendi la conferma nella parte superiore dello schermo che sono stati inviati.

   Gli utenti designati nella notifica di promemoria ricevono un’e-mail.

---
title: Impostare le notifiche di promemoria
description: Le notifiche di promemoria generano e-mail inviate agli utenti in base a criteri specificati. Le notifiche di promemoria ricordano agli utenti di un’azione la necessità di eseguire per un’attività, un problema, un progetto o una scheda orario.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 2%

---

# Impostare le notifiche di promemoria

<!-- Audited: 1/2024 -->

In qualità di amministratore di Workfront, puoi creare notifiche di promemoria per gli utenti e associarli a oggetti a cui desideri che gli utenti prestino particolare attenzione.

Le notifiche di promemoria generano e-mail inviate agli utenti in base a criteri specificati. Le notifiche di promemoria ricordano agli utenti di un’azione la necessità di eseguire per un’attività, un problema, un progetto o una scheda orario.

Dopo aver creato le notifiche di promemoria, gli utenti possono associarle manualmente agli elementi di lavoro, ad esempio progetti, attività, problemi e schede orario. Per informazioni, vedere [Allegare una notifica di promemoria a un oggetto](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard </p>
 <p>oppure</p> 
<p>Corrente: Piano</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Planner o versione successiva, con accesso amministrativo per notifiche promemoria</p></td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare l’e-mail di promemoria

Puoi personalizzare l’oggetto, il corpo e il HTML nell’e-mail di notifica del promemoria.

In alternativa, puoi utilizzare l’e-mail predefinita inclusa nella notifica del promemoria. L’e-mail predefinita utilizza il nome della notifica del promemoria come oggetto dell’e-mail e il nome dell’oggetto nel corpo dell’e-mail, incluso l’evento che ha attivato la notifica.

Se desideri personalizzare l’e-mail di promemoria, devi creare un modello e-mail e allegarlo alla notifica del promemoria.

Per informazioni su come creare un modello di posta elettronica, vedere [Configurare i modelli di posta elettronica](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Creare una notifica di promemoria

{{step-1-to-setup}}

1. Fai clic su **Email** > **Notifiche** > **Notifiche promemoria**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Fai clic su **Nuova notifica promemoria**.

1. Nell&#39;elenco a discesa fare clic sul tipo di oggetto che si desidera associare alla notifica di promemoria.

   Ad esempio, se si desidera allegare una notifica di promemoria a una scheda orario, fare clic su **Scheda orario**.

1. Nella casella **Nuova notifica promemoria** visualizzata, specificare le informazioni seguenti.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome notifica promemoria</td> 
      <td>Specificare un nome per la notifica di promemoria.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Periodo idoneo</td> 
      <td> <p>Specifica il numero di ore, giorni lavorativi, giorni (giorni di calendario), settimane o mesi prima o dopo la data nel campo <strong>Timing</strong>.</p> <p><b>NOTA</b>:  
        <ul> 
         <li> <p>Le notifiche di promemoria iniziano 24 ore dopo la data specificata e una volta soddisfatti tutti i criteri.</p> </li> 
         <li> <p>Le notifiche di promemoria per progetti, attività e problemi si attivano ogni notte a mezzanotte, ora di montagna negli Stati Uniti. Tutti gli oggetti idonei per una notifica di promemoria da quel giorno attivano una notifica agli utenti designati poco dopo tale momento.</p> </li> 
         <li> <p>Le notifiche di promemoria per le schede orario vengono inviate all’ora specificata in base al fuso orario e alla data di fine della scheda orario, alla data di inizio o alla data dell’ultimo aggiornamento.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Seleziona l’evento che attiva la notifica di promemoria da programmare.</p> <p>Se la notifica di promemoria è destinata a progetti, attività o problemi, le opzioni disponibili sono relative alla Data di completamento o alla Data di inizio. La notifica di promemoria tiene conto della marca temporale sulle date di completamento e di inizio dei progetti, delle attività e dei problemi.</p>

   <p>Se la notifica di promemoria è destinata alle schede orario, le opzioni disponibili sono relative alla Data di fine, alla Data di inizio o alla Data ultimo aggiornamento. La notifica del promemoria per le schede orario tiene conto della marca temporale delle date di fine, inizio e ultimo aggiornamento della scheda orario. La scheda orario inizia a mezzanotte del giorno della data di inizio (12:00) e termina subito prima di mezzanotte della data di fine (23:59).</p>

   <p><b>NOTA</b></p>
      <p>Le notifiche dei promemoria delle schede orario vengono distribuite solo una volta ogni 24 ore.</p> <p>Quando imposti più notifiche di promemoria entro un periodo di 24 ore, Workfront invia un’e-mail di notifica con tutti i promemoria inclusi nella notifica.</p>
      <p>Ad esempio, se configuri tre notifiche di promemoria in modo che vengano attivate 10 ore prima, 2 ore prima e 1 ora prima di una data di scadenza, tutti e tre i promemoria verranno combinati nella stessa notifica se si verificano durante lo stesso giorno.</p> <p>Tuttavia, se imposti una notifica di promemoria per 26 ore prima e un’altra per 1 ora prima di una data di scadenza, gli utenti riceveranno due notifiche separate. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criteri</td> 
      <td> <p>Selezionare i criteri per qualificare la notifica di promemoria da programmare. Le notifiche di promemoria non vengono pianificate a meno che la selezione dei criteri non sia soddisfatta.</p> <p>A seconda del tipo di oggetto selezionato nel passaggio 4, sono disponibili le seguenti opzioni di criteri:</p> 
       <ul> 
        <li><strong>Incompleto nei progetti correnti:</strong> <i>(Disponibile per promemoria attività e problemi)</i> La notifica promemoria è pianificata per essere inviata solo quando lo stato dell'oggetto a cui è associata la notifica promemoria non è Completo e lo stato del progetto è Corrente.</li> 
        <li><strong>Tutti i progetti correnti:</strong> <i>(Disponibile per promemoria attività e problemi)</i> La notifica promemoria è pianificata per essere inviata indipendentemente dallo stato dell'oggetto e solo quando lo stato del progetto a cui è associata la notifica promemoria è Corrente.</li> 
        <li><strong>Progetti incompleti:</strong> <i>(Disponibile per i promemoria del progetto)</i> La notifica del promemoria è programmata per essere inviata quando lo stato del progetto è tutt'altro che Completo.</li> 
        <li><strong>Tutti i progetti:</strong> <i>(Disponibile per i promemoria del progetto)</i> La notifica del promemoria è pianificata per essere inviata indipendentemente dallo stato del progetto.</li> 
        <li><strong>Schede orario aperte:</strong> <i>(Disponibile per i promemoria delle schede orario)</i> La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Aperto.</li> 
        <li><strong>Schede orario inviate:</strong> <i>(Disponibile per i promemoria delle schede orario)</i> La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Inviato.</li> 
        <li><strong>Apri scheda orario o meno di 40 ore alla settimana:</strong> <i>(Disponibile per i promemoria della scheda orario)</i> La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Aperto o quando la scheda orario ha registrato meno di 40 ore.</li> 
        <li><strong>Modello e-mail:</strong> dall'elenco a discesa, selezionare un modello e-mail da allegare al promemoria.<br>Per informazioni su come creare un modello di posta elettronica, fare riferimento a <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurare i modelli di posta elettronica</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinatari</td> 
      <td><p>A seconda dell’oggetto a cui si riferisce la notifica di promemoria, seleziona uno dei seguenti tipi di utenti a cui desideri inviare la notifica:</p>
      <ul>
      <li>Assegnato a</li>
      <li>Immesso da</li>
      <li>Team di progetto (tutti gli utenti del team di progetto ricevono il promemoria)</li>
      <li>Assegnatari attività dipendenti (gli utenti assegnati ad attività dipendenti ricevono il promemoria)</li>
      <li>Proprietario progetto</li>
      <li>Assegnato a (gli utenti assegnati a un'attività o a un problema ricevono il promemoria)</li>
      <li>Proprietario scheda orario</li>
      <li>Progetti non completati</li>
      <li>Gestore del proprietario scheda orario</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
1. Allegare la notifica di promemoria a un elemento di lavoro, come descritto in [Allegare una notifica di promemoria a un oggetto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Ricevi una notifica di promemoria

Quando la condizione viene soddisfatta sull’elemento a cui è allegata la notifica del promemoria, viene attivata una notifica e-mail all’utente definito nella notifica del promemoria.

Per ulteriori informazioni sulla ricezione di notifiche di promemoria, vedere la sezione [Notifiche di promemoria](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) in [Notifiche di Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Consegna notifiche promemoria test

Le notifiche di promemoria vengono attivate ogni notte a mezzanotte, ora di montagna. Tutti gli oggetti idonei per una notifica di promemoria attivano una notifica agli utenti designati poco dopo.

Per fare in modo che le notifiche dei promemoria vengano attivate manualmente, è necessario che la condizione per il promemoria sia soddisfatta.\
Ad esempio, se un promemoria è impostato per essere attivato un’ora dopo la data di completamento pianificata di un progetto, tale ora deve essere trascorsa tra la data in cui è stato impostato il promemoria e ora. Qualsiasi progetto con date di completamento pianificate passate prima dell’attivazione del promemoria non attiverà una notifica.

Per attivare manualmente una notifica di promemoria:

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Diagnostica** nell&#39;angolo inferiore sinistro di Workfront.

1. Fai clic su **Invia notifiche promemoria** e attendi la conferma nella parte superiore della schermata dell&#39;invio.

   Gli utenti designati nella notifica del promemoria ricevono un messaggio e-mail.

![](assets/reminder-test.png)
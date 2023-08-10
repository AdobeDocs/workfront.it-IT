---
title: Configurare le notifiche di promemoria
description: Configurare le notifiche di promemoria
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 1129f8ab93d349325bed56bc2b3ba94c2600c03f
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 1%

---

# Configurare le notifiche di promemoria

Le notifiche di promemoria inviano e-mail ai destinatari in base a criteri specificati. In qualità di amministratore di Adobe Workfront o di utente con un livello di accesso alla Pianificazione e un accesso amministrativo alle notifiche dei promemoria, puoi associare manualmente le notifiche dei promemoria agli elementi di lavoro, come progetti, attività, problemi e schede orario.

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Planner o versione successiva, con accesso amministrativo per notifiche promemoria</p> <p>Per informazioni su come concedere a un utente del piano l'accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Personalizzare l’e-mail di promemoria

Puoi personalizzare la notifica del promemoria con un’e-mail personalizzata che include un oggetto e un corpo dell’e-mail personalizzati. Il corpo dell’e-mail può contenere HTML personalizzati.

In alternativa, puoi utilizzare l’e-mail predefinita inclusa nella notifica del promemoria. L’e-mail predefinita utilizza il nome della notifica del promemoria come oggetto dell’e-mail e il nome dell’oggetto nel corpo dell’e-mail, incluso l’evento che ha attivato la notifica.

Se desideri personalizzare l’e-mail di promemoria, devi creare un modello e-mail e allegarlo alla notifica del promemoria.

Per informazioni su come creare un modello e-mail, consulta [Configurare i modelli e-mail](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Creare una notifica di promemoria

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **E-mail** > **Notifiche** > **Avvisi di Promemoria**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Clic **Nuovo Avviso di Promemoria**.

1. Nell&#39;elenco a discesa fare clic sul tipo di oggetto che si desidera associare alla notifica di promemoria.

   Ad esempio, se desideri allegare una notifica di promemoria a una scheda orario, fai clic su **Scheda orario**.

1. In **Nuovo Avviso di Promemoria** nella casella visualizzata, specificare le seguenti informazioni.

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
      <td> <p>Specifica il numero di ore, giorni lavorativi, giorni (giorni di calendario), settimane o mesi prima o dopo la data nella <strong>Tempistica</strong> campo.</p> <p><b>NOTA</b>:  
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
        <li><strong>Incompleto nei progetti correnti:</strong> (Disponibile per promemoria relativi a attività e problemi) La notifica di promemoria è pianificata per essere inviata solo quando lo stato dell'oggetto a cui è associata la notifica di promemoria non è Completo e lo stato del progetto è Corrente.</li> 
        <li><strong>Tutto nei progetti correnti:</strong>(Disponibile per promemoria relativi a attività e problemi) La notifica di promemoria è pianificata per essere inviata indipendentemente dallo stato dell'oggetto e solo quando lo stato del progetto a cui è associata la notifica di promemoria è Corrente.</li> 
        <li><strong>Progetti non Completati:</strong> (Disponibile per i promemoria del progetto) La notifica del promemoria è pianificata per essere inviata quando lo stato del progetto è diverso da Completo.</li> 
        <li><strong>Progetti completati:</strong> (Disponibile per i promemoria del progetto) La notifica del promemoria è programmata per essere inviata quando lo stato del progetto è Completo.</li> 
        <li><strong>Schede orario aperte:</strong> (Disponibile per i promemoria della scheda orario) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Aperto.</li> 
        <li><strong>Schede orario inviate:</strong> (Disponibile per i promemoria della scheda orario) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Inviato.</li> 
        <li><strong>Scheda orario aperta o meno di 40 ore a settimana:</strong> (Disponibile per i promemoria della scheda orario) La notifica del promemoria è pianificata per essere inviata quando lo stato della scheda orario è Aperto o quando la scheda orario ha registrato meno di 40 ore.</li> 
        <li><strong>Modello e-mail:</strong> Dall’elenco a discesa, seleziona un modello e-mail da allegare al promemoria.<br>Per informazioni su come creare un modello e-mail, consulta <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurare i modelli e-mail</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinatari</td> 
      <td>Seleziona i tipi di utenti a cui desideri inviare la notifica. Consente di selezionare tra vari soggetti interessati all'oggetto, ad esempio proprietario, approvatore o assegnatario.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
1. Allegare la notifica di promemoria a un elemento di lavoro, come descritto in [Allegare una notifica di promemoria a un oggetto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Ricevi una notifica di promemoria

Quando la condizione viene soddisfatta sull’elemento a cui è allegata la notifica del promemoria, viene attivata una notifica e-mail all’utente definito nella notifica del promemoria.

Per ulteriori informazioni sulla ricezione delle notifiche di promemoria, vedere [Notifiche promemoria](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) sezione in [Notifiche Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Consegna notifiche promemoria test

Le notifiche di promemoria vengono attivate ogni notte a mezzanotte, ora di montagna. Tutti gli oggetti idonei per una notifica di promemoria attivano una notifica agli utenti designati poco dopo.

Per fare in modo che le notifiche dei promemoria vengano attivate manualmente, è necessario che la condizione per il promemoria sia soddisfatta.\
Ad esempio, se un promemoria è impostato per essere attivato un’ora dopo la data di completamento pianificata di un progetto, tale ora deve essere trascorsa tra la data in cui è stato impostato il promemoria e ora. Qualsiasi progetto con date di completamento pianificate passate prima dell’attivazione del promemoria non attiverà una notifica.

Per attivare manualmente una notifica di promemoria:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** > **Diagnostica** nell&#39;angolo inferiore sinistro di Workfront.

1. Clic **Invia Avvisi di Promemoria** e attendi la conferma, nella parte superiore della schermata, dell’invio.

   Gli utenti designati nella notifica del promemoria ricevono un messaggio e-mail.

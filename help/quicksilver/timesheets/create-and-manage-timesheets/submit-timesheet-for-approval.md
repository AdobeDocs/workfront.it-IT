---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Invia una scheda attività per l'approvazione
description: L'invio della scheda attività per l'approvazione consente al tuo responsabile di avere visibilità nelle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Invia una scheda attività per l&#39;approvazione

L&#39;invio della scheda attività per l&#39;approvazione consente al tuo responsabile di avere visibilità nelle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza accesso o superiore a Attività e problemi</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Invia una scheda attività per l&#39;approvazione

* [Invia una scheda attività per l&#39;approvazione](#submit-a-timesheet-for-approval)
* [Visualizza lo stato di una scheda attività inviata](#view-the-status-of-a-submitted-timesheet)

### Invia una scheda attività per l&#39;approvazione

Dopo aver impostato un approvatore della scheda attività (come descritto nella sezione [Designazione degli approvatori della scheda attività](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) nell&#39;articolo [Approva una scheda attività](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **Chiudi** il pulsante nella parte inferiore della scheda attività diventa un **Invia per approvazione** pulsante .

Per inviare una scheda attività per l&#39;approvazione:

1. Passa a una scheda attività configurata per disporre di un approvatore.
1. Tempo di log, come descritto in [Tempo di log](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Fai clic su **Invia per approvazione** per avviare il processo di approvazione della scheda attività.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   La **Invia per approvazione** viene sostituito dal **Approva**, **Rifiuta** e **Richiama** pulsanti. Lo stato della scheda attività cambia in **Inviato**.

   Quando la scheda attività viene inviata per l&#39;approvazione, l&#39;approvatore visualizza la scheda attività elencata in **Approvazioni** area **Pagina principale** pagina. Potrebbero verificarsi i seguenti eventi:

   * Se lo approvano, il **Richiama** il pulsante cambia in **Riaprire** e lo stato della scheda attività viene aggiornato a **Apri**.
   * Se la rifiutano, la **Invia per approvazione** sostituisce il pulsante **Richiama** lo stato del pulsante e della scheda attività si aggiorna a **Rifiutato**.

1. (Facoltativo) Fai clic su **Richiama** se è necessario riaprire la scheda attività e aggiornare l&#39;ora. Per informazioni, consulta la sezione [Richiama una scheda attività](#recall-a-timesheet) in questo articolo.

### Visualizza lo stato di una scheda attività inviata {#view-the-status-of-a-submitted-timesheet}

È possibile visualizzare lo stato di una scheda attività dopo l&#39;invio.

Se l&#39;amministratore Workfront ha abilitato l&#39;approvazione della scheda attività per l&#39;utente e il rifiuto della scheda attività per i gestori di eventi utente, viene inviata una notifica dopo l&#39;approvazione o il rifiuto della scheda attività. Per informazioni sull&#39;abilitazione delle notifiche degli eventi, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Senza queste notifiche, è possibile conoscere lo stato dei fogli presenze inviati nell&#39;area Scheda attività di Workfront.

Per visualizzare lo stato di una scheda attività:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fai clic su **Schede temporali**. La **Tutto** Il filtro è selezionato per impostazione predefinita.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco dei fogli presenze, effettuare una delle seguenti operazioni:

   * Seleziona **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

      Oppure

      Seleziona **Fogli orari personali** per visualizzare solo i fogli presenze.

      Questo applica le approvazioni della scheda attività personale o i filtri della scheda attività personale all&#39;elenco dei fogli presenze.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Pagine attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo hanno rimosso le approvazioni della scheda attività personale e i filtri della scheda attività personale dai controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   >   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Condizionale) Se hai selezionato **Fogli orari personali**, assicura che **Standard** viene applicata la visualizzazione e viene visualizzata la **Stato** colonna.

   I fogli presenze possono presentare i seguenti stati:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aperto</td> 
      <td> <p>La scheda attività è attualmente aperta ed è possibile registrare il tempo. </p> <p>Viene visualizzata una scheda attività richiamata con lo stato Apri. Per informazioni, consulta la sezione <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda attività</a> in questo articolo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inviate</td> 
      <td>La scheda attività è stata inviata per l'approvazione ma non è ancora stata approvata. È possibile richiamare una scheda attività inviata per continuare a modificarla. Per informazioni, consulta la sezione <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda attività</a> in questo articolo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiuso</td> 
      <td> <p>Esistono i seguenti scenari:</p> 
       <ul> 
        <li> <p>Se la scheda attività non dispone di un approvatore, il tempo è stato salvato e chiuso.</p> </li> 
        <li> <p>Se la scheda attività dispone di un approvatore, è stata inviata per l'approvazione ed è stata approvata.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rifiutato</td> 
      <td>La scheda attività è stata inviata per l'approvazione e l'approvatore l'ha rifiutata.</td> 
     </tr> 
    </tbody> 
   </table>

## Richiama una scheda attività {#recall-a-timesheet}

È possibile richiamare una scheda attività già inviata per l&#39;approvazione. È possibile richiamare solo i fogli presenze non approvati.

Per richiamare una scheda attività:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Schede temporali**.
1. Fai clic su **Fogli orari personali** nell’angolo superiore destro dello schermo o seleziona **Fogli orari personali** dal **Filtro** ![](assets/filter-nwepng.png) menu a discesa.
1. Fare clic sull&#39;intervallo di tempo per una scheda attività con stato **Inviato**.
1. Fai clic su **Richiama**.

   La scheda attività diventa nuovamente modificabile e il suo stato cambia in **Apri**.

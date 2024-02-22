---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Invia una scheda orario per l'approvazione
description: L'invio della scheda orario per l'approvazione fornisce al tuo responsabile visibilità sulle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# Invia una scheda orario per l&#39;approvazione

L&#39;invio della scheda orario per l&#39;approvazione fornisce al tuo responsabile visibilità sulle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o superiore per attività e problemi</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Invia una scheda orario per l&#39;approvazione

* [Invia una scheda orario per l&#39;approvazione](#submit-a-timesheet-for-approval)
* [Visualizzare lo stato di una scheda orario inviata](#view-the-status-of-a-submitted-timesheet)

### Invia una scheda orario per l&#39;approvazione

Dopo aver impostato un approvatore della scheda orario (come descritto nella sezione [Designa approvatori scheda orario](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) nell’articolo [Approvare una scheda orario](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), il **Chiudi** nella parte inferiore della scheda orario diventa un **Invia per approvazione** pulsante.

Per inviare una scheda orario per l&#39;approvazione:

1. Vai a una scheda orario configurata per avere un approvatore.
1. Tempo di connessione, come descritto in [Tempo di connessione](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Clic **Invia per approvazione** per avviare il processo di approvazione della scheda orario.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Il **Invia per approvazione** è sostituito da **Approva**, **Rifiuta**, e **Richiama** pulsanti. Lo stato della scheda orario diventa **Inviato**.

   Quando la scheda orario viene inviata per l&#39;approvazione, l&#39;approvatore visualizza la scheda orario elencata in **Approvazioni** area sul **Home** pagina. Potrebbero verificarsi gli eventi seguenti:

   * Se la approvano, il **Richiama** il pulsante diventa **Riapri** e lo stato della scheda orario viene aggiornato in **Apri**.
   * Se la rifiutano, il **Invia per approvazione** sostituisce il pulsante **Richiama** e lo stato della scheda orario viene aggiornato in **Rifiutato**.

1. (Facoltativo) Fai clic su **Richiama** se devi riaprire la scheda orario e aggiornare l’orario. Per informazioni, vedere [Richiama una scheda orario](#recall-a-timesheet) in questo articolo.

### Visualizzare lo stato di una scheda orario inviata {#view-the-status-of-a-submitted-timesheet}

È possibile visualizzare lo stato di una scheda orario dopo averla inviata.

Se l&#39;amministratore di Workfront ha attivato i gestori eventi Approvazione scheda orario e Rifiuto scheda orario per utente, l&#39;utente riceverà una notifica dopo l&#39;approvazione o il rifiuto della scheda orario. Per informazioni sull’abilitazione delle notifiche degli eventi, consulta [Tipi di notifica degli eventi](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Senza queste notifiche, puoi scoprire lo stato delle schede orario inviate nell’area Scheda orario di Workfront.

Per visualizzare lo stato di una scheda orario:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront.
1. Clic **Schede orario**. Il **Tutti** è selezionato per impostazione predefinita.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell’angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro. ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   >   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Condizionale) Se hai selezionato **Le mie schede orario**, assicurano che **Standard** viene applicata la visualizzazione e si osserva **Stato** colonna.

   Le schede orario possono avere i seguenti stati:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aperti</td> 
      <td> <p>La scheda orario è attualmente aperta e si potrebbe registrare l'ora. </p> <p>Viene visualizzata una scheda orario richiamata con lo stato Aperto. Per informazioni, vedere <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda orario</a> in questo articolo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inviate</td> 
      <td>La scheda orario è stata inviata per l'approvazione ma non è ancora stata approvata. È possibile richiamare una scheda orario inviata per continuare a modificarla. Per informazioni, vedere <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda orario</a> in questo articolo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiuso</td> 
      <td> <p>Esistono i seguenti scenari:</p> 
       <ul> 
        <li> <p>Se la scheda orario non ha un approvatore, l'orario è stato salvato e chiuso.</p> </li> 
        <li> <p>Se la scheda orario dispone di un approvatore, è stata inviata per l'approvazione ed è stata approvata.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rifiutato</td> 
      <td>La scheda orario è stata inviata per l'approvazione e l'approvatore l'ha rifiutata.</td> 
     </tr> 
    </tbody> 
   </table>

## Richiama una scheda orario {#recall-a-timesheet}

È possibile richiamare una scheda orario già inviata per l&#39;approvazione. È possibile richiamare solo le schede orario non approvate.

Per richiamare una scheda orario:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront.

1. Clic **Schede orario**.
1. Clic **Le mie schede orario** nell’angolo superiore destro dello schermo o seleziona **Le mie schede orario** dal **Filtro** ![](assets/filter-nwepng.png) menu a discesa.
1. Fai clic sull’intervallo di tempo per una scheda orario con stato **Inviato**.
1. Clic **Richiama**.

   La scheda orario diventa nuovamente modificabile e il suo stato cambia in **Apri**.

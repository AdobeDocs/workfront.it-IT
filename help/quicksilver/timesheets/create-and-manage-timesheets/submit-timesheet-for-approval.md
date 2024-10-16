---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Invia una scheda orario per l'approvazione
description: L'invio della scheda orario per l'approvazione fornisce al tuo responsabile visibilità sulle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Invia una scheda orario per l&#39;approvazione

<!--Audited: 8/2024-->

L&#39;invio della scheda orario per l&#39;approvazione fornisce al tuo responsabile visibilità sulle ore lavorative. Gli approvatori possono verificare che tutto il tempo registrato sia stato assegnato nelle aree corrette e che sia stato registrato un numero sufficiente di ore per il periodo di tempo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Chiaro o superiore </p>
   <p>Corrente: revisione o versione successiva </p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizzare o accedere più facilmente ad attività e problemi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per la scheda orario</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Invia una scheda orario per l&#39;approvazione

* [Invia una scheda orario per l&#39;approvazione](#submit-a-timesheet-for-approval)
* [Visualizzare lo stato di una scheda orario inviata](#view-the-status-of-a-submitted-timesheet)

### Invia una scheda orario per l&#39;approvazione

Dopo aver impostato un approvatore della scheda orario (come descritto nella sezione [Designare gli approvatori della scheda orario](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) nell&#39;articolo [Approvare una scheda orario](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), il pulsante **Chiudi** nella parte inferiore della scheda orario diventa un pulsante **Invia per approvazione**.

Per inviare una scheda orario per l&#39;approvazione:

1. Vai a una scheda orario configurata per avere un approvatore.
1. Tempo di connessione, come descritto in [Tempo di connessione](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Fai clic su **Invia per approvazione** per avviare il processo di approvazione della scheda orario.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Il pulsante **Invia per approvazione** è sostituito dai pulsanti **Approva**, **Rifiuta** e **Richiama**. Lo stato della scheda orario diventa **Inviato**.

   Quando la scheda orario viene inviata per l&#39;approvazione, l&#39;approvatore visualizza la scheda orario elencata nel widget **Approvazioni personali** nell&#39;area **Home**. Potrebbero verificarsi gli eventi seguenti:

   * Se l&#39;approvano, il pulsante **Richiama** diventa **Riapri** e lo stato della scheda orario diventa **Apri**.
   * Se rifiuta, il pulsante **Invia per approvazione** sostituisce il pulsante **Richiama** e lo stato della scheda orario viene aggiornato a **Rifiutato**.

1. (Facoltativo) Fai clic su **Richiama** per riaprire la scheda orario e aggiornare l&#39;orario. Per informazioni, vedere la sezione [Richiama una scheda orario](#recall-a-timesheet) in questo articolo.

### Visualizzare lo stato di una scheda orario inviata {#view-the-status-of-a-submitted-timesheet}

È possibile visualizzare lo stato di una scheda orario dopo averla inviata.

Se l&#39;amministratore di Workfront ha attivato i gestori eventi Approvazione scheda orario e Rifiuto scheda orario per utente, l&#39;utente riceverà una notifica dopo l&#39;approvazione o il rifiuto della scheda orario. Per informazioni sull&#39;attivazione delle notifiche degli eventi, vedere [Tipi di notifica degli eventi](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Senza queste notifiche, puoi scoprire lo stato delle schede orario inviate nell’area Scheda orario di Workfront.

Per visualizzare lo stato di una scheda orario:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.
1. Fai clic su **Schede orario**. Il filtro **All** è selezionato per impostazione predefinita.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fare clic sull&#39;icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   >   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Condizionale) Se hai selezionato **Le mie schede orario**, accertati che sia applicata la visualizzazione **Standard** e osserva la colonna **Stato**.

   Le schede orario possono avere i seguenti stati:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aperti</td> 
      <td> <p>La scheda orario è attualmente aperta e si potrebbe registrare l'ora. </p> <p>Viene visualizzata una scheda orario richiamata con lo stato Aperto. Per informazioni, vedere la sezione <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda orario</a> in questo articolo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inviate</td> 
      <td>La scheda orario è stata inviata per l'approvazione ma non è ancora stata approvata. È possibile richiamare una scheda orario inviata per continuare a modificarla. Per informazioni, vedere la sezione <a href="#recall-a-timesheet" class="MCXref xref">Richiama una scheda orario</a> in questo articolo. </td> 
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

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **Schede orario**.
1. Fai clic su **Le mie schede orario** nell&#39;angolo superiore destro dello schermo o seleziona **Le mie schede orario** dal menu a discesa **Filtra** ![](assets/filter-nwepng.png).
1. Fare clic sull&#39;intervallo di tempo per una scheda orario con stato **Inviato**.
1. Fare clic su **Richiama**.

   La scheda orario diventa nuovamente modificabile e il suo stato cambia in **Open**.

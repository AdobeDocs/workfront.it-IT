---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifica informazioni scheda orario
description: In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 1%

---

# Modifica informazioni scheda orario

In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.

È possibile modificare le informazioni su un&#39;unica scheda orario oppure modificare più schede orario in blocco.

>[!IMPORTANT]
>
>Se gli utenti sono associati ai profili delle schede orario e queste vengono generate automaticamente, le modifiche apportate alle schede esistenti non verranno applicate alle schede orario che verranno generate per le date future. Tutte le schede orario generate automaticamente hanno le impostazioni stabilite nei Profili delle schede orario. Per ulteriori informazioni, consulta [Creare profili di schede orario](../create-and-manage-timesheets/create-timesheet-profiles.md)


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>È necessario disporre dell'accesso amministrativo alle schede orario. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Modifica schede orario

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Schede orario**.

   Il **Tutti** Il filtro è selezionato per impostazione predefinita e visualizza tutte le schede orario a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Fai clic su **ricerca** icona ![](assets/search-icon.png) e digita una parola chiave e cerca una scheda orario specifica. Ad esempio, puoi cercare un intervallo di tempo della scheda orario o il nome del proprietario.

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell’angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro. ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facoltativo) Fai clic su **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) icone per applicare una visualizzazione o un raggruppamento diverso o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare viste in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona una o più schede orario, quindi fai clic su **Modifica** icona ![](assets/edit-icon.png) nella parte superiore dell’elenco delle schede orario.
1. Visualizza o specifica le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Proprietario</strong> </td> 
      <td> <p>Questo è il nome dell'utente per cui è stata creata la scheda orario. Impossibile modificare questo campo. </p> <p>Il campo non viene visualizzato quando si selezionano più schede orario. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di inizio</strong> </td> 
      <td>Questa è la data di inizio della scheda orario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di fine</strong> </td> 
      <td> Questa è la data di fine della scheda orario.</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>Stato</strong> </td> 
      <td> Questo è lo stato della scheda orario.
      Di seguito sono riportate le possibili opzioni di stato della scheda orario: 
      <ul><li><b>Apri</b>: la scheda orario è aperta e le voci orarie possono essere modificate.</li>
      <li><b>Inviato</b>: la scheda orario viene inviata per l’approvazione agli approvatori designati.</li>
      <li><b>Rifiutato</b>: la scheda orario non è stata approvata dagli approvatori ed è ora nuovamente disponibile per l’utente per modificare le voci relative all’ora.</li>
      <li><b>Chiuso</b>: la scheda orario è chiusa dall’utente o approvata dall’approvatore e, di conseguenza, ora è chiusa. Non è possibile aggiungere un orario a una scheda orario chiusa.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approvatori</strong> </td> 
      <td> <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. Solo gli utenti con accesso amministrativo alle schede orario possono essere impostati come approvatori. </p> <p>Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Inizia a immettere i nomi degli approvatori della scheda orario e selezionali quando vengono visualizzati nell’elenco.</p> <p>In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, questa viene contrassegnata come <strong>Chiuso</strong> e scompare dall’elenco approvazioni scheda orario di tutti gli approvatori rimanenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Può modificare l’ora</strong> </td> 
      <td> <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda orario.</p> <p>Questa opzione non è disponibile quando si selezionano più schede orario. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td> <p>È possibile scegliere di nascondere la casella Straordinari nella scheda attività.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

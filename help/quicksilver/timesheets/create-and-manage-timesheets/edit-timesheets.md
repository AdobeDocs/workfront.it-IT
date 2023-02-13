---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifica delle informazioni della scheda attività
description: In qualità di utente con accesso amministrativo ai fogli presenze, puoi modificare le informazioni sui fogli presenze esistenti in Adobe Workfront . Ad esempio, è possibile modificare il proprietario, gli approvatori o l'intervallo di tempo della scheda attività.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# Modifica delle informazioni della scheda attività

In qualità di utente con accesso amministrativo ai fogli presenze, puoi modificare le informazioni sui fogli presenze esistenti in Adobe Workfront . Ad esempio, è possibile modificare il proprietario, gli approvatori o l&#39;intervallo di tempo della scheda attività.

È possibile modificare le informazioni in una singola scheda attività oppure modificare più fogli presenze in blocco.

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario disporre dell’accesso amministrativo ai fogli presenze. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modificare i fogli presenze

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Schede temporali**.

   La **Tutto** Il filtro è selezionato per impostazione predefinita e visualizza tutti i fogli ore a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Fai clic sul pulsante **ricerca** icona ![](assets/search-icon.png) e digitare una parola chiave e cercare una scheda attività specifica. Ad esempio, è possibile cercare un intervallo di tempo della scheda attività o il nome del proprietario.

1. (Facoltativo) Per aggiornare il filtro nell’elenco dei fogli presenze, effettuare una delle seguenti operazioni:

   * Seleziona **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

      Oppure

      Seleziona **Fogli orari personali** per visualizzare solo i fogli presenze.

      Questo applica le approvazioni della scheda attività personale o i filtri della scheda attività personale all&#39;elenco dei fogli presenze.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Pagine attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo hanno rimosso le approvazioni della scheda attività personale e i filtri della scheda attività personale dai controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facoltativo) Fai clic sul pulsante **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diversi o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, visualizzazioni o raggruppamenti, consulta i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona uno o più fogli presenze, quindi fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nella parte superiore dell&#39;elenco della scheda attività.
1. Visualizza o specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Proprietario</strong> </td> 
      <td> <p>Nome dell'utente per il quale è stata creata la scheda attività. Non è possibile modificare questo campo. </p> <p>Il campo non viene visualizzato quando si selezionano più fogli presenze. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di inizio</strong> </td> 
      <td>Data di inizio della scheda attività.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di fine</strong> </td> 
      <td> Data di fine della scheda attività.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approvatori</strong> </td> 
      <td> <p>Gli approvatori sono utenti che approvano la scheda attività per gli utenti associati alla scheda attività. È possibile impostare come approvatori solo gli utenti con accesso amministrativo ai fogli presenze. </p> <p>Per ulteriori informazioni sui diritti amministrativi della scheda attività, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Iniziare a immettere i nomi degli approvatori della scheda attività e selezionarli quando vengono visualizzati nell'elenco.</p> <p>È possibile avere più approvatori in una scheda attività. In questo caso, dopo che uno degli approvatori approva la scheda attività, la scheda attività viene contrassegnata come <strong>Chiuso</strong> e scompare dall'elenco delle approvazioni della scheda attività di tutti gli approvatori rimanenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Può modificare l’ora</strong> </td> 
      <td> <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda attività.</p> <p>Questa opzione non è disponibile quando si selezionano più fogli presenze. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td> <p>È possibile scegliere di nascondere la casella Overtime nella scheda attività.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su Salva.

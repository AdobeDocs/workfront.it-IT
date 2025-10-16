---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifica informazioni scheda orario
description: In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 1%

---

# Modifica informazioni scheda orario

In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.

È possibile modificare le informazioni su un&#39;unica scheda orario oppure modificare più schede orario in blocco.

>[!IMPORTANT]
>
>Se gli utenti sono associati ai profili delle schede orario e queste vengono generate automaticamente, le modifiche apportate alle schede esistenti non verranno applicate alle schede orario che verranno generate per le date future. Tutte le schede orario generate automaticamente hanno le impostazioni stabilite nei Profili delle schede orario. Per ulteriori informazioni, consulta [Creare profili scheda orario](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Accesso amministrativo alle schede orario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifica schede orario

1. Fai clic sull&#39;icona **del** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Schede orario**.

   Il filtro **All** è selezionato per impostazione predefinita e visualizza tutte le schede orario a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Fai clic sull&#39;icona **ricerca** ![](assets/search-icon.png), digita una parola chiave e cerca una scheda orario specifica. Ad esempio, puoi cercare un intervallo di tempo della scheda orario o il nome del proprietario.

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fare clic sull&#39;icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   >
   >   
   >   
   >   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facoltativo) Fai clic sulle icone **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diverso o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona una o più schede orario, quindi fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png) nella parte superiore dell&#39;elenco delle schede orario.
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
      <td role="rowheader"><strong>Data inizio</strong> </td> 
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
      <ul><li><b>Apri</b>: la scheda orario è aperta e le ore possono essere modificate.</li>
      <li><b>Inviato</b>: la scheda orario viene inviata per l'approvazione agli approvatori designati.</li>
      <li><b>Rifiutato</b>: la scheda orario non è stata approvata dagli approvatori ed è ora nuovamente disponibile per consentire all'utente di modificare le voci relative all'ora.</li>
      <li><b>Chiusa</b>: la scheda orario è stata chiusa dall'utente o approvata dall'approvatore e di conseguenza è ora chiusa. Non è possibile aggiungere un orario a una scheda orario chiusa.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approvatori</strong> </td> 
      <td> <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. Solo gli utenti con accesso amministrativo alle schede orario possono essere impostati come approvatori. </p> <p>Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p>Inizia a immettere i nomi degli approvatori della scheda orario e selezionali quando vengono visualizzati nell’elenco.</p> <p>In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come <strong>Chiusa</strong> e scompare dall'elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifica ora</strong> </td> 
      <td> <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda orario.</p> <p>Questa opzione non è disponibile quando si selezionano più schede orario. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td> <p>È possibile scegliere di nascondere la casella Straordinari nella scheda attività.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

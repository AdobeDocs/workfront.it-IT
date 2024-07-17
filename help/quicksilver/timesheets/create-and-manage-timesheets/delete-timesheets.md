---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminare i timesheet in Adobe Workfront
description: Le modifiche apportate a un profilo di scheda orario non sono immediatamente effettive per le schede orario esistenti, come spiegato in Creare, modificare e assegnare profili di scheda orario. Per rendere visibili le modifiche nelle schede orario esistenti, devi eliminare le schede orario generate e generarne di nuove. Questo si applica solo alle schede orario generate associando profili della scheda orario agli utenti.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Eliminare i timesheet in Adobe Workfront

Le modifiche apportate a un profilo scheda orario non sono immediatamente valide per le schede orario esistenti, come spiegato in [Creare, modificare e assegnare profili scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Per rendere visibili le modifiche nelle schede orario esistenti, devi eliminare le schede orario generate e generarne di nuove. Questo si applica solo alle schede orario generate associando profili della scheda orario agli utenti.

>[!NOTE]
>
>Le schede orario create manualmente non possono essere ricreate rigenerando le schede orario, a meno che gli utenti non siano stati associati a un profilo di scheda orario da quando la scheda orario è stata creata manualmente. L’eliminazione di una scheda orario creata manualmente può causare la perdita di dati. Per informazioni sulla creazione di una singola scheda orario, vedere [Creare una scheda orario monouso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Gli amministratori di Adobe Workfront o di gruppi possono generare schede orario per tutti gli utenti del sistema. Per ulteriori informazioni sulla generazione manuale delle schede orario, consulta:

* [Genera manualmente i timesheet](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Creare e gestire i profili delle schede orario di un gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Non puoi recuperare una scheda orario eliminata.
>* È consigliabile non eliminare le schede orario passate perché non vengono generate automaticamente in base ai profili delle schede orario. È possibile eliminare le schede attività correnti e future e generarle manualmente se si desidera che le modifiche apportate ai profili delle schede attività siano immediatamente visibili nelle nuove schede attività.
>* Quando elimini le schede orario, le ore registrate per attività, problemi e progetti non vengono eliminate. Solo le Ore Generali vengono eliminate con la scheda orario. In un editor di testo separato, annota le ore generali associate alla scheda orario. Una volta eliminata la scheda orario, puoi registrarla nella nuova scheda orario.
>

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
   <td> <p>È necessario disporre dell'accesso amministrativo alle schede orario. </p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Eliminare le schede orario in un elenco

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **Schede orario**. Il filtro **All** è selezionato per impostazione predefinita e visualizza tutte le schede orario per le quali si dispone dell&#39;accesso.

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

1. Seleziona una o più schede orario da eliminare e fai clic sull&#39;icona **Elimina** ![](assets/delete.png) nella parte superiore dell&#39;elenco delle schede orario.

1. Fare clic su **Elimina**.

   Le schede orario selezionate vengono eliminate e non possono essere recuperate.

   Per generare nuove schede orario, accertati che gli utenti siano associati a un profilo di scheda orario e chiedi all’amministratore di Workfront o a un amministratore di gruppo di generare nuove schede orario.

   Per ulteriori informazioni, vedi:

   * [Crea, modifica e assegna profili scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Genera manualmente le schede orario](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Creare e gestire i profili delle schede orario di un gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Eliminare una scheda orario dalla pagina della scheda orario

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del [!UICONTROL **menu principale**] nell&#39;angolo superiore destro di Adobe Workfront.
1. Fai clic sulla scheda orario da eliminare per aprirla.
1. Fai clic sull&#39;icona [!UICONTROL **Altro**] ![](assets/more-icon.png) a destra del nome della scheda orario, quindi fai clic su **Elimina**.

   ![Elimina scheda orario dalla pagina della scheda orario](assets/delete-timesheet-from-timesheet-page.png)
1. Fai clic su [!UICONTROL **Elimina**] per confermare.

   La scheda orario viene eliminata e non può essere recuperata.

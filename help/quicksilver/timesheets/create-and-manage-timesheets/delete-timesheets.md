---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminare i fogli presenze in Adobe Workfront
description: Le modifiche apportate a un profilo foglio presenze non sono immediatamente effettive per i fogli presenze esistenti, come spiegato in Creazione, modifica e assegnazione di profili foglio presenze. Per rendere le modifiche visibili sui fogli presenze esistenti, è necessario eliminare i fogli presenze generati e generarne di nuovi. Ciò si applica solo ai fogli presenze generati associando profili della scheda attività agli utenti.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Eliminare i fogli presenze in Adobe Workfront

Le modifiche apportate a un profilo foglio presenze non sono immediatamente effettive per i fogli presenze esistenti, come spiegato in [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Per rendere le modifiche visibili sui fogli presenze esistenti, è necessario eliminare i fogli presenze generati e generarne di nuovi. Ciò si applica solo ai fogli presenze generati associando profili della scheda attività agli utenti.

>[!NOTE]
>
>Le schede attività create manualmente non possono essere ricreate rigenerando le schede attività, a meno che gli utenti non siano stati associati a un profilo della scheda attività dalla creazione manuale della scheda attività. L&#39;eliminazione di una scheda attività creata manualmente può causare la perdita di dati. Per informazioni sulla creazione di un foglio presenze singolo, consulta [Creare una scheda attività a uso singolo](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Gli amministratori di Adobe Workfront o gli amministratori di gruppo possono generare fogli ore per tutti gli utenti del sistema. Per ulteriori informazioni sulla generazione manuale dei fogli ore, consulta:

* [Generare manualmente fogli presenze](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Creare e gestire i profili della scheda attività di un gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Impossibile recuperare una scheda attività eliminata.
>* È consigliabile non eliminare i fogli presenze passati perché non vengono generati automaticamente in base ai profili della scheda attività. È possibile eliminare le schede attività correnti e future e generarle manualmente se si desidera che le modifiche ai profili delle schede attività siano immediatamente visibili nelle nuove schede attività.
>* Quando si eliminano i fogli ore, le ore registrate rispetto a attività, problemi e progetti non vengono eliminate. Con la scheda attività vengono cancellate solo le ore generali. In un editor di testo separato, annotare gli orari generali associati alla scheda attività. Una volta eliminata la scheda attività, è possibile registrarla nella nuova scheda attività.
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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario disporre dell’accesso amministrativo ai fogli presenze. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Eliminare i fogli presenze in un elenco

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Schede temporali**. La **Tutto** Il filtro è selezionato per impostazione predefinita e visualizza tutti i fogli presenze a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco dei fogli presenze, effettuare una delle seguenti operazioni:

   * Seleziona **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

      Oppure

      Seleziona **Fogli orari personali** per visualizzare solo i fogli presenze.

      Questo applica le approvazioni della scheda attività personale o i filtri della scheda attività personale all&#39;elenco dei fogli presenze.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   Le opzioni Approvazioni schede attività personali e Pagine attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo hanno rimosso le approvazioni della scheda attività personale e i filtri della scheda attività personale dai controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facoltativo) Fai clic sul pulsante **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diversi o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, visualizzazioni o raggruppamenti, consulta i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona uno o più fogli presenze da eliminare e fai clic sul pulsante **Elimina**  ![](assets/delete.png) nella parte superiore dell’elenco dei fogli presenze.

1. Fai clic su **Elimina**.

   I fogli presenze selezionati vengono eliminati e non possono essere recuperati.

   Per generare nuovi fogli presenze, assicurarsi che gli utenti siano associati a un profilo della scheda attività e chiedere all&#39;amministratore di Workfront o a un amministratore di gruppo di generare nuovi fogli presenze.

   Per ulteriori informazioni, consulta quanto segue:

   * [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Generare manualmente fogli presenze](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Creare e gestire i profili della scheda attività di un gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Elimina una scheda attività dalla pagina della scheda attività

1. Fai clic sul pulsante [!UICONTROL **Menu principale**] icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fare clic sulla scheda attività che si desidera eliminare per aprirla.
1. Fai clic sul pulsante [!UICONTROL **Altro**] icona ![](assets/more-icon.png) a destra del nome della scheda attività, quindi fare clic su **Elimina**.

   ![Elimina scheda attività dalla pagina della scheda attività](assets/delete-timesheet-from-timesheet-page.png)
1. Fai clic su [!UICONTROL **Elimina**] per confermare.

   La scheda attività viene eliminata e non può essere recuperata.

---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e gestire i profili della scheda attività di un gruppo
description: Quando si visualizza un gruppo gestito nell'area Gruppi, è possibile visualizzare e utilizzare i profili della scheda attività per i quali gli amministratori del gruppo o di uno dei relativi sottogruppi hanno accesso amministrativo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Creare e gestire i profili della scheda attività di un gruppo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Quando si visualizza un gruppo gestito nell&#39;area Gruppi, è possibile visualizzare e utilizzare i profili della scheda attività per i quali gli amministratori del gruppo o di uno dei relativi sottogruppi hanno accesso amministrativo.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario essere un amministratore del gruppo.</p>  <p>È inoltre necessario disporre dell’accesso amministrativo ai fogli presenze. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p>  <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare e modificare profili della scheda attività a livello di gruppo

È possibile creare e modificare i profili della scheda attività da utilizzare in un gruppo gestito. Per istruzioni, consulta [Creare, modificare e assegnare profili della scheda attività](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Elimina profili foglio presenze a livello di gruppo

È possibile eliminare i profili della scheda attività utilizzati da un gruppo gestito. Per istruzioni, consulta [Elimina profili foglio presenze](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Generare manualmente fogli presenze di gruppo

Per abilitare le modifiche apportate ai profili della scheda attività del gruppo in modo che si riflettano nei fogli presenze del gruppo corrente, è innanzitutto necessario eliminare i fogli presenze esistenti e quindi generarne manualmente nuovi. Per istruzioni, consulta [Generare manualmente i fogli ore dall’area Timesheets &amp; Hours](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Generare manualmente fogli presenze](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Per informazioni sull&#39;eliminazione dei fogli presenze di gruppo, vedere [Eliminare i fogli presenze in Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Esporta profili foglio presenze a livello di gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).
1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo con i profili della scheda attività che si desidera esportare.
1. Fai clic su **Profili scheda attività**.
1. Fai clic su **Esporta** per esportare l&#39;elenco dei profili della scheda attività per il gruppo.

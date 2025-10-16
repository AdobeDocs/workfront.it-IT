---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e gestire i profili delle schede orario di un gruppo
description: Quando si visualizza un gruppo gestito nell'area Gruppi, è possibile visualizzare e utilizzare i profili delle schede attività per i quali gli amministratori del gruppo o di uno dei suoi sottogruppi dispongono dell'accesso amministrativo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Creare e gestire i profili delle schede orario di un gruppo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Quando si visualizza un gruppo gestito nell&#39;area Gruppi, è possibile visualizzare e utilizzare i profili delle schede attività per i quali gli amministratori del gruppo o di uno dei suoi sottogruppi dispongono dell&#39;accesso amministrativo.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

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
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</p>
   <p>È inoltre necessario disporre dell'accesso amministrativo alle schede orario.</p></td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare e modificare i profili delle schede orario a livello di gruppo

Puoi creare e modificare i profili delle schede orario da utilizzare in un gruppo che gestisci. Per istruzioni, vedere [Creare, modificare e assegnare profili scheda orario](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Elimina profili scheda orario a livello di gruppo

Puoi eliminare i profili delle schede orario in uso da un gruppo che gestisci. Per istruzioni, consulta [Eliminare i profili della scheda orario](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Genera manualmente i Timesheet del gruppo

Per consentire alle modifiche apportate ai profili delle schede orario di gruppo di rispecchiare le schede orario del gruppo corrente, devi prima eliminare le schede orario esistenti e quindi generarne manualmente di nuove. Per istruzioni, vedere [Generare manualmente i Timesheets dalla sezione Timesheets &amp; Hours](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Generare manualmente i Timesheets](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Per informazioni sull&#39;eliminazione dei Timesheets di gruppo, vedere [Eliminare i Timesheets in Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Esporta profili scheda orario a livello di gruppo

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fai clic sul nome del gruppo con i profili della scheda orario che desideri esportare.
1. Fare clic su **Profili scheda orario**.
1. Fai clic su **Esporta** per esportare l&#39;elenco dei profili delle schede orario per il gruppo.

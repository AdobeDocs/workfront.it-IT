---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Genera manualmente i timesheet
description: Per consentire alle modifiche apportate ai profili delle schede orario di essere visibili nelle schede orario correnti, devi prima eliminare le schede orario esistenti e quindi generarne manualmente di nuove. È possibile generare manualmente le schede orario dall’area Schede orario o Diagnostica in Configurazione, come spiegato in questo articolo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 311816df863d3c03a54d43c8fa3cac69d2d6d7d4
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Genera manualmente i timesheet

Per consentire alle modifiche apportate ai profili delle schede orario di essere visibili nelle schede orario correnti, devi prima eliminare le schede orario esistenti e quindi generarne manualmente di nuove. È possibile generare manualmente le schede orario dall’area Schede orario o Diagnostica in Configurazione, come spiegato in questo articolo.

Per istruzioni sull&#39;eliminazione delle schede orario, vedere [Elimina schede orario in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
   <td> <p>Devi essere un amministratore di Workfront oppure, se lavori sui profili delle schede orario per un gruppo, un amministratore di gruppo (o un amministratore di Workfront). Per ulteriori informazioni, vedere <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a>.</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulle schede orario generate manualmente

Quando generi manualmente le schede orario:

* Vengono generati in base ai profili della scheda orario associati ai tuoi utenti. Gli utenti a cui non sono associati profili della scheda orario non ricevono le schede orario.
* Vengono generate solo la scheda orario corrente e quella successiva. Workfront non genera due schede orario per lo stesso periodo. Se disponi già di una scheda orario per l’arco temporale corrente, un’altra non verrà generata quando utilizzi il processo manuale per generare le schede orario.

## Genera manualmente i Timesheets dalla sezione Timesheets &amp; Hours (Schede orario e ore)

Puoi generare manualmente schede orario a livello di sistema o di gruppo dall’area Schede orario e ore in Configurazione.

1. Fai clic sull&#39;icona **del** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Se stai generando le schede orario in uso in tutto il sistema, fai clic su **Schede orario e ore.**

   Oppure

   Se stai generando schede orario utilizzate da un gruppo specifico, fai clic su **Gruppi**, quindi fai clic sul nome del gruppo.

1. Fare clic su **Profili scheda orario**.
1. Fai clic sull&#39;icona Altro ![icona Altro](assets/more-icon.png), quindi **Genera schede orario**.

1. Nella parte superiore dell&#39;elenco dei profili della scheda orario, fare clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) per i profili della scheda orario a livello di sistema oppure **Altro** per i profili della scheda orario di gruppo, quindi fare clic su **Genera schede orario**.

   Le nuove schede orario vengono create per un massimo di due periodi di tempo per gli utenti associati ai profili delle schede orario.

## Genera manualmente schede orario a livello di sistema dall&#39;area Diagnostica

È possibile generare manualmente schede orario a livello di sistema dall&#39;area Diagnostica in Configurazione.

1. Fai clic sull&#39;icona **del** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandere **Sistema**, quindi fare clic su **Diagnostica**.

1. Fare clic su **Esegui diagnostica**.
1. Fai clic su **Genera schede orario**.

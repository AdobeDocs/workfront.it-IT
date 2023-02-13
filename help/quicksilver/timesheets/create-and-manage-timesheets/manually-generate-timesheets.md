---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generare manualmente fogli presenze
description: Per abilitare le modifiche apportate ai profili della scheda attività affinché riflettano nei fogli presenze correnti, è necessario prima eliminare i fogli presenze esistenti e quindi generarne manualmente nuovi. È possibile generare manualmente i fogli ore dall’area Timesheets o dall’area Diagnostics in Setup, come spiegato in questo articolo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Generare manualmente fogli presenze

Per abilitare le modifiche apportate ai profili della scheda attività affinché riflettano nei fogli presenze correnti, è necessario prima eliminare i fogli presenze esistenti e quindi generarne manualmente nuovi. È possibile generare manualmente i fogli ore dall’area Timesheets o dall’area Diagnostics in Setup, come spiegato in questo articolo.

Per istruzioni sull&#39;eliminazione dei fogli presenze, consulta [Eliminare i fogli presenze in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

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
   <td> <p>È necessario essere un amministratore di Workfront oppure, se si lavora sui profili della scheda attività per un gruppo, è necessario essere un amministratore di gruppo (o un amministratore Workfront). Per ulteriori informazioni, consulta <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a>.</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sui fogli presenze generati manualmente

Quando si generano manualmente fogli presenze:

* Vengono generati in base ai profili della scheda attività associati agli utenti. Gli utenti a cui non sono associati profili della scheda attività non ricevono fogli presenze. 
* Vengono generati solo la scheda attività corrente e quella da seguire. Workfront non genera due fogli presenze per lo stesso periodo. Se si dispone già di una scheda attività per un intervallo di tempo specifico, un&#39;altra non verrà generata quando si utilizza il processo manuale per generare fogli presenze.

## Generare manualmente i fogli ore dall’area Timesheets &amp; Hours

Puoi generare manualmente fogli presenze a livello di sistema o di gruppo dall’area Timesheets &amp; Hours in Configurazione.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Se si generano fogli presenze in uso in tutto il sistema, fare clic su **Tempi e ore.**

   Oppure

   Se si generano fogli presenze utilizzati da un gruppo specifico, fare clic su **Gruppi**, quindi fai clic sul nome del gruppo.

1. Fai clic su **Profili scheda attività**.
1. Fai clic su **Altro**, quindi **Genera fogli presenze**.

   I nuovi fogli presenze vengono creati per un massimo di due periodi di tempo per gli utenti associati ai profili della scheda attività.

## Generare manualmente fogli presenze a livello di sistema dall&#39;area Diagnostics

È possibile generare manualmente fogli presenze a livello di sistema dall&#39;area Diagnostica in Configurazione.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandi **Sistema**, quindi fai clic su **Diagnostica**.

1. Fai clic su **Diagnostica di condotta**. 
1. Fai clic su **Genera fogli presenze**.

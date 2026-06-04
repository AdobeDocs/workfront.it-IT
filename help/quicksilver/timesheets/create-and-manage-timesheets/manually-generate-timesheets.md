---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generare manualmente schede orario
description: Per consentire alle modifiche apportate ai profili delle schede orario di essere visibili nelle schede orario correnti, devi prima eliminare le schede orario esistenti e quindi generarne manualmente di nuove. È possibile generare manualmente le schede orario dall’area Schede orario o Diagnostica in Configurazione, come spiegato in questo articolo.
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
TQID: https://experienceleague.adobe.com/0hU3VlHM8l5TXee6K3lJaV9-W3ZKujDYf9-f1NXH-Nc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 9%

---

# Generare manualmente schede orario

Per consentire alle modifiche apportate ai profili delle schede orario di essere visibili nelle schede orario correnti, devi prima eliminare le schede orario esistenti e quindi generarne manualmente di nuove. È possibile generare manualmente le schede orario dall’area Schede orario o Diagnostica in Configurazione, come spiegato in questo articolo.

Per istruzioni sull&#39;eliminazione delle schede orario, vedere [Elimina schede orario in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Devi essere un amministratore di Workfront oppure, se lavori sui profili delle schede orario per un gruppo, un amministratore di gruppo (o un amministratore di Workfront).</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulle schede orario generate manualmente

Quando generi manualmente le schede orario:

* Vengono generati in base ai profili della scheda orario associati ai tuoi utenti. Gli utenti a cui non sono associati profili della scheda orario non ricevono le schede orario.
* Vengono generate solo la scheda orario corrente e quella successiva. Workfront non genera due schede orario per lo stesso periodo. Se disponi già di una scheda orario per l’arco temporale corrente, un’altra non verrà generata quando utilizzi il processo manuale per generare le schede orario.

## Genera manualmente i Timesheets dalla sezione Timesheets &amp; Hours (Schede orario e ore)

Puoi generare manualmente schede orario a livello di sistema o di gruppo dall’area Schede orario e ore in Configurazione.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Se stai generando le schede orario in uso in tutto il sistema, fai clic su **Schede orario e ore.**

   Oppure

   Se stai generando schede orario utilizzate da un gruppo specifico, fai clic su **Gruppi**, quindi fai clic sul nome del gruppo.

1. Fare clic su **Profili scheda orario**.
1. Fai clic sull&#39;icona Altro ![icona Altro](assets/more-icon.png), quindi **Genera schede orario**.

1. Nella parte superiore dell&#39;elenco dei profili della scheda orario, fare clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) per i profili della scheda orario a livello di sistema oppure **Altro** per i profili della scheda orario di gruppo, quindi fare clic su **Genera schede orario**.

   Le nuove schede orario vengono create per un massimo di due periodi di tempo per gli utenti associati ai profili delle schede orario.

## Genera manualmente schede orario a livello di sistema dall&#39;area Diagnostica

È possibile generare manualmente schede orario a livello di sistema dall&#39;area Diagnostica in Configurazione.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandere **Sistema**, quindi fare clic su **Diagnostica**.

1. Fare clic su **Esegui diagnostica**.
1. Fai clic su **Genera schede orario**.

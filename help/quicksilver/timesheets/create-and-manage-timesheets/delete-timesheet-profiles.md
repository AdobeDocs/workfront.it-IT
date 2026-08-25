---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminare profili di timesheet
description: Puoi eliminare un profilo di scheda orario che potrebbe non essere più rilevante.
author: Lisa
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
source-git-commit: 0a3a49ff0e6347e0a0b327fcd692d5e1d9598f08
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 18%

---

# Eliminare profili di timesheet

<!--Audited:6/2025-->

La creazione e l’assegnazione di profili della scheda orario agli utenti garantisce la coerenza nella creazione delle schede orario da parte di Adobe Workfront.

Puoi eliminare un profilo di scheda orario che potrebbe non essere più rilevante.

Per informazioni sui profili delle schede orario, vedere [Creare, modificare e assegnare profili delle schede orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td><p>Accesso amministrativo alle schede orario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare profili di timesheet

{{step-1-to-setup}}

1. Se si elimina un profilo di scheda orario a livello di sistema, fare clic su **Schede orario e ore > Profili scheda orario**.

   Oppure

   Se si sta eliminando un profilo di scheda orario per un gruppo, fare clic su **Gruppi** > fare clic sul nome del gruppo, quindi fare clic su **Profili scheda orario**.

1. Per il livello di sistema, seleziona almeno un profilo di scheda orario da eliminare, quindi fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png) > **Elimina**.

   Oppure

   Fai clic su **Altro** > **Elimina** per il profilo della scheda orario a livello di gruppo.

1. (Condizionale) Se il profilo scheda orario è già assegnato agli utenti, viene visualizzata la casella **Profilo scheda orario sostitutivo**. Effettua le seguenti operazioni:
   1. Seleziona un altro profilo di scheda orario dall’elenco a discesa. Il profilo della scheda orario che stai eliminando verrà sostituito dal profilo della scheda orario con cui lo sostituisci per tutti gli utenti assegnati. Le schede orario verranno generate in base al nuovo profilo assegnato nel seguente ciclo di generazione della scheda orario.
   1. Fai clic su **Elimina** per confermare l&#39;eliminazione.

1. (Condizionale) Se il profilo della scheda orario non è assegnato agli utenti, viene visualizzata la casella **Elimina scheda orario**.

   Fai clic su **Elimina** per confermare l&#39;eliminazione.

---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Blocca o sblocca una scheda orario di gruppo e la preferenza dell'ora
description: Se si è un amministratore di gruppo, è possibile configurare e quindi bloccare una scheda orario e una preferenza per le ore per il gruppo dopo che un amministratore di Workfront lo ha sbloccato a livello di sistema.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Blocca o sblocca una preferenza di tipo Timesheet gruppo e Ora

Se si è un amministratore di gruppo, è possibile configurare e quindi bloccare una scheda orario e una preferenza per le ore per il gruppo dopo che un amministratore di Workfront lo ha sbloccato a livello di sistema.

Il blocco di una preferenza Adobe Workfront garantisce che tutti gli utenti del gruppo e dei relativi sottogruppi utilizzino la stessa impostazione per tale preferenza. Anche se è ancora possibile riconfigurare una preferenza bloccata, gli amministratori dei gruppi non possono farlo per i sottogruppi inferiori.

Al contrario, sbloccare una preferenza a livello di gruppo consente agli amministratori dei sottogruppi una maggiore flessibilità per gestire il modo in cui i loro gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppi possono riconfigurarla per tali sottogruppi.

Ciò è parallelo alla possibilità che un amministratore di Workfront deve bloccare o sbloccare una preferenza per tutti gli utenti del sistema.

Per informazioni su come un amministratore di Workfront può bloccare o sbloccare una preferenza per le ore e le schede orario per tutti i gruppi del sistema, vedere [Configurare le preferenze per le ore e le schede orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni sulla configurazione di una preferenza di tipo Timesheet e Ora per un gruppo, vedere [Configurare le preferenze di tipo Timesheet e Ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configurazione di una preferenza sbloccata per un gruppo non influisce sulla preferenza per i sottogruppi al di sotto del gruppo.
>
>  Tuttavia, quando viene creato un nuovo sottogruppo, questo eredita le impostazioni di preferenza e lo stato bloccato o sbloccato del gruppo immediatamente superiore.
>
>* Se spostate un gruppo all&#39;interno di un gruppo che ha una preferenza bloccata, il gruppo spostato eredita tale preferenza e viene bloccato per il gruppo spostato.
>* Se spostate un gruppo all&#39;interno di un gruppo che ha una preferenza sbloccata, il gruppo spostato non viene influenzato da tale preferenza.
>
>  Se la preferenza nel gruppo spostato è bloccata al momento dello spostamento, rimane bloccata, ma l&#39;amministratore del gruppo può sbloccarla ora perché è sbloccata per il gruppo padre.

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
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Blocca o sblocca una preferenza di tipo Timesheet gruppo e Ora

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi saltare i passaggi 1-4 da Configurazione > Scheda orario e ore > Preferenze, quindi cercare il nome del gruppo nella casella nella parte superiore della pagina.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Fare clic sul nome del gruppo in cui si desidera bloccare o sbloccare una preferenza di schede orario e ore.
1. Nel pannello a sinistra, fai clic su **Schede orario e preferenze ore**.

1. Nella pagina visualizzata eseguire una delle operazioni seguenti:

   * Se vuoi che gli amministratori dei gruppi al di sotto del gruppo possano configurare una preferenza per i loro gruppi, sbloccarla ![Attiva/Disattiva blocco](assets/unlock-toggle-button.png).
   * Se vuoi che tutti i gruppi al di sotto del tuo utilizzino la configurazione per una preferenza, assicurati che sia bloccata ![Attiva/Disattiva blocco](assets/lock-toggle-button.png) (impostazione predefinita).

     >[!IMPORTANT]
     >
     >È importante comunicare con gli amministratori e gli utenti nei gruppi sottostanti per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata. Quando la blocchi, la configurazione viene ereditata da tutti i sottogruppi sottostanti. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori dei gruppi dei sottogruppi inferiori potrebbero aver effettuato.

1. Fai clic su **Salva**.

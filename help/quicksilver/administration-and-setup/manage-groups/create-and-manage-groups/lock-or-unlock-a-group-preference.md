---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloccare o sbloccare un progetto, un'attività o una preferenza di problema per i sottogruppi
description: In qualità di amministratore di gruppo, è possibile configurare e quindi bloccare un progetto, un'attività o una preferenza di problema se un amministratore di Workfront lo ha sbloccato a livello di sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi

In qualità di amministratore di gruppo, è possibile configurare e quindi bloccare un progetto, un&#39;attività o una preferenza di problema se un amministratore di Workfront lo ha sbloccato a livello di sistema.

Il blocco di un progetto, un&#39;attività o una preferenza di problema configurata a livello di assicura che tutti gli utenti del gruppo e dei relativi sottogruppi utilizzino la stessa impostazione per tale preferenza. Anche se è ancora possibile riconfigurare una preferenza bloccata per il gruppo, gli amministratori del gruppo non possono riconfigurarla per i gruppi.

Al contrario, lo sblocco di un progetto, di un’attività o di una preferenza per un problema consente agli amministratori di gruppo una maggiore flessibilità per gestire il modo in cui i gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppo possono riconfigurarla per tali sottogruppi.

Ciò è parallelo alla possibilità che un amministratore di Workfront debba bloccare o sbloccare una preferenza per tutti gli utenti del sistema.

Per informazioni su come un amministratore di Workfront può bloccare o sbloccare una preferenza per tutti i gruppi del sistema, consulta [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configurazione di una preferenza sbloccata per un gruppo non influisce su tale preferenza per i sottogruppi al di sotto del gruppo.
>
>  Tuttavia, quando viene creato un nuovo sottogruppo, eredita le impostazioni delle preferenze e lo stato bloccato o sbloccato del gruppo immediatamente sopra di esso.
>
>* Se si sposta un gruppo sotto un gruppo con una preferenza bloccata, il gruppo spostato eredita tale preferenza ed è bloccato per il gruppo spostato.
>* Se si sposta un gruppo in un gruppo con una preferenza sbloccata, il gruppo spostato non viene interessato da tale preferenza.
>
>  Se la preferenza nel gruppo spostato è bloccata al momento dello spostamento, rimane bloccata, ma l&#39;amministratore del gruppo può sbloccarla ora perché è sbloccata per il gruppo principale.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Bloccare o sbloccare un progetto di gruppo, un&#39;attività o una preferenza di problema

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Fare clic sul nome del gruppo in cui si desidera bloccare o sbloccare una preferenza di progetto.
1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** o **Preferenze relative a operazioni e problemi**.

1. Nella pagina visualizzata, effettua una delle seguenti operazioni per una preferenza sbloccata a livello di sistema o per un gruppo al di sopra del gruppo:

   * Se desideri che gli amministratori dei gruppi al di sotto del tuo gruppo siano in grado di configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che tutti i gruppi al di sotto del tuo per utilizzare la tua configurazione per una preferenza, assicurati che sia bloccata ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >È importante comunicare con gli amministratori e gli utenti dei gruppi indicati di seguito per garantire che tutte le esigenze siano prese in considerazione nel modo in cui configuri una preferenza bloccata. Quando lo blocchi, la configurazione per esso viene ereditata da qualsiasi sottogruppo sottostante. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo nei sottogruppi inferiori potrebbero aver effettuato.

1. Fai clic su **Salva**.

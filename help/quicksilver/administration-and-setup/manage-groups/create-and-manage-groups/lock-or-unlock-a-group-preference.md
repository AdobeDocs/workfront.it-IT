---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloccare o sbloccare una preferenza di progetto, attività o problema per i sottogruppi
description: In qualità di amministratore di gruppo, puoi configurare e quindi bloccare un progetto, un’attività o una preferenza di problema se un amministratore di Workfront lo ha sbloccato a livello di sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Bloccare o sbloccare una preferenza di progetto, attività o problema per i sottogruppi

In qualità di amministratore di gruppo, puoi configurare e quindi bloccare un progetto, un’attività o una preferenza di problema se un amministratore di Workfront lo ha sbloccato a livello di sistema.

Il blocco di un progetto, di un’attività o di una preferenza di problema configurato a livello di garantisce che tutti gli utenti del gruppo e dei relativi sottogruppi utilizzino la stessa impostazione per tale preferenza. Sebbene sia comunque possibile riconfigurare una preferenza bloccata per il gruppo, gli amministratori dei gruppi non possono riconfigurarla per i gruppi.

Al contrario, sbloccare un progetto, un’attività o una preferenza per un problema consente agli amministratori di gruppi di gestire in modo più flessibile il modo in cui i loro gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppi possono riconfigurarla per tali sottogruppi.

Ciò è parallelo alla possibilità che un amministratore di Workfront deve bloccare o sbloccare una preferenza per tutti gli utenti del sistema.

Per informazioni su come un amministratore di Workfront può bloccare o sbloccare una preferenza per tutti i gruppi del sistema, vedere [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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
>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

## Bloccare o sbloccare una preferenza di progetto, attività o problema di gruppo

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Fare clic sul nome del gruppo in cui si desidera bloccare o sbloccare una preferenza di progetto.
1. Nel pannello a sinistra, fai clic su **Preferenze progetto** o **Preferenze attività e problemi**.

1. Nella pagina visualizzata eseguire una delle operazioni seguenti per una preferenza sbloccata a livello di sistema o per un gruppo al di sopra del gruppo:

   * Se desideri che gli amministratori dei gruppi al di sotto del gruppo possano configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che tutti i gruppi al di sotto del tuo utilizzino la tua configurazione per una preferenza, assicurati che sia bloccata ![](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >È importante comunicare con gli amministratori e gli utenti nei gruppi sottostanti per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata. Quando la blocchi, la configurazione viene ereditata da tutti i sottogruppi sottostanti. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori dei gruppi dei sottogruppi inferiori potrebbero aver effettuato.

1. Fai clic su **Salva**.

---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloccare o sbloccare una scheda attività e una preferenza ora del gruppo
description: Se si è un amministratore di gruppo, è possibile configurare e quindi bloccare una scheda attività e una preferenza oraria per il gruppo dopo che un amministratore di Workfront lo sblocca a livello di sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Bloccare o sbloccare una scheda attività e una preferenza ora del gruppo

Se si è un amministratore di gruppo, è possibile configurare e quindi bloccare una scheda attività e una preferenza oraria per il gruppo dopo che un amministratore di Workfront lo sblocca a livello di sistema.

Il blocco di una preferenza Adobe Workfront garantisce che tutti gli utenti del gruppo e dei sottogruppi utilizzino la stessa impostazione per tale preferenza. Anche se è ancora possibile riconfigurare una preferenza bloccata, gli amministratori dei gruppi non possono farlo per i sottogruppi inferiori.

Al contrario, lo sblocco di una preferenza a livello di gruppo consente agli amministratori dei sottogruppi di gestire in modo più flessibile il modo in cui i gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppo possono riconfigurarla per tali sottogruppi.

Ciò è parallelo alla possibilità che un amministratore di Workfront debba bloccare o sbloccare una preferenza per tutti gli utenti del sistema.

Per informazioni su come un amministratore di Workfront può bloccare o sbloccare una scheda attività e le preferenze orarie per tutti i gruppi del sistema, vedere [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni sulla configurazione di una scheda attività e delle preferenze orarie per un gruppo, vedere [Configurare le preferenze relative a schede attività e ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## Bloccare o sbloccare una scheda attività e una preferenza ora del gruppo

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi ignorare i passaggi 1-4 andando su Configurazione > Scheda attività e ore > Preferenze, quindi cercando il nome del gruppo nella casella nella parte superiore della pagina.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Fare clic sul nome del gruppo in cui si desidera bloccare o sbloccare le preferenze relative a fogli presenze e ore.
1. Nel pannello a sinistra, fai clic su **Preferenze per fogli orari e ore**.

1. Nella pagina visualizzata, effettuare una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi al di sotto del tuo gruppo siano in grado di configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che tutti i gruppi al di sotto del tuo per utilizzare la tua configurazione per una preferenza, assicurati che sia bloccata ![](assets/lock-toggle-button.png) (questa è l’impostazione predefinita).

      >[!IMPORTANT]
      >
      >È importante comunicare con gli amministratori e gli utenti dei gruppi indicati di seguito per garantire che tutte le esigenze siano prese in considerazione nel modo in cui configuri una preferenza bloccata. Quando lo blocchi, la configurazione per esso viene ereditata da qualsiasi sottogruppo sottostante. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo nei sottogruppi inferiori potrebbero aver effettuato.

1. Fai clic su **Salva**.

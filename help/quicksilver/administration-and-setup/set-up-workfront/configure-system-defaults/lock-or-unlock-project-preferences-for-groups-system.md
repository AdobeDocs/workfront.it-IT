---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Blocca o sblocca le preferenze di progetto per tutti i gruppi nel sistema
description: I gruppi dell’organizzazione potrebbero aver bisogno di una preferenza di progetto configurata in modo diverso per i loro flussi di lavoro univoci. Puoi sbloccare la preferenza per tutti i gruppi dell’organizzazione in modo che possano configurarla autonomamente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 3e97df265df83965d094d8723fe76043ff4af80e
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Blocca o sblocca le preferenze di progetto per tutti i gruppi nel sistema

I gruppi dell’organizzazione potrebbero aver bisogno di una preferenza di progetto configurata in modo diverso per i loro flussi di lavoro univoci. Puoi sbloccare la preferenza per tutti i gruppi dell’organizzazione in modo che possano configurarla autonomamente.

Quando una preferenza viene sbloccata e l&#39;amministratore del gruppo la modifica, i progetti associati al gruppo acquisiscono la configurazione per tale preferenza dall&#39;impostazione a livello di gruppo anziché dall&#39;impostazione a livello di sistema.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Preferenze bloccate e sbloccate

Il blocco di un progetto, di un’attività o di una preferenza di problema configurato a livello di sistema garantisce che tutti utilizzino la stessa impostazione per tale preferenza. Sebbene sia ancora possibile riconfigurare una preferenza bloccata, gli amministratori dei gruppi non possono riconfigurarla per i propri gruppi.

Al contrario, sbloccare un progetto, un’attività o una preferenza per un problema consente agli amministratori di gruppi di gestire in modo più flessibile il modo in cui i loro gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppi possono riconfigurarla per i loro gruppi.

Se un campo non dispone di un interruttore di blocco/sblocco, non può essere sbloccato per consentire agli amministratori di gruppi di configurare le impostazioni a livello di gruppo. Configurazione disponibile solo a livello di sistema.

Per istruzioni su come bloccare o sbloccare un progetto, un’attività o una preferenza per un problema a livello di sistema, vedi [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Dopo un [!DNL Workfront] l’amministratore sblocca una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per garantire che tutti gli utenti del gruppo e i sottogruppi sottostanti utilizzino la stessa configurazione. Questo è parallelo alla capacità che un [!DNL Workfront] l’amministratore deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloccare o sbloccare una preferenza di progetto, attività o problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Sbloccare una preferenza di progetto in modo che i gruppi possano configurarla

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Preferenze progetto]**, quindi fai clic su **[!UICONTROL Progetti]**.

1. Effettua una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi possano configurare una preferenza per i loro gruppi, sbloccalo ![](assets/unlock-toggle-button.png).
   * Se si desidera che tutti i gruppi utilizzino la configurazione per una preferenza, assicurarsi che sia bloccata (impostazione predefinita).

     >[!IMPORTANT]
     >
     >È consigliabile comunicare con gli amministratori e gli utenti in gruppi in tutto il sistema per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata. Quando la blocchi, la configurazione viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.

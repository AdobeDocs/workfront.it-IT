---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema
description: I gruppi dell’organizzazione potrebbero aver bisogno di una preferenza di progetto configurata in modo diverso per i flussi di lavoro univoci. È possibile sbloccare la preferenza per tutti i gruppi all’interno dell’organizzazione in modo che possano configurarla autonomamente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema

I gruppi dell’organizzazione potrebbero aver bisogno di una preferenza di progetto configurata in modo diverso per i flussi di lavoro univoci. È possibile sbloccare la preferenza per tutti i gruppi all’interno dell’organizzazione in modo che possano configurarla autonomamente.

Quando una preferenza viene sbloccata e l’amministratore del gruppo la modifica, i progetti associati al gruppo acquisiscono la configurazione di tale preferenza dall’impostazione a livello di gruppo anziché dall’impostazione a livello di sistema.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sulle preferenze bloccate e sbloccate

Il blocco di un progetto, un&#39;attività o una preferenza di problema configurata a livello di sistema garantisce che tutti utilizzino la stessa impostazione per tale preferenza. Anche se è ancora possibile riconfigurare una preferenza bloccata, gli amministratori dei gruppi non possono riconfigurarla per i loro gruppi.

Al contrario, lo sblocco di un progetto, di un’attività o di una preferenza per un problema consente agli amministratori di gruppo una maggiore flessibilità per gestire il modo in cui i gruppi lavorano con tali elementi. Quando una preferenza viene sbloccata, gli amministratori di gruppo possono riconfigurarla per i propri gruppi.

Per istruzioni su come bloccare o sbloccare un progetto, un task o una preferenza di problema a livello di sistema, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Dopo un [!DNL Workfront] l’amministratore sblocca una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per garantire che tutti i membri del proprio gruppo e dei sottogruppi sottostanti utilizzino la stessa configurazione. Ciò è parallelo alla capacità di un [!DNL Workfront] l’amministratore deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Sblocca una preferenza di progetto in modo che i gruppi possano configurarla

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Preferenze del progetto]**, quindi fai clic su **[!UICONTROL Progetti]**.

1. Effettua una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi siano in grado di configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che tutti i gruppi utilizzino la configurazione per una preferenza, accertati che sia bloccata (questa è l’impostazione predefinita).

      >[!IMPORTANT]
      >
      >È consigliabile comunicare con gli amministratori e gli utenti di gruppi in tutto il sistema per garantire che tutte le esigenze siano prese in considerazione nel modo in cui si configura una preferenza bloccata. Quando lo si blocca, la configurazione per esso viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.

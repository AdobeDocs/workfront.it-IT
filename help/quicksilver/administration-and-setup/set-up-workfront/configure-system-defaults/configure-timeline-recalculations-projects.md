---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurare i calcoli della timeline per i progetti
description: Il ricalcolo delle timeline consente ai responsabili di vedere in che modo le forze esterne al progetto influiscono sulla timeline del progetto. La timeline di un progetto si riferisce alle date pianificate e previste per il progetto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Configurare i calcoli della timeline per i progetti

Il ricalcolo delle timeline consente ai responsabili di vedere in che modo le forze esterne al progetto influiscono sulla timeline del progetto. La timeline di un progetto si riferisce alle date pianificate e previste per il progetto.

Come [!DNL Adobe Workfront] amministratore, puoi ricalcolare manualmente le timeline per tutti i progetti nel sistema. I proprietari dei progetti possono inoltre ricalcolare manualmente le timeline per i singoli progetti. Per ulteriori informazioni, consulta [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Questo articolo descrive come [!DNL Workfront] amministratore, può determinare come e quando [!DNL Workfront] calcola automaticamente le timeline del progetto configurando le preferenze del progetto nel [!UICONTROL Configurazione] area.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td> <p>Livello di accesso dell'amministratore di sistema</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare i ricalcoli automatici

Come [!DNL Adobe Workfront] amministratore, puoi configurare quando [!DNL Workfront] ricalcola automaticamente le timeline del progetto. [!DNL Workfront] può ricalcolare le timeline del progetto ogni notte o quando l’ambito del progetto cambia, oppure entrambe.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Preferenze del progetto]** > **[!UICONTROL Progetti].**

1. In **[!UICONTROL Timeline]** abilitare o disabilitare una o entrambe le impostazioni riportate di seguito. Per impostazione predefinita, entrambe le impostazioni sono abilitate.

   * **Ogni notte:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] ricalcola le tempistiche di notte solo per i progetti con stato [!UICONTROL Corrente] e sono stati aggiornati negli ultimi tre mesi.

      In questo caso, [!DNL Workfront] ricalcola la timeline per tutti i progetti con un [!UICONTROL Tipo di aggiornamento] di [!UICONTROL Automatico] o [!UICONTROL Automatico e On Change].

   * **Quando l’ambito di un progetto cambia**: Per informazioni sulla modifica dell’ambito di un progetto, consulta [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      In questo caso, [!DNL Workfront] ricalcola la timeline per tutti i progetti con un tipo di aggiornamento [!UICONTROL Automatico e On Change] o [!UICONTROL Solo su modifica].
Per informazioni sui tipi di aggiornamento dei progetti, consulta [Panoramica sul tipo di aggiornamento del progetto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Fai clic su **[!UICONTROL Salva]**.

   La timeline di tutti i progetti nel sistema viene ricalcolata automaticamente in base al tipo di aggiornamento di ciascun progetto.

## Ricalcolare le timeline per l’intero [!DNL Workfront] istanza

Puoi eseguire il [!UICONTROL Ricalcola timeline] diagnostica per ricalcolare manualmente tutte le timeline nel [!DNL Workfront] sistema. Questo consente a tutti i project manager di vedere immediatamente l’influenza dei cambiamenti esterni sia sulle date pianificate che su quelle previste. Per ulteriori informazioni, consulta [Utilizzare Diagnostica per attivare i processi automatizzati](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).

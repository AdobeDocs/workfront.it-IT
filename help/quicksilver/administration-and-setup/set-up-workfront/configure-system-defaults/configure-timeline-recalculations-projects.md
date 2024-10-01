---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurare i ricalcoli della sequenza temporale per i progetti
description: Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 7c2d6d1960752a109c02039c1af8d1d1850bcb8c
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configurare i ricalcoli della sequenza temporale per i progetti

Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.

In qualità di amministratore [!DNL Adobe Workfront], puoi ricalcolare manualmente le timeline per tutti i progetti nel sistema. I proprietari dei progetti possono inoltre ricalcolare manualmente le tempistiche per i singoli progetti. Per ulteriori informazioni, vedere [Ricalcolare i timeline del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Questo articolo descrive come l&#39;amministratore di [!DNL Workfront] può determinare come e quando [!DNL Workfront] calcola automaticamente le sequenze temporali del progetto configurando le preferenze del progetto nell&#39;area [!UICONTROL Configurazione].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare i ricalcoli automatici

In qualità di amministratore [!DNL Adobe Workfront], puoi configurare quando [!DNL Workfront] ricalcola automaticamente le timeline del progetto. [!DNL Workfront] può ricalcolare le sequenze temporali del progetto ogni notte o quando l&#39;ambito del progetto cambia, o entrambe.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Progetti].**

1. Nella sezione **[!UICONTROL Timeline]**, abilita o disabilita una o entrambe le impostazioni seguenti. Per impostazione predefinita, entrambe le impostazioni sono abilitate.

   * **Ogni notte:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] ricalcola le sequenze temporali una volta ogni 24 ore, di notte, solo per i progetti con stato [!UICONTROL Corrente] e che sono stati aggiornati negli ultimi tre mesi. A seconda del carico del sistema e di altri fattori, il tempo di ricalcolo potrebbe essere ritardato di oltre 24 ore.

     In questo caso, [!DNL Workfront] ricalcola la sequenza temporale per tutti i progetti con tipo di aggiornamento [!UICONTROL Update] di [!UICONTROL Automatic] o [!UICONTROL Automatic e On Change].

   * **Quando l&#39;ambito di un progetto cambia**: per informazioni su ciò che costituisce una modifica dell&#39;ambito di un progetto, vedere [Ricalcolare le timeline del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In questo caso, [!DNL Workfront] ricalcola la sequenza temporale per tutti i progetti con tipo di aggiornamento [!UICONTROL Automatico e alla modifica] o [!UICONTROL Solo alla modifica].
Per informazioni sui tipi di aggiornamento del progetto, vedere [Panoramica sul tipo di aggiornamento del progetto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Fai clic su **[!UICONTROL Salva]**.

   La timeline di tutti i progetti nel sistema viene ricalcolata automaticamente in base al Tipo di aggiornamento di ciascun progetto.

>[!IMPORTANT]
>
>Per gli ambienti Sandbox di anteprima e aggiornamento personalizzato, il ricalcolo notturno è disattivato e le timeline del progetto non vengono ricalcolate automaticamente. Devi ricalcolare manualmente la timeline del progetto per gli ambienti Sandbox di anteprima e aggiornamento personalizzati. Per informazioni, vedere [Ricalcolare i timeline del progetto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Ricalcola le timeline per l&#39;intera istanza [!DNL Workfront]

È possibile eseguire la diagnostica [!UICONTROL Ricalcola timeline] per ricalcolare manualmente tutte le timeline nel sistema [!DNL Workfront]. Questo consente a tutti i project manager di visualizzare immediatamente l&#39;influenza di modifiche esterne sia nelle date pianificate che in quelle previste. Per ulteriori informazioni, vedere [Utilizzare Diagnostica per attivare i processi automatizzati](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).

---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurare i ricalcoli della sequenza temporale per i progetti
description: Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Configurare i ricalcoli della sequenza temporale per i progetti

Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.

Come un [!DNL Adobe Workfront] amministratore, puoi ricalcolare manualmente le timeline per tutti i progetti nel sistema. I proprietari dei progetti possono inoltre ricalcolare manualmente le tempistiche per i singoli progetti. Per ulteriori informazioni, consulta [Ricalcolare i timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Questo articolo descrive come [!DNL Workfront] , può determinare come e quando [!DNL Workfront] calcola automaticamente le sequenze temporali del progetto configurando le preferenze del progetto nel [!UICONTROL Configurazione] area.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Livello di accesso amministratore di sistema</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare i ricalcoli automatici

Come un [!DNL Adobe Workfront] amministratore, puoi configurare quando [!DNL Workfront] ricalcola automaticamente le timeline del progetto. [!DNL Workfront] può ricalcolare le sequenze temporali del progetto ogni notte o quando l’ambito del progetto cambia, oppure entrambe.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro o [!UICONTROL **Menu principale**] icona ![](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro di [!DNL Workfront], se disponibile, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Progetti].**

1. In **[!UICONTROL Timeline]** , attivare o disattivare una o entrambe le impostazioni seguenti. Per impostazione predefinita, entrambe le impostazioni sono abilitate.

   * **Ogni notte:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] ricalcola le sequenze temporali una volta ogni 24 ore, di notte, solo per i progetti con stato [!UICONTROL Corrente] e che sono state aggiornate negli ultimi tre mesi. A seconda del carico del sistema e di altri fattori, il tempo di ricalcolo potrebbe essere ritardato di oltre 24 ore.

     In questo caso, [!DNL Workfront] ricalcola la timeline per tutti i progetti che hanno un [!UICONTROL Tipo di aggiornamento] di [!UICONTROL Automatico] o [!UICONTROL Automatico e in caso di modifica].

   * **Quando l’ambito di un progetto cambia**: per informazioni su cosa costituisce una modifica dell’ambito di un progetto, consulta [Ricalcolare i timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In questo caso, [!DNL Workfront] ricalcola la timeline per tutti i progetti con Tipo di aggiornamento [!UICONTROL Automatico e in caso di modifica] o [!UICONTROL Solo su modifica].
Per informazioni sui tipi di aggiornamento dei progetti, consulta [Panoramica del tipo di aggiornamento del progetto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Fai clic su **[!UICONTROL Salva]**.

   La timeline di tutti i progetti nel sistema viene ricalcolata automaticamente in base al Tipo di aggiornamento di ciascun progetto.

## Ricalcolare le timeline per l’intero [!DNL Workfront] istanza

È possibile eseguire [!UICONTROL Ricalcola sequenza temporale] diagnostica per ricalcolare manualmente tutte le timeline nel [!DNL Workfront] di rete. Questo consente a tutti i project manager di visualizzare immediatamente l&#39;influenza di modifiche esterne sia nelle date pianificate che in quelle previste. Per ulteriori informazioni, consulta [Utilizzare la diagnostica per attivare i processi automatizzati](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).

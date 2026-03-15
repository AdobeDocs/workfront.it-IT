---
product-area: agile-and-teams
navigation-topic: burndown
title: Usa una pianificazione alternativa per i grafici a discesa
description: Le pianificazioni definite in [!DNL Adobe Workfront] influiscono sul grafico di masterizzazione escludendo i giorni di riposo (fine settimana e festivi) dal masterizzazione.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 18%

---

# Utilizzare una pianificazione del team alternativa per i grafici lavoro

Le pianificazioni definite in [!DNL Adobe Workfront] influiscono sul grafico di masterizzazione escludendo i giorni di riposo (fine settimana e festivi) dal masterizzazione.

Per impostazione predefinita, il grafico a dispersione utilizza la pianificazione predefinita. Oltre alla pianificazione predefinita, i team Agile possono scegliere di utilizzare anche una pianificazione alternativa per includere giorni non lavorativi specifici del team. Questa pianificazione alternativa viene quindi riflessa nel grafico a discesa di qualsiasi iterazione assegnata al team. La pianificazione alternativa ha effetto solo sul grafico di masterizzazione. Per ulteriori informazioni sulla pianificazione predefinita e su come l&#39;amministratore di [!DNL Workfront] può creare una pianificazione specifica per il team, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Il grafico di masterizzazione non prende in considerazione i giorni parziali. Ad esempio, se il team lavora 4 ore ogni venerdì, viene rappresentato come un giorno intero nel grafico di masterizzazione.

Per ulteriori informazioni sull&#39;utilizzo del grafico di masterizzazione, vedere [Panoramica del grafico di masterizzazione Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p> </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizzare una pianificazione del team alternativa per i grafici lavoro

1. Assicurati che l&#39;amministratore [!DNL Workfront] abbia già creato la pianificazione alternativa, come descritto in [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team Agile che desideri gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella sezione **[!UICONTROL Agile]**, nell&#39;area **[!UICONTROL Pianificazione]**, selezionare la nuova pianificazione dal menu a discesa.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

---
product-area: agile-and-teams
navigation-topic: burndown
title: Usa una pianificazione alternativa del team per i grafici Burndown
description: Le pianificazioni definite in [!DNL Adobe Workfront] influiscono sul grafico burndown escludendo i giorni liberi (fine settimana e festivi) dal burndown.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 16%

---

# Utilizzare una pianificazione del team alternativa per i grafici lavoro

Le pianificazioni definite in [!DNL Adobe Workfront] influiscono sul grafico burndown escludendo i giorni liberi (fine settimana e festivi) dal burndown.

Per impostazione predefinita, il grafico a dispersione utilizza la pianificazione predefinita. Oltre alla pianificazione predefinita, i team Agile possono scegliere di utilizzare anche una pianificazione alternativa per incorporare giorni non lavorativi specifici del team. Questa pianificazione alternativa viene quindi riportata nel grafico a discesa di qualsiasi iterazione assegnata al team. La pianificazione alternativa influisce solo sul grafico a dispersione. Per ulteriori informazioni sulla pianificazione predefinita e su come l&#39;amministratore [!DNL Workfront] può creare una pianificazione specifica per il team, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Il grafico burndown non prende in considerazione i giorni parziali. Ad esempio, se il tuo team lavora 4 ore al venerdì, viene rappresentato come un giorno intero nel grafico a dispersione.

Per ulteriori informazioni sull&#39;utilizzo del grafico a dispersione, vedere [Panoramica del grafico a dispersione Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizzare una pianificazione del team alternativa per i grafici lavoro

1. Verificare che l&#39;amministratore [!DNL Workfront] abbia già creato la pianificazione alternativa, come descritto in [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team Agile da gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

1. Nella sezione **[!UICONTROL Agile]**, nell&#39;area **[!UICONTROL Pianificazione]**, selezionare la nuova pianificazione dal menu a discesa.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

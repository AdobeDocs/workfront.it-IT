---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usa bandiere sulle storie sulla bacheca Kanban
description: Sulla [!DNL Kanban] bacheca, i flag forniscono un'indicazione visiva di quando una storia è pronta per passare al successivo stato. Questo consente ai team Kanban di utilizzare un approccio "pull" anziché un approccio "push" quando si spostano le storie tra stati diversi.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Usa bandiere sulle storie [!UICONTROL Kanban] bacheca

Sulla [!DNL Kanban] bacheca, i flag forniscono un&#39;indicazione visiva di quando una storia è pronta per passare al successivo stato. Ciò consente [!UICONTROL Kanban] i team devono utilizzare un approccio &quot;pull&quot; anziché &quot;push&quot; quando si spostano le storie tra stati diversi.

**Esempio:** Prendi in considerazione l’esempio seguente di un team che utilizza un approccio &quot;pull&quot;: Olivia, la graphic designer del team, termina il suo lavoro e poi imposta il flag di storia come &quot;[!UICONTROL Pronto per il pull].&quot; Questo flag fornisce un&#39;indicazione visiva a Tony, il copywriter del team, che la storia è pronta per il suo passaggio al prossimo stato. Tony quindi sposta la storia allo stato successivo quando è pronto per iniziare a lavorarci.

Quando utilizzi i flag sulle storie, tieni presente quanto segue:

* I flag non sono uno stato, ma piuttosto un’indicazione visiva che la storia è pronta per essere spostata nello stato successivo da un altro membro del team.
* I flag non vengono visualizzati su nessuna delle schede del brano che si trovano in [!UICONTROL Backlog] o nella colonna [!UICONTROL Completa] o in una colonna in cui lo stato della colonna è uguale a [!UICONTROL Completa]).

   Per ulteriori informazioni sugli stati della storia, consulta [Usa bandiere sulle storie sulla bacheca Kanban](#updating-the-status-of-stories-and-subtasks)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Usa bandiere sulle storie [!UICONTROL Kanban] bacheca

Per cambiare una bandiera su una storia:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo [!UICONTROL Kanban] dal menu a discesa o cerca un team nella barra di ricerca.

1. Vai a [!UICONTROL Kanban] bordo in cui si desidera cambiare una bandiera su una storia.
1. Espandi il riquadro della storia per visualizzare la bandiera.\
   Il flag è impostato su **[!UICONTROL On Track]** per ogni storia per impostazione predefinita.\
   ![Scheda Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Fai clic sul flag corrente, quindi seleziona una delle seguenti opzioni di flag:

   * **[!UICONTROL On Track]:** La storia si trova nello stato appropriato e non è necessario intervenire in questo momento.\

      Questo è il flag predefinito per ogni storia sulla bacheca Kanban.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Bloccato]:** Impossibile passare allo stato successivo. Quando questo flag è impostato su un brano, il brano non viene conteggiato verso il limite WIP. (Per ulteriori informazioni sui limiti WIP, vedere l&#39;articolo [Configurare Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_bloccato.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Pronto per il pull]:** Il brano è pronto per essere spostato allo stato successivo da un altro membro del team.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)

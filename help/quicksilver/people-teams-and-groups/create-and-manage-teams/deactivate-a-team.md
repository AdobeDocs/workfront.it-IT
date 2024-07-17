---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Disattivare un team
description: Puoi disattivare i team che non utilizzi più conservando i dati storici associati. Gli amministratori di Adobe Workfront possono riattivare un team in qualsiasi momento dall’area Team di Configurazione.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Disattivare un team

Puoi disattivare i team che non utilizzi più conservando i dati storici associati. Gli amministratori di [!DNL Adobe Workfront] possono riattivare un team in qualsiasi momento dall&#39;area Team in Configurazione. Se si disattiva un team, il team non verrà più visualizzato nelle seguenti aree:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campi typeahead nei moduli personalizzati</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Finestra di dialogo Condivisione per gli oggetti</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu a discesa di selezione principale nell'area [!UICONTROL Teams]</p> </li> 
     <li> <p>[Assegnazioni UICONTROL] completamento automatico</p> </li> 
     <li> <p>Finestra di dialogo [!UICONTROL Aggiungi a Kanban] in un progetto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

I team disattivati non vengono visualizzati durante la ricerca di un team, ma verranno comunque visualizzati nel [!UICONTROL Team predefinito] e in Altri team se l&#39;utente è stato assegnato al team prima della disattivazione.

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
   <td> <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore [!DNL Workfront].

## Disattivare un team

Eventuale lavoro assegnato al team prima della disattivazione rimane assegnato. È consigliabile riassegnare il lavoro prima di disattivare il team.

>[!TIP]
>
>Puoi creare un rapporto per filtrare le attività o i problemi per i quali il team disattivato è ancora assegnato.

Quando si utilizzano le code di richieste, se si disattiva un team assegnato come team predefinito in una regola di routing, il team rimane e le richieste vengono ancora instradate al team disattivato. Prima di disattivare il team, è consigliabile aggiornare le regole di instradamento con i team attivi.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sull&#39;icona **[!DNL Switch team]**, quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   ![](assets/edit-team-settings-350x205.png)

1. Deselezionare la casella di controllo **[!UICONTROL È attivo]**.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Limitazioni note

I team disattivati vengono visualizzati nelle seguenti aree:

* Il campo Proprietario in [!DNL Workfront Goals]. È necessaria una licenza aggiuntiva per [!DNL Adobe Workfront Goals]. Per ulteriori informazioni, vedere [Introduzione a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

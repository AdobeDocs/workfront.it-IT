---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Disattivare o eliminare un team
description: Puoi disattivare i team che non utilizzi più conservando i dati storici associati. Gli amministratori di Adobe Workfront possono riattivare un team in qualsiasi momento dall’area Team di Configurazione.
author: Courtney
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 10%

---

# Disattivare o eliminare un team

Puoi disattivare i team che non utilizzi più conservando i dati storici associati. Gli amministratori di [!DNL Adobe Workfront] possono riattivare un team in qualsiasi momento dall&#39;area Team in Configurazione. Se disattivi un team, questo non verrà più visualizzato nelle seguenti aree:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campi Typeahead nei moduli personalizzati</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Finestra di dialogo per la condivisione degli oggetti</p> </li> 
     <li> <p>[!UICONTROL Profilo Utente]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu a discesa di selezione principale nell'area [!UICONTROL Teams]</p> </li> 
     <li> <p>Typeahead [!UICONTROL Assignments]</p> </li> 
     <li> <p>Finestra di dialogo della bacheca [!UICONTROL Add to Kanban] in un progetto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

I team disattivati non vengono visualizzati durante la ricerca di un team, ma verranno comunque visualizzati nel [!UICONTROL team principale] e in altri team se l&#39;utente è stato assegnato al team prima della disattivazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Pacchetto Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr>
   <td>Configurazioni del livello di accesso</td>
   <td><p>Per disattivare un team, non è necessaria alcuna configurazione.</p>
   <p>Per eliminare un team, è necessario essere un amministratore di sistema.</p></td>
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Disattivare un team

Eventuale lavoro assegnato al team prima della disattivazione rimane assegnato. È consigliabile riassegnare il lavoro prima di disattivare il team.

>[!TIP]
>
>Puoi creare un rapporto per filtrare le attività o i problemi per i quali il team disattivato è ancora assegnato.

Quando si utilizzano le code di richiesta, se si disattiva un team assegnato come team predefinito in una regola di routing, il team rimane e le richieste vengono ancora instradate al team disattivato. Si consiglia di aggiornare le regole di routing con i team attivi prima di disattivare il team.

{{step1-to-team}}

1. Fai clic sull’icona **[!DNL Switch team]**, quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   ![](assets/edit-team-settings.png)

1. Deselezionare la casella di controllo **[!UICONTROL Attivo]** nelle impostazioni del team.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Limitazioni note della disattivazione di un team

I team disattivati vengono visualizzati nelle seguenti aree:

* Il campo Proprietario in [!DNL Workfront Goals]. È necessaria una licenza aggiuntiva per [!DNL Adobe Workfront Goals]. Per ulteriori informazioni, vedere [Introduzione a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Eliminare un team

Solo un amministratore di sistema può eliminare un team. Se sei il proprietario di un team (ma non un amministratore) e provi a eliminare un team, visualizzerai un messaggio di errore.

Per eliminare un team:

{{step1-to-team}}

1. Fai clic sull’icona **[!DNL Switch team]**, quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Elimina]**.

   ![](assets/edit-team-settings.png)

1. Fai clic su [!UICONTROL **Conferma**] nel messaggio di conferma per eliminare definitivamente il team. I team eliminati non possono essere recuperati.

---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Disattivare un team
description: È possibile disattivare i team non più utilizzati mantenendo i dati storici associati. Gli amministratori di Adobe Workfront possono riattivare un team in qualsiasi momento dall’area Team in Configurazione.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Disattivare un team

È possibile disattivare i team non più utilizzati mantenendo i dati storici associati. [!DNL Adobe Workfront] Gli amministratori possono riattivare un team in qualsiasi momento dall&#39;area Team in Configurazione. Se disattivi un team, il team non viene più visualizzato nelle seguenti aree:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campi di tipo anticipo nei moduli personalizzati</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Finestra di dialogo di condivisione per gli oggetti</p> </li> 
     <li> <p>[!UICONTROL Profilo utente]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu a discesa della selezione principale nell’area [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Assegnazioni] tipo di anticipo</p> </li> 
     <li> <p>Finestra di dialogo Aggiungi a bacheca Kanban in un progetto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

I team disattivati non vengono visualizzati quando si cerca un team, ma vengono comunque visualizzati in [!UICONTROL Team principale] e altri team se l’utente è stato assegnato al team prima della disattivazione.

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

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Disattivare un team

Qualsiasi lavoro assegnato al team prima della disattivazione rimane assegnato. È consigliabile riassegnare il lavoro prima di disattivare il team.

>[!TIP]
>
>È possibile creare un rapporto per filtrare le attività o i problemi a cui il team disattivato è ancora assegnato.

Quando si utilizzano le code di richiesta, se si disattiva un team assegnato come team predefinito in una regola di routing, il team rimane e le richieste vengono comunque indirizzate al team disattivato. È consigliabile aggiornare le regole di routing con i team attivi prima di disattivare il team.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sul pulsante **[!DNL Switch team]** , quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.

   ![](assets/edit-team-settings-350x205.png)

1. Elimina **[!UICONTROL È attivo]** casella di controllo.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Limitazioni note

I team disattivati vengono visualizzati nelle seguenti aree:

* Il campo Proprietario in [!DNL Workfront Goals]. È necessaria una licenza aggiuntiva per [!DNL Adobe Workfront Goals]. Per ulteriori informazioni, consulta [Introduzione a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

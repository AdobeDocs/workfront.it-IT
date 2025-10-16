---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare le preferenze per gli aggiornamenti utente
description: Puoi configurare le preferenze che accedono a determinate funzioni quando gli utenti aggiungono commenti nell'area [!UICONTROL Aggiornamenti] di un oggetto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Configurare le preferenze per gli aggiornamenti utente

<!--Audited: 08/2025-->

Puoi configurare le preferenze che consentono agli utenti di accedere a determinate funzioni quando aggiungono commenti nell&#39;area [!UICONTROL Aggiornamenti] di un oggetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>dall'amministratore di sistema, per eseguire questi passaggi a livello di sistema. </p>
   <p>Planner, per eseguire questi passaggi per un gruppo, oltre a essere il manager di quel gruppo.</p></td>
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## Consenti agli utenti di aggiungere immagini negli aggiornamenti

Per impostazione predefinita, gli utenti non possono aggiungere immagini negli aggiornamenti. Se si attiva questa preferenza, gli utenti potranno allegare immagini negli aggiornamenti. La preferenza si applica a tutti gli aggiornamenti in tutte le aree dell&#39;istanza [!DNL Workfront].

>[!NOTE]
>
>* Le immagini salvate negli aggiornamenti vengono conteggiate in base al limite di archiviazione dei documenti. Per informazioni, vedere [Controllare i limiti di archiviazione dei documenti](../../../documents/managing-documents/check-document-storage.md).
>* Le immagini sono accessibili tramite la scheda [!UICONTROL Aggiornamenti] su un oggetto e sono disponibili anche nell&#39;area [!UICONTROL Documenti] del [!UICONTROL Menu principale].
>

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, seleziona **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.
1. Selezionare la scheda **[!UICONTROL Preferenze]**.

   ![Preferenze utente per feed di aggiornamento](assets/updatefeeds-preferences-350x137.png)

1. Selezionare la casella di controllo **[!UICONTROL Consenti agli utenti di aggiungere immagini negli aggiornamenti]**.
1. Seleziona **[!UICONTROL Salva]**.

   Se questa preferenza è attivata, è possibile disattivarla in qualsiasi momento. Tutte le immagini già pubblicate negli aggiornamenti rimarranno nell&#39;area [!UICONTROL Aggiornamenti] dell&#39;oggetto.

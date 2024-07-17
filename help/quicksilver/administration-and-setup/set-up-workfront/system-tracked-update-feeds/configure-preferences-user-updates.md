---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare le preferenze per gli aggiornamenti utente
description: Puoi configurare le preferenze che accedono a determinate funzioni quando gli utenti aggiungono commenti nell'area [!UICONTROL Aggiornamenti] di un oggetto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---

# Configurare le preferenze per gli aggiornamenti utente

Puoi configurare le preferenze che consentono agli utenti di accedere a determinate funzioni quando aggiungono commenti nell&#39;area [!UICONTROL Aggiornamenti] di un oggetto.

## Requisiti di accesso

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario il livello di accesso [!UICONTROL System Administrator].</p><p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Consenti agli utenti di aggiungere immagini negli aggiornamenti

Per impostazione predefinita, gli utenti non possono aggiungere immagini negli aggiornamenti. Se si attiva questa preferenza, gli utenti potranno allegare immagini negli aggiornamenti. La preferenza si applica a tutti gli aggiornamenti in tutte le aree dell&#39;istanza [!DNL Workfront].

>[!NOTE]
>
>* Le immagini salvate negli aggiornamenti vengono conteggiate in base al limite di archiviazione dei documenti. Per informazioni, vedere [Controllare i limiti di archiviazione dei documenti](../../../documents/managing-documents/check-document-storage.md).
>* Le immagini sono accessibili tramite la scheda [!UICONTROL Aggiornamenti] su un oggetto e sono disponibili anche nell&#39;area [!UICONTROL Documenti] del [!UICONTROL Menu principale].
>

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, seleziona **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.
1. Selezionare la scheda **[!UICONTROL Preferenze]**.

   ![Preferenze utente per feed di aggiornamento](assets/updatefeeds-preferences-350x137.png)

1. Selezionare la casella di controllo **[!UICONTROL Consenti agli utenti di aggiungere immagini negli aggiornamenti]**.
1. Seleziona **[!UICONTROL Salva]**.

   Se questa preferenza è attivata, è possibile disattivarla in qualsiasi momento. Tutte le immagini già pubblicate negli aggiornamenti rimarranno nell&#39;area [!UICONTROL Aggiornamenti] dell&#39;oggetto.

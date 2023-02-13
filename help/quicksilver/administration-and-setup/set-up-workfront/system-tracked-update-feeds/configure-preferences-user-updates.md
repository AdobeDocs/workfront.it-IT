---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare le preferenze per gli aggiornamenti utente
description: È possibile configurare preferenze che consentono l'accesso a determinate funzioni quando gli utenti aggiungono commenti in un oggetto [!UICONTROL Aggiornamenti] area.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Configurare le preferenze per gli aggiornamenti utente

È possibile configurare le preferenze che consentono agli utenti di accedere a determinate funzioni quando aggiungono commenti in un oggetto [!UICONTROL Aggiornamenti] area.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso [!UICONTROL System Administrator].</p><p>Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Consenti agli utenti di aggiungere immagini negli aggiornamenti

Per impostazione predefinita, gli utenti non possono aggiungere immagini negli aggiornamenti. Quando abiliti questa preferenza, gli utenti potranno allegare le immagini negli aggiornamenti. La preferenza si applica a tutti gli aggiornamenti in tutte le aree del [!DNL Workfront] istanza.

>[!NOTE]
>
>* Le immagini salvate negli aggiornamenti vengono conteggiate fino al limite di archiviazione del documento. Per informazioni, consulta [Controlla i limiti di archiviazione dei documenti](../../../documents/managing-documents/check-document-storage.md).
>* Le immagini sono accessibili solo tramite [!UICONTROL Aggiornamenti] su un oggetto e non sono disponibili nella scheda [!UICONTROL Documenti] scheda .
>




1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, seleziona **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.
1. Seleziona la **[!UICONTROL Preferenze]** scheda .

   ![Preferenze utente per l’aggiornamento dei feed](assets/updatefeeds-preferences-350x137.png)

1. Seleziona la **[!UICONTROL Consenti agli utenti di aggiungere immagini negli aggiornamenti]** casella di controllo.
1. Seleziona **[!UICONTROL Salva]**.

   Quando questa preferenza è attivata, puoi disattivarla in qualsiasi momento. Tutte le immagini già pubblicate negli aggiornamenti rimarranno nel [!UICONTROL Aggiornamenti] area dell&#39;oggetto.

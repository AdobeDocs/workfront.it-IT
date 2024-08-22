---
title: Configura l'integrazione  [!DNL Workfront] e [!DNL Frame.io]
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: In qualità di  [!DNL Adobe Workfront] amministratore, puoi integrare [!DNL Workfront] con [!DNL Frame.io] e fornire alla tua organizzazione un modo semplice per rivedere e approvare le risorse.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Configurare l&#39;integrazione di [!DNL Workfront] e [!DNL Frame.io]

L&#39;amministratore di Workfront abilita l&#39;integrazione tra Workfront e Frame.io configurando l&#39;account predefinito Frame.io nell&#39;area Setup e quindi designando gli utenti Frame.io in Workfront. Questo consente al coordinatore del progetto di pianificare e avviare il lavoro utilizzando i progetti Workfront e i flussi di lavoro di revisione e approvazione.


## Requisiti di accesso

>[!IMPORTANT]
>
>Questa funzionalità è disponibile solo per le organizzazioni che sono state caricate in [!DNL Adobe Admin Console].

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] piano</td>
   <td>Qualsiasi</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenze
   </td>
   <td><p>Corrente: [!UICONTROL Plan]</p>
   <p>Nuovo: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>

</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura un account [!DNL Frame.io] predefinito [!BADGE Disponibile a breve]{type=Informative}

Una volta configurato l&#39;account predefinito [!DNL Frame.io], tutti i progetti creati in [!DNL Workfront] avranno un progetto mirror creato in Frame.io.

>[!IMPORTANT]
>
>Questa funzione sarà presto disponibile. Per il momento, gli account Frame.io vengono aggiunti manualmente dal team Workfront. Contatta il rappresentante del tuo account di Adobe per assistenza.

## Configurare un singolo account Frame.io con un gruppo Workfront

È possibile collegare un singolo gruppo Workfront con un singolo account Frame.io diverso dall&#39;account predefinito.

Per configurare un singolo account Frame.io con un gruppo Workfront:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Scegli un gruppo esistente o fai clic su **Crea gruppo**.
1. Nel pannello a sinistra, fai clic su **Connetti a Frame.io**.
1. Immetti il token di sviluppo API.
1. Fare clic su **Avvia connessione**.
1. (Condizionale) Se siete l&#39;amministratore di più account Frame.io, selezionate l&#39;account che desiderate utilizzare.

## Abilita utenti Frame.io

Gli utenti Workfront che utilizzano regolarmente Frame.io devono essere contrassegnati come utenti Frame.io. Gli amministratori di Workfront possono designare gli utenti Frame.io nel profilo utente di Workfront.

>[!TIP]
>
>Consigliamo di abilitare gli utenti che lavorano regolarmente in strumenti creativi e caricano risorse da rivedere e approvare come utenti Frame.io.

Quando un utente viene contrassegnato come utente Frame.io in Workfront e viene aggiunto a un progetto:

* Vengono aggiunti come collaboratori in Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Possono inviare le risorse da Frame.io a Workfront per la revisione e l’approvazione formali.
* Possono visualizzare informazioni nella cartella di sincronizzazione unidirezionale da Workfront. [!BADGE In arrivo]{type=Informative}

Per abilitare gli utenti Frame.io:

{{step-1-to-users}}

1. Seleziona uno o più utenti, quindi fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).
1. Nella sezione Accesso, abilita la casella di controllo Aggiungi a progetti in Frame.io, quindi seleziona **Sì** nel menu a discesa.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Se questa casella non è selezionata, l&#39;utente mantiene l&#39;accesso alle assegnazioni passate e viene aggiunto ai progetti Frame.io a partire dal.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

---
title: Configurare [!DNL Workfront] e [!DNL Frame.io] integrazione
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Come un [!DNL Adobe Workfront] amministratore, puoi integrare [!DNL Workfront] con [!DNL Frame.io] e fornire all’organizzazione un modo semplice per rivedere e approvare le risorse.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Configurare [!DNL Workfront] e [!DNL Frame.io] integrazione

L&#39;amministratore di Workfront abilita l&#39;integrazione tra Workfront e Frame.io configurando l&#39;account predefinito Frame.io nell&#39;area Setup e quindi designando gli utenti Frame.io in Workfront. Questo consente al coordinatore del progetto di pianificare e avviare il lavoro utilizzando i progetti Workfront e i flussi di lavoro di revisione e approvazione.


## Requisiti di accesso

>[!IMPORTANT]
>
>Questa funzionalità è disponibile solo per le organizzazioni che sono state caricate in [!DNL Adobe Admin Console].

Devi avere i seguenti:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] piano</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenze</strong>
   </td>
   <td>Corrente: [!UICONTROL Plan] <br>
   Nuovo: [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>Configurazioni del livello di accesso</strong>
   </td>
   <td>Devi essere un [!DNL Workfront] amministratore.
   </td>
  </tr>

</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Configurare un valore predefinito [!DNL Frame.io] account [!BADGE Disponibile a breve]{type=Informative}

Una volta impostato il valore predefinito [!DNL Frame.io] è configurato, tutti i progetti creati in [!DNL Workfront] dispongono di un progetto mirror creato in Frame.io.

>[!IMPORTANT]
>
>Questa funzione sarà presto disponibile. Per il momento, gli account Frame.io vengono aggiunti manualmente dal team Workfront. Contatta il rappresentante del tuo account di Adobe per assistenza.

## Configurare un singolo account Frame.io con un gruppo Workfront

È possibile collegare un singolo gruppo Workfront con un singolo account Frame.io diverso dall&#39;account predefinito.

Per configurare un singolo account Frame.io con un gruppo Workfront:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Scegliete un gruppo esistente o fate clic su **Crea gruppo**.
1. Nel pannello a sinistra, fai clic su **Connetti a Frame.io**.
1. Immetti il token di sviluppo API.
1. Clic **Avvia connessione**.
1. (Condizionale) Se siete l&#39;amministratore di più account Frame.io, selezionate l&#39;account che desiderate utilizzare.

## Abilita utenti Frame.io

Gli utenti Workfront che utilizzano regolarmente Frame.io devono essere contrassegnati come utenti Frame.io. Gli amministratori di Workfront possono designare gli utenti Frame.io nel profilo utente di Workfront.

>[!TIP]
>
>Consigliamo di abilitare gli utenti che lavorano regolarmente in strumenti creativi e caricano risorse da rivedere e approvare come utenti Frame.io.

Quando un utente viene contrassegnato come utente Frame.io in Workfront e viene aggiunto a un progetto:

* Vengono aggiunti come collaboratori in Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Possono inviare le risorse da Frame.io a Workfront per la revisione e l’approvazione formali.
* Possono visualizzare informazioni nella cartella di sincronizzazione unidirezionale da Workfront. [!BADGE Disponibile a breve]{type=Informative}

Per abilitare gli utenti Frame.io:

{{step-1-to-users}}

1. Seleziona uno o più utenti, quindi fai clic su **Modifica** icona ![](assets/edit-icon.png).
1. Nella sezione Accesso, abilita la casella di controllo Aggiungi a progetti in Frame.io, quindi seleziona **Sì** nel menu a discesa.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Se questa casella non è selezionata, l&#39;utente mantiene l&#39;accesso alle assegnazioni passate e viene aggiunto ai progetti Frame.io in futuro.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->


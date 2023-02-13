---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integrazioni di Adobe Experience Manager Assets
description: Puoi collegare il tuo lavoro con le seguenti integrazioni di Adobe Experience Manager Assets.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# Configura le [!UICONTROL Experience Manager Assets as a Cloud Service] integrazione

Puoi collegare il tuo lavoro con il tuo contenuto in [!DNL Experience Manager Assets]&#x200B;:

* Push di risorse e metadati da [!DNL Adobe Workfront] a [!DNL Experience Manager Assets]&#x200B;
* Collegare le risorse da [!DNL Experience Manager Assets] a progetti e attività in [!DNL Workfront&#x200B;]
* Facilitare i casi di utilizzo del controllo delle versioni
* Crea cartelle collegate a [!DNL Experience Manager Assets]
* Tracciamento metadati per risorse e cartelle
* Sincronizza i metadati del progetto tra [!DNL Workfront] e [!DNL Experience Manager Assets]


## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] piano*</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenze*</strong>
   </td>
   <td>[!UICONTROL Plan]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] licenza</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td>Devi avere [!DNL Experience Manager Assets as a Cloud Service]e devi essere aggiunto al prodotto come utente.
   </td>
  </tr>
  <tr>
   <td>Configurazioni a livello di accesso*
   </td>
   <td>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <strong>Concedere a un utente pieno accesso amministrativo</strong>.
   </td>
  </tr>
</table>


*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.


## Prerequisiti

Prima di iniziare,

* Devi avere [!DNL Workfront] e [!DNL Adobe Experience Manager Assets] associato a un ID organizzazione in [!DNL Adobe Admin Consol]e. Per ulteriori informazioni, consulta [Differenze di amministrazione basate su piattaforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configurare le informazioni sull’integrazione

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** .
1. Seleziona **[!UICONTROL Documenti]** nel pannello a sinistra, seleziona **[!UICONTROL [!DNL Experience Manager]Integrazione]**.
   >[!NOTE]
   >
   >Questa area di configurazione viene visualizzata solo se [!DNL Workfront] l&#39;ambiente è incluso in un [!DNL Adobe Admin Console].

1. Seleziona **[!UICONTROL Aggiungi [!DNL Experience Manager] Integrazione]**.
1. In **[!UICONTROL Nome]** immetti il nome che gli utenti dovranno visualizzare quando interagiscono con questa integrazione in Workfront e Experience Manager Assets.
1. In **[!UICONTROL URL di navigazione]** Il sistema popola automaticamente l&#39;URL di navigazione. Questo URL di sola lettura viene utilizzato per effettuare un collegamento a [!DNL Experience Manager] istanza dal [!UICONTROL Menu principale] per un accesso rapido.
1. Scegli un archivio dal **[!UICONTROL [!DNL Experience Manager]Archivio risorse]** menu a discesa. Il sistema popola automaticamente qualsiasi [!DNL Experience Manager] archivi associati all&#39;ID organizzazione a cui è assegnato il profilo utente.
   ![scegli archivio experience manager](assets/setup-information.png)

1. Fai clic su **[!UICONTROL Salva]** o passare alla [Impostare i metadati (facoltativo)](#set-up-metadata-optional) in questo articolo.

   >[!NOTE]
   >
   >A causa della complessità dell’integrazione, non puoi modificare l’archivio dopo aver salvato la configurazione iniziale.

## Impostare i metadati (facoltativo)

Puoi mapparlo [!DNL Workfront] dati oggetto ai campi del supporto risorse in [!DNL Experience Manager] Risorse.

>[!IMPORTANT]
>
>Puoi mappare i metadati in una sola direzione: da [!DNL Workfront] a [!DNL Experience Manager]. Metadati dei documenti collegati a [!DNL Workfront] da [!DNL Experience Manager] non può essere trasferito in [!DNL Workfront].



### Configurare i campi di metadati

1. Configurare uno schema di metadati in [!DNL Experience Manager Assets] come spiegato in [Configurare la mappatura dei metadati delle risorse tra Adobi [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Configura campi modulo personalizzati in Workfront. [!DNL Workfront] dispone di molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, puoi anche creare campi personalizzati come descritto in [Creare o modificare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Risorse

I metadati vengono mappati quando una risorsa viene inviata da [!DNL Workfront] per la prima volta. I documenti con campi incorporati o personalizzati vengono mappati automaticamente ai campi specificati al primo invio di una risorsa [!DNL Experience Manager Assets].

>[!NOTE]
>
>Questa integrazione non supporta metadati personalizzati da [!DNL Adobe Experience Manager].

Per mappare i metadati per le risorse:

1. Seleziona **[!UICONTROL Risorse]** sopra la tabella metadati.
1. In **[!UICONTROL [!DNL Workfront]field]** scegliere un campo Workfront integrato o personalizzato.

   >[!NOTE]
   >
   >Puoi mappare una singola [!DNL Workfront] campo a più [!UICONTROL Experience Manager Assets] campi. Non è possibile mappare più [!DNL Workfront] campi in un singolo [!DNL Experience Manager Assets] campo .

1. In [!DNL Experience Manager Assets] , cerca tra le categorie prepopolate o inserisci almeno due lettere nel campo di ricerca per accedere alle categorie aggiuntive.
1. Ripetere i passaggi 2 e 3 come necessario.
   ![campi metadati](assets/asset-metadata.png)
1. Fai clic su [!UICONTROL Salva] o passare alla [Cartelle](#folders) in questo articolo.

### Cartelle

Quando gli utenti creano una cartella collegata su un progetto, i dati del progetto, del portfolio e del programma associati vengono mappati sui campi dei metadati della cartella in [!DNL Experience Manager Assets].

>[!NOTE]
>
>Questa integrazione non supporta metadati personalizzati da [!DNL Adobe Experience Manager].

Per mappare i metadati per le cartelle:

1. Seleziona **[!UICONTROL Cartelle]** sopra la tabella metadati.
1. In **[!UICONTROL [!DNL Workfront]field]** scegliere un campo Workfront integrato o personalizzato.

   >[!NOTE]
   >
   >È possibile mappare un singolo campo Workfront su più campi Experience Manager Assets. Non è possibile mappare più [!DNL Workfront] campi in un singolo [!DNL Experience Manager Assets] campo .

1. In **[!DNL Experience Manager Assets]** , cerca tra le categorie prepopolate o inserisci almeno due lettere nel campo di ricerca per accedere alle categorie aggiuntive.
1. Ripetere i passaggi 2 e 3 come necessario.
   ![metadati della cartella](assets/folder-metadata.png)
1. Fai clic su **[!UICONTROL Salva]** o passare alla [Sincronizzazione dei metadati del progetto](#project-metadata-sync) in questo articolo.


### Sincronizzazione dei metadati degli oggetti

Un [!DNL Experience Manager] campi mappati su [!DNL Workfront] i campi portfolio, programma, progetto, task, problema e documento vengono aggiornati automaticamente quando il campo viene modificato in [!DNL Workfront].

>[!IMPORTANT]
>
>Gli utenti devono avere accesso in scrittura in [!DNL Experience Manager] per le risorse che vivono nell’oggetto per consentire la sincronizzazione dei metadati al momento dell’aggiornamento.

1. Abilita la **[!UICONTROL Sincronizzazione dei metadati degli oggetti]** campo .
1. Fai clic su Salva o passa a [Configurare cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.

## Configurare cartelle collegate (facoltativo)

Puoi consentire agli utenti di creare cartelle collegate a [!DNL Experience Manager] mentre in un [!DNL Workfront] progetto. Quando una cartella è collegata, tutte le risorse aggiunte alla cartella vengono automaticamente visualizzate in entrambi [!DNL Workfront] e [!DNL Experience Manager]. Quando una risorsa viene aggiunta alla cartella collegata in [!DNL Workfront] per la prima volta, i metadati della risorsa vengono inviati a [!DNL Experience Manager Assets].

Nei passaggi seguenti, si indica dove si desidera creare le cartelle collegate. Ciascuna integrazione può avere una sola posizione per tutte le cartelle collegate.

Per impostare le cartelle collegate:

1. Attiva/disattiva la **[!UICONTROL Abilita cartella collegata]** su.
1. Scegli un percorso di cartella per indicare la posizione in cui dovranno essere associate tutte le cartelle collegate a questa integrazione.

   >[!NOTE]
   >
   >Gli utenti devono accedere in scrittura a [!DNL Adobe Experience Manager Assets] alla cartella specificata per creare una cartella collegata.

1. Fai clic su **[!UICONTROL Salva]**.

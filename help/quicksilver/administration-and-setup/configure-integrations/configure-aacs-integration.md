---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integrazioni di Adobe Experience Manager Assets
description: Puoi collegare il tuo lavoro con le seguenti integrazioni di Adobe Experience Manager Assets.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 337aead90dba40a3c9104fb0183897c17f2cd66d
workflow-type: tm+mt
source-wordcount: '1504'
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

Puoi anche collegare più archivi Experience Manager Assets a un ambiente Workfront o a più ambienti Workfront a un archivio Experience Manager Assets in tutti gli ID organizzazione. Segui le istruzioni di configurazione riportate in questo articolo per ogni integrazione che desideri configurare.

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

Prima di iniziare la mappatura dei campi di metadati, è necessario configurare i campi di metadati sia in Workfront che in Experience Manager Assets.

Per configurare i campi metadati:

1. Configurare uno schema di metadati in [!DNL Experience Manager Assets] come spiegato in [Configurare la mappatura dei metadati delle risorse tra Adobi [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configura campi modulo personalizzati in Workfront. [!DNL Workfront] dispone di molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, puoi anche creare campi personalizzati come descritto in [Creare o modificare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Espandi per visualizzare ulteriori informazioni sui campi Workfront e Experience Manager Assets supportati**

**Tag Experience Manager Assets**

Puoi mappare qualsiasi campo supportato da Workfront a un tag in Experience Manager Assets. A questo scopo, è necessario assicurarsi che i valori dei tag in Experience Manager Assets corrispondano a Workfront.

* I tag e i valori dei campi Workfront devono corrispondere esattamente in ortografia e formato.
* I valori dei campi di Workfront mappati ai tag delle risorse di experience Manager devono essere tutti minuscoli, anche se il tag in Experience Manager Assets sembra avere lettere maiuscole.
* I valori dei campi Workfront non devono includere spazi.
* Il valore del campo in Workfront deve includere anche la struttura di cartelle del tag Experience Manager Assets.
* Per mappare più campi di testo a riga singola ai tag, immetti un elenco separato da virgole dei valori dei tag nel lato Workfront della mappatura dei metadati e `xcm:keywords` sul lato Experience Manager Assets. Ogni valore di campo è associato a un tag separato. È possibile utilizzare un campo calcolato per combinare più campi Workfront in un singolo campo di testo separato da virgole.
* È possibile mappare i valori dai campi a discesa, pulsante di scelta o casella di controllo immettendo un elenco separato da virgole dei valori disponibili in quel campo.


>[!INFO]
>
>**Esempio**: Per far corrispondere qui il tag presente nella struttura delle cartelle, il valore del campo in Workfront è `landscapes:trees/spruce`. Nel valore del campo Workfront sono riportate le lettere minuscole.
>
>Se desideri che il tag sia l’elemento più a sinistra nella struttura dei tag, deve essere seguito da due punti. In questo esempio, per eseguire la mappatura sul tag relativo ai paesaggi, il valore del campo in Workfront sarà `landscapes:`.
>
>![Struttura delle cartelle in AEM](assets/aem-folder-structure-with-red-boxes.png)


Dopo aver creato i tag in Experience Manager Assets, questi verranno visualizzati nel menu a discesa Tag nella sezione Metadati . Per collegare un campo a un tag, seleziona `xcm:keywords` nell’elenco a discesa Campo Experience Manager Assets nell’area di mappatura metadati.

Per ulteriori informazioni sui tag in Experience Manager Assets, tra cui come creare e gestire i tag, consulta [Amministrazione dei tag](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Campi dello schema dei metadati personalizzati Experience Manager Assets**

È possibile mappare i campi Workfront incorporati e personalizzati ai campi dello schema dei metadati personalizzati in Experience Manager Assets.

I campi di metadati personalizzati creati in Experience Manager Assets sono organizzati nella relativa sezione nell’area di configurazione dei metadati.

![sezione metadati personalizzati](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Campi Workfront**

Puoi mappare i campi Workfront incorporati e personalizzati su Experience Manager Assets. I seguenti valori di campo devono corrispondere sia in lettere maiuscole che minuscole che in corrispondenza dell’ortografia tra Workfront e Experience Manager Assets:

* Campi a discesa
* Campi per selezione multipla

>[!TIP]
>
> Per verificare se i valori dei campi corrispondono esattamente, vai a
>
> * Configurazione > Forms personalizzato in Workfront o nel campo dell’oggetto
> * Risorse > schemi di metadati in Experience Manager Assets


+++

### Mappatura dei metadati per le risorse

I metadati vengono mappati quando una risorsa viene inviata da [!DNL Workfront] per la prima volta. I documenti con campi incorporati o personalizzati vengono mappati automaticamente ai campi specificati al primo invio di una risorsa [!DNL Experience Manager Assets].

Per mappare i metadati per le risorse:

1. Seleziona **[!UICONTROL Risorse]** sopra la tabella metadati.
1. In **[!UICONTROL [!DNL Workfront]field]** scegliere un campo Workfront integrato o personalizzato.

   >[!NOTE]
   >
   >Puoi mappare una singola [!DNL Workfront] campo a più [!UICONTROL Experience Manager Assets] campi. Non è possibile mappare più [!DNL Workfront] campi in un singolo [!DNL Experience Manager Assets] campo .
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->


1. In [!DNL Experience Manager Assets] , cerca tra le categorie prepopolate o inserisci almeno due lettere nel campo di ricerca per accedere alle categorie aggiuntive.
1. Ripetere i passaggi 2 e 3 come necessario.
   ![campi metadati](assets/asset-metadata.png)
1. Fai clic su [!UICONTROL Salva] o passare alla [Cartelle](#folders) in questo articolo.

### Mappare metadati per le cartelle

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
1. Fai clic su **Salva** o passare alla [Configurare i flussi di lavoro (facoltativo)](#set-up-workflows-optional) in questo articolo.

<!--Courtney start here-->

## Configurare i flussi di lavoro (facoltativo)

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. In qualità di amministratore di Workfront, puoi configurare i flussi di lavoro in Workfront, quindi assegnarli ai modelli di progetto. Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

I valori del flusso di lavoro predefiniti impostati nell’integrazione possono essere ignorati a livello di Modello di progetto e di Progetto.

### Configurare un flusso di lavoro per la creazione di cartelle collegate Adobe Experience Manager

1. Attiva/disattiva la **[!UICONTROL Crea cartella collegata]** su.
1. Scegli un percorso di cartella per indicare la posizione in cui dovranno essere associate tutte le cartelle collegate a questa integrazione.
   ![Navigazione cartelle collegate](assets/select-folder-aem-integration.png)
1. Abilita la **Aggiungi nomi di Portfoli e programmi** per includere automaticamente i nomi dei Portfoli e dei programmi alla fine del nome della cartella collegata.
1. Fai clic su **Salva** o passare alla [Configurare cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.

<!--Courtney end here-->

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

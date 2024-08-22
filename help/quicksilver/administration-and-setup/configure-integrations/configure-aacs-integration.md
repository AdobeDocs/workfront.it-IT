---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configura l'integrazione di [!UICONTROL Experience Manager Assets as a Cloud Service]
description: Puoi collegare il tuo lavoro al contenuto in [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 0%

---

# Configura l&#39;integrazione di [!UICONTROL Experience Manager Assets as a Cloud Service]

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Questa funzionalità è disponibile solo per le organizzazioni che sono state caricate in [!DNL Adobe Admin Console].

È possibile collegare il proprio lavoro al contenuto in [!DNL Experience Manager Assets]&#x200B;:

* Invio di risorse e metadati da [!DNL Adobe Workfront] a [!DNL Experience Manager Assets]&#x200B;
* Collega risorse da [!DNL Experience Manager Assets] ai tuoi progetti e attività in [!DNL Workfront&#x200B;]
* Facilitare i casi di utilizzo del controllo delle versioni
* Crea cartelle collegate a [!DNL Experience Manager Assets]
* Tracciare i metadati per risorse e cartelle
* Sincronizza metadati progetto tra [!DNL Workfront] e [!DNL Experience Manager Assets]

>[!NOTE]
>
>È inoltre possibile connettere più archivi [!DNL Experience Manager Assets] a un ambiente [!UICONTROL Workfront] o più ambienti [!DNL Workfront] a un archivio [!DNL Experience Manager Assets] tra gli ID organizzazione. Segui le istruzioni di configurazione in questo articolo per ogni integrazione da configurare.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] piano
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenza
   </td>
   <td><p>Corrente: [!UICONTROL Plan]</p>
   <p>Nuovo: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licenza
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Prodotto
   </td>
   <td>Devi avere [!DNL Experience Manager Assets as a Cloud Service] e devi essere aggiunto al prodotto come utente.
   </td>
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

## Prerequisiti

Prima di iniziare,

* [!DNL Workfront] e [!DNL Adobe Experience Manager Assets] devono essere associati a un ID organizzazione in [!DNL Adobe Admin Console]. Per ulteriori informazioni, vedere [Differenze di amministrazione basate su Platform ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Impostare le informazioni sull’integrazione

{{step-1-to-setup}}

1. Seleziona **[!UICONTROL Documenti]** nel pannello a sinistra, quindi seleziona **[!UICONTROL [!DNL Experience Manager]Integrazione]**.

   >[!NOTE]
   >
   >Questa area di configurazione viene visualizzata solo se l&#39;ambiente [!DNL Workfront] è incluso in un [!DNL Adobe Admin Console].

1. Selezionare **[!UICONTROL Aggiungi integrazione [!DNL Experience Manager]]**.
1. Nel campo **[!UICONTROL Nome]**, immetti il nome che desideri che gli utenti visualizzino quando interagiscono con questa integrazione in Workfront e Experience Manager Assets.
1. Nel campo **[!UICONTROL URL di navigazione]**, il sistema popola automaticamente l&#39;URL di navigazione. Questo URL di sola lettura viene utilizzato per collegarsi all&#39;istanza [!DNL Experience Manager] della tua organizzazione dal [!UICONTROL Main Menu] per un accesso rapido.
1. Scegliere un repository dal menu a discesa del repository **[!UICONTROL [!DNL Experience Manager]Assets]**. Il sistema popola automaticamente tutti gli archivi [!DNL Experience Manager] associati all&#39;ID organizzazione a cui è assegnato il profilo utente.
   ![scegli archivio di experience manager](assets/setup-information.png)

1. Fai clic su **[!UICONTROL Salva]** o passa alla sezione [Configura metadati (facoltativo)](#set-up-metadata-optional) in questo articolo.

   >[!NOTE]
   >
   >A causa della complessità dell’integrazione, non è possibile modificare l’archivio dopo il salvataggio della configurazione iniziale.

## Configurazione metadati (facoltativo)

È possibile mappare i dati dell&#39;oggetto [!DNL Workfront] ai campi degli elementi multimediali delle risorse in [!DNL Experience Manager] Assets.

>[!IMPORTANT]
>
>È possibile mappare i metadati solo in una direzione: da [!DNL Workfront] a [!DNL Experience Manager]. Impossibile trasferire i metadati per i documenti collegati a [!DNL Workfront] da [!DNL Experience Manager] a [!DNL Workfront].

### Configurare i campi di metadati

Prima di iniziare la mappatura dei campi di metadati, è necessario configurare i campi di metadati sia in Workfront che in Experience Manager Assets.

Per configurare i campi metadati:

1. Configura uno schema metadati in [!DNL Experience Manager Assets] come spiegato in [Configura la mappatura dei metadati delle risorse tra Adobe [!DNL Workfront] e [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configurare i campi modulo personalizzati in Workfront. [!DNL Workfront] contiene molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, è anche possibile creare campi personalizzati come descritto in [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **Espandi per visualizzare ulteriori informazioni sui campi Workfront e Experience Manager Assets supportati**

**Tag Experience Manager Assets**

Puoi mappare qualsiasi campo supportato da Workfront a un tag in Experience Manager Assets. A questo scopo, è necessario assicurarsi che i valori dei tag in Experience Manager Assets corrispondano a Workfront.

* I valori dei campi Tag e Workfront devono corrispondere esattamente in ortografia e formato.
* I valori dei campi di Workfront mappati sui tag di experience Manager assets devono essere tutti in minuscolo, anche se il tag in Experience Manager Assets sembra avere lettere maiuscole.
* I valori dei campi di Workfront non devono includere spazi.
* Il valore del campo in Workfront deve includere anche la struttura di cartelle del tag Experience Manager Assets.
* Per mappare più campi di testo a riga singola ai tag, immetti un elenco separato da virgole dei valori tag nel lato Workfront della mappatura metadati e `xcm:keywords` nel lato Experience Manager Assets. Ogni valore di campo viene mappato su un tag separato. È possibile utilizzare un campo calcolato per combinare più campi Workfront in un unico campo di testo separato da virgole.
* È possibile mappare i valori dai campi elenco a discesa, pulsante di scelta o casella di controllo immettendo un elenco separato da virgole dei valori disponibili in tale campo.


>[!INFO]
>
>**Esempio**: per far corrispondere il tag visualizzato nella struttura di cartelle, il valore del campo in Workfront sarà `landscapes:trees/spruce`. Osserva le lettere minuscole nel valore del campo Workfront.
>
>Se si desidera che il tag sia l&#39;elemento più a sinistra nella struttura dei tag, è necessario che sia seguito da due punti. In questo esempio, per eseguire il mapping al tag landscapes, il valore del campo in Workfront sarà `landscapes:`.
>
>![Struttura delle cartelle in AEM](assets/aem-folder-structure-with-red-boxes.png)


Dopo aver creato i tag in Experience Manager Assets, vengono visualizzati nel menu a discesa Tag della sezione Metadati. Per collegare un campo a un tag, selezionare `xcm:keywords` nel menu a discesa del campo Experience Manager Assets nell&#39;area di mappatura dei metadati.

Per ulteriori informazioni sui tag in Experience Manager Assets, tra cui come creare e gestire i tag, vedere [Amministrazione dei tag](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Campi schema metadati personalizzati Experience Manager Assets**

Puoi mappare i campi Workfront incorporati e personalizzati ai campi schema metadati personalizzati in Experience Manager Assets.

I campi di metadati personalizzati creati in Experience Manager Assets sono organizzati in una sezione specifica nell’area di configurazione dei metadati.

![sezione metadati personalizzata](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Campi Workfront**

Puoi mappare su Experience Manager Assets i campi Workfront incorporati e personalizzati. I seguenti valori dei campi devono corrispondere tra Workfront e Experience Manager Assets sia in maiuscolo che in minuscolo:

* Campi a discesa
* Campi a selezione multipla

>[!TIP]
>
> Per verificare se i valori dei campi corrispondono esattamente, vai a
>
> * Configurazione > Forms personalizzato in Workfront o il campo nell’oggetto
> * Assets > schemi metadati in Experience Manager Assets

+++

### Mappare i metadati per le risorse

I metadati vengono mappati quando una risorsa viene inviata per la prima volta da [!DNL Workfront]. I documenti con i campi predefiniti o personalizzati vengono mappati automaticamente ai campi specificati la prima volta che una risorsa viene inviata a [!DNL Experience Manager Assets].

Per mappare i metadati delle risorse:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Nella colonna **[!UICONTROL [!DNL Workfront]campo]** scegliere un campo Workfront predefinito o personalizzato.

   >[!NOTE]
   >
   >È possibile mappare un singolo campo [!DNL Workfront] a più campi [!UICONTROL Experience Manager Assets]. Impossibile mappare più campi [!DNL Workfront] a un singolo campo [!DNL Experience Manager Assets].
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Nel campo [!DNL Experience Manager Assets], eseguire la ricerca nelle categorie precompilate o immettere almeno due lettere nel campo di ricerca per accedere ad altre categorie.
1. Ripetere i passaggi 2 e 3 in base alle esigenze.
   ![campi metadati](assets/metadata-no-asset-toggle.png)
1. Fai clic su [!UICONTROL Salva] o passa alla sezione [Configura flussi di lavoro](#set-up-workflows-optional) in questo articolo.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Impostare i flussi di lavoro (facoltativo)

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. In qualità di amministratore di Workfront, puoi configurare i flussi di lavoro in Workfront e quindi assegnarli a Modelli di progetto. Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

I flussi di lavoro sono abilitati e configurati per Adobe Experience Manager nel suo complesso. Questi flussi di lavoro possono quindi essere applicati ai modelli di progetto e modificati o personalizzati a livello di modello o di progetto.

Nell’integrazione di Adobe Experience Manager sono disponibili i seguenti flussi di lavoro:

* [Creare cartelle collegate a Adobe Experience Manager](#create-adobe-experience-manager-linked-folders)
* [Risorse Publish inviate ad Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Creare cartelle collegate a Adobe Experience Manager

1. Attiva **[!UICONTROL Crea cartella collegata]**.
1. Immettere un nome per la cartella collegata che si sta creando.
1. (Condizionale) Abilitare l&#39;opzione **Struttura cartelle predefinita** se si desidera che questa cartella collegata sia la cartella predefinita per i progetti creati con modelli che utilizzano questa integrazione. È possibile selezionare una o più cartelle predefinite.
1. Scegli un percorso di cartella per indicare dove desideri che tutte le cartelle collegate siano associate a questa integrazione.
1. (Condizionale) Per aggiungere una struttura di cartelle (cartelle nidificate) a questa integrazione, effettua le seguenti operazioni:

   1. Fai clic sull&#39;icona **Aggiungi cartella** ![Aggiungi cartella](assets/add-folder-aem.png).
   1. Nel campo **Tipo nome**, selezionare la modalità di denominazione della cartella:

      * **Nome**: immettere un nome per la cartella.
      * **Dati oggetto**: selezionare l&#39;origine per il nome della cartella, ad esempio Nome progetto.

      >[!NOTE]
      >
      >* I nomi delle cartelle devono contenere meno di 100 caratteri.
      >* I seguenti caratteri verranno rimossi dai nomi delle cartelle:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Per aggiungere una cartella nidificata all&#39;albero delle cartelle, fare clic sul menu a tre punti accanto alla cartella in cui si desidera creare una cartella nidificata e selezionare **Aggiungi cartella**. Compila i campi come descritto nel passaggio precedente.
   1. Per collegare una cartella a Workfront, selezionarla e fare clic su **Crea cartella collegata**   icona ![Collega cartella](assets/link-folder.png).
   1. (Facoltativo) Per modificare una cartella, selezionarla e fare clic sull&#39;icona **Modifica cartella** ![Modifica icona](assets/edit-icon.png).
   1. (Facoltativo) Per eliminare una cartella, selezionarla e fare clic sull&#39;icona **Elimina cartella** ![Elimina cartella](assets/delete-folder.png).
1. (Condizionale) Per aggiungere un&#39;altra struttura di cartelle, fare clic su **+ Aggiungi struttura di cartelle** e seguire la procedura descritta nel passaggio 5.

1. Fai clic su **[!UICONTROL Salva]** o passa alle [risorse Publish inviate ad Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) in questo articolo.

>[!NOTE]
>
>* Questa integrazione non creerà più di 100 cartelle, indipendentemente dal numero di strutture di cartelle create. Ad esempio, un’integrazione con 4 strutture di cartelle può creare fino a 100 cartelle, non 400.
>* La prima cartella nella struttura delle cartelle viene automaticamente contrassegnata come collegata a Workfront. Se non desideri collegare questa cartella, puoi scollegarla.
>* Se non viene fornita alcuna struttura di cartelle, la cartella principale diventa la cartella collegata.


### Risorse Publish inviate ad Adobe Experience Manager Assets

1. Attiva automaticamente **[!UICONTROL risorse Publish]**.
1. Seleziona la casella accanto al percorso in cui desideri pubblicare le risorse inviate alle risorse Adobe Experience Manager. Puoi abilitare una o entrambe le opzioni.
1. (Condizionale) Se hai attivato l’opzione Brand Portal, seleziona il Brand Portal in cui desideri pubblicare le risorse.
1. Fai clic su **[!UICONTROL Salva]** o passa alla sezione [Configura cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.

## Configurare le cartelle collegate (facoltativo)

È possibile consentire agli utenti di creare cartelle collegate a [!DNL Experience Manager] durante un progetto [!DNL Workfront]. Quando una cartella viene collegata, qualsiasi risorsa aggiunta alla cartella viene visualizzata automaticamente sia in [!DNL Workfront] che in [!DNL Experience Manager]. Quando una risorsa viene aggiunta alla cartella collegata in [!DNL Workfront] per la prima volta, i metadati della risorsa vengono inviati a [!DNL Experience Manager Assets].

Nei passaggi seguenti, indichi dove desideri creare le cartelle collegate. Ogni integrazione può avere una sola posizione per tutte le cartelle collegate.

Per impostare le cartelle collegate:

1. Attiva **[!UICONTROL Abilita cartella collegata]**.
1. Scegli un percorso di cartella per indicare dove desideri che tutte le cartelle collegate siano associate a questa integrazione.

   >[!NOTE]
   >
   >Gli utenti devono poter accedere in scrittura in [!DNL Adobe Experience Manager Assets] alla cartella specificata per creare una cartella collegata.

1. Fai clic su **[!UICONTROL Salva]**.

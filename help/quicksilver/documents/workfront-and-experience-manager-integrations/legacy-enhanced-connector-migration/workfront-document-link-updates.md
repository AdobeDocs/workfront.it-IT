---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Eseguire la migrazione di cartelle e documenti collegati
description: Puoi utilizzare l’API per migrare cartelle e documenti collegati in Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Eseguire la migrazione di cartelle e documenti collegati

Puoi utilizzare l’API per migrare cartelle e documenti collegati in Adobe Experience Manager Assets.

## Procedura

1. Identificare tutti i documenti e le cartelle collegati al precedente provider di archiviazione documenti esterno, notando i relativi identificatori interni di documenti o cartelle Workfront e l&#39;ID cartella di qualsiasi cartella contenitore.

   >[!NOTE]
   >
   > È necessario verificare che non sia già stato creato un collegamento con il nuovo provider per tutte le cartelle o tutti i documenti individuati.

1. Individuare i documenti e le cartelle nel nuovo repository in base al percorso, quindi cercare la relativa identità nel sistema esterno.

1. Crea una mappatura dell’ID Workfront interno sull’ID nel nuovo archivio esterno. Per creare un nuovo collegamento, segui il passaggio seguente.

1. Crea un nuovo collegamento a documento o cartella documenti in Workfront, che punta alla risorsa nella nuova posizione tramite il nuovo ID esterno.

   1. **Documenti**: aggiungi una nuova versione del documento esistente con il nuovo provider di documenti esterno.
   1. **Cartelle**: crea una nuova cartella nella stessa posizione con lo stesso nome.

>[!CAUTION]
>
>   Non eliminare le cartelle collegate esistenti. Questo potrebbe causare la perdita di dati. Per rimuovere i vecchi collegamenti alle cartelle dall’applicazione Workfront, disabilita l’integrazione dei documenti personalizzati nell’area Setup.


## Processo di esempio per la migrazione dei collegamenti

![flusso di collegamento semplificato](assets/links-flow-simplified.png)

## Informazioni API

Per ulteriori informazioni sulle API di Workfront in questa sezione, consulta [Documentazione per sviluppatori:Documenti](https://developer.workfront.com/documents.html).

### Trova tutti i documenti

Trova tutto **Documenti (DOCU)** Collegato a **Provider documento** di **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Documentazione di riferimento API](https://developer.workfront.com/documents.html#get-/docu/search)

### Trova tutte le cartelle

Trova tutto **Cartelle documenti (DOCFDR)** Collegato al provider di documenti di **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

DOCS API: (gli endpoint per cartelle di documenti non sono attualmente inclusi in developer.workfront.com)

### Collega documenti

Collegamento **Documenti (DOCU)** da **Provider documento esterno** di **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>I documenti vengono archiviati temporaneamente. Ciò significa che è possibile accedere a tutte le versioni del documento. Quando crei il collegamento, puoi specificare l’ID del documento esistente. In tal modo, ti basta scrivere una nuova versione del documento e i dati vengono ospitati esternamente nel nuovo provider. L&#39;ID documento è uguale all&#39;ID documento trovato nel collegamento documento che si sta sostituendo. È lo stesso documento concettuale. Stai semplicemente indicando che i byte per questa nuova versione sono memorizzati con un provider diverso.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

DOCUMENTAZIONE API: (gli endpoint per collegamenti interni non sono attualmente inclusi in developer.workfront.com)

### Collega cartelle

Collegamento **Cartelle documenti (DOCFDR)** da **Provider documento esterno** di **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>Per i collegamenti alle cartelle, a differenza dei collegamenti ai documenti, è necessario &quot;documentFolderId&quot; della cartella in Workfront in cui si desidera inserire il nuovo collegamento. Si tratta probabilmente della stessa cartella principale della cartella collegata in fase di copia.

>[!CAUTION]
>
>Le cartelle non vengono archiviate temporalmente. Non eliminare le vecchie cartelle. Per rimuovere le vecchie cartelle, disabilita l’integrazione del documento personalizzato nell’area di configurazione.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

DOCUMENTAZIONE API: (gli endpoint per collegamenti interni non sono attualmente inclusi in developer.workfront.com)

## Termini importanti

* **Documento**: risorsa digitale in Workfront

* **Cartella documenti**: contenitore per risorse digitali in Workfront

* **ID documento**: ID interno di Workfront per una risorsa digitale

* **ID cartella documenti**: ID interno di Workfront per una cartella di risorse digitali

* **ID provider documenti**: ID associato a provider di documenti specifici

>[!IMPORTANT]
>
> Per un determinato tipo di provider di documenti, un cliente può avere più istanze collegate. Ad esempio, possono avere più archivi AEM collegati. Oppure più istanze di Google Drive collegate. L&#39;ID del provider di documenti indica l&#39;istanza specifica del tipo di connessione che si desidera sostituire o a cui si desidera passare.

* **Tipo di provider di archiviazione documenti (anche &quot;tipo di integrazione esterna&quot;)**: tipo di integrazione del provider di archiviazione dei documenti supportata da Workfront. Tramite un’integrazione dedicata o una &quot;integrazione personalizzata&quot;.

* **Tipi di provider di archiviazione documenti correnti ( providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Documento collegato**: risorsa digitale ospitata in un provider di archiviazione documenti esterno. Workfront avrà un proprio &quot;ID documento&quot; interno per la risorsa, ma i byte vengono memorizzati esternamente. Per facilitare questa operazione, Workfront memorizza anche un &quot;ID documento esterno&quot; per facilitare l’individuazione della risorsa a cui si fa riferimento esternamente all’interno dell’archivio o dell’archivio remoto.

* **Cartella documenti collegati**: contenitore per risorse digitali ospitato in un provider di archiviazione documenti esterno. Workfront avrà un proprio &quot;ID cartella documenti&quot; interno per la risorsa, ma i byte vengono archiviati esternamente. Per facilitare questa operazione, Workfront memorizza anche un &quot;ID documento esterno&quot; per facilitare l’individuazione della risorsa a cui si fa riferimento esternamente all’interno dell’archivio o dell’archivio remoto.

* **ID documento esterno**: ID assegnato quando le risorse vengono memorizzate al di fuori di Workfront. Workfront mappa il proprio identificatore interno all’identificatore utilizzato per individuare la risorsa nel sistema esterno, tramite questo campo &quot;identificatore documento esterno&quot;. Pertanto, quando si collega il documento o la cartella da un nuovo archivio esterno, è necessario comporre un nuovo identificatore di documento esterno nel formato appropriato affinché il provider di documenti esterni possa identificare il documento nel nuovo archivio o archivio.

  >[!NOTE]
  >
  > Workfront non dispone ancora di uno standard per gli identificatori di documenti esterni. È in uso una nuova specifica per gli ID AEM, ma per altri ID, l’ID documento esterno può assumere forme diverse a seconda del tipo di provider.


* **Tipo di oggetto**: termine utilizzato solo nelle API ai fini del presente documento. Si tratta di un tipo di oggetto generico all’interno di Workfront con cui desideri interagire. In questi casi, si interagirà con documenti e cartelle di tipo &quot;DOCU&quot; e &quot;DOCFDR&quot; rispettivamente.

* **ID oggetto**: identificatore interno di Workfront per l’oggetto generico con cui desideri interagire. Interagirai con documenti e cartelle in modo che questo sia rispettivamente l’ID del documento o l’ID della cartella del documento.

---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrazione di cartelle e documenti collegati
description: Puoi utilizzare l’API per migrare cartelle e documenti collegati ad Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Migrazione di cartelle e documenti collegati

Puoi utilizzare l’API per migrare cartelle e documenti collegati ad Adobe Experience Manager Assets.

## Procedura

1. Identificare tutti i documenti e le cartelle collegati al provider di archiviazione documenti esterno precedente, annotando gli identificatori dei documenti o delle cartelle interni di Workfront e l&#39;ID della cartella di qualsiasi cartella contenente.

   >[!NOTE]
   >
   > È necessario verificare che tutte le cartelle o i documenti scoperti non abbiano già creato un collegamento con il nuovo provider.

1. Individua i documenti e le cartelle nel nuovo archivio in base al percorso, quindi cerca la loro identità nel sistema esterno.

1. Crea una mappatura dell’ID Workfront interno all’ID nel nuovo archivio esterno. Per creare un nuovo collegamento, effettua le seguenti operazioni.

1. Crea un nuovo collegamento a una cartella di documenti o documenti in Workfront, indicando la risorsa nella nuova posizione tramite il nuovo ID esterno.

   1. **Documenti**: Aggiungere una nuova versione del documento esistente con il nuovo provider di documenti esterno.
   1. **Cartelle**: Crea un nuovo filtro nella stessa posizione con lo stesso nome.

>[!CAUTION]
>
>   Non eliminare le cartelle collegate esistenti. Questo potrebbe causare la perdita di dati. Per rimuovere i vecchi collegamenti alle cartelle dall&#39;applicazione Workfront, disattivare l&#39;integrazione dei documenti personalizzati nell&#39;area Configurazione.


## Esempio di processo per la migrazione dei collegamenti

![flusso di collegamento semplificato](assets/links-flow-simplified.png)

## Informazioni API

Per ulteriori informazioni sulle API di Workfront in questa sezione, vedi [Documentazione per gli sviluppatori:Documenti](https://developer.workfront.com/documents.html).

### Trova tutti i documenti

Trova tutto **Documenti (DOCU)** Collegato a **Provider di documenti** di **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Riferimento API DOCS](https://developer.workfront.com/documents.html#get-/docu/search)

### Trova tutte le cartelle

Trova tutto **Cartelle documenti (DOCFDR)** Collegato al provider di documenti di **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

DOCS API: (Endpoint cartella documenti non attualmente coperti da developer.workfront.com)

### Collegamento di documenti

Collegamento **Documenti (DOCU)** da **Provider di documenti esterni** di **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>I documenti vengono archiviati temporaneamente. Ciò significa che puoi accedere a tutte le versioni del documento. Quando crei il collegamento, puoi specificare l’ID del documento esistente, in modo da scrivere semplicemente una nuova versione del documento e i dati saranno ospitati esternamente nel nuovo provider. Questo ID documento corrisponde all&#39;ID documento trovato sul collegamento documento che si sta sostituendo. È lo stesso documento concettuale. Stai semplicemente indicando che i byte per questa nuova versione sono memorizzati con un provider diverso.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

DOCS API: (Endpoint di collegamento interni non attualmente coperti da developer.workfront.com)

### Collega cartelle

Collegamento **Cartelle documenti (DOCFDR)** da **Provider di documenti esterni** di **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>Per i collegamenti alle cartelle , a differenza dei collegamenti a documenti, è necessario disporre del &#39;documentFolderId&#39; della cartella in Workfront in cui si desidera inserire il nuovo collegamento. Si tratta probabilmente della stessa cartella padre della cartella collegata che stiamo copiando.

>[!CAUTION]
>
>Le cartelle non vengono memorizzate in modo temporaneo. Non eliminare le vecchie cartelle. Disattiva l&#39;integrazione del documento personalizzato nell&#39;area di configurazione per rimuovere le vecchie cartelle.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

DOCS API: (Endpoint di collegamento interni non attualmente coperti da developer.workfront.com)

## Termini importanti

* **Documento**: Una risorsa digitale in Workfront

* **Cartella documenti**: Un contenitore per risorse digitali in Workfront

* **ID documento**: ID interno Workfront per una risorsa digitale

* **ID cartella documenti**: ID interno Workfront per una cartella di risorse digitali

* **ID fornitore documenti**: ID associato a provider di documenti specifici

>[!IMPORTANT]
>
> Per un determinato tipo di provider di documenti, un cliente può avere più istanze collegate. Possono avere più archivi AEM collegati, ad esempio. Oppure più istanze di Google Drive collegate. L&#39;ID del provider di documenti indica l&#39;istanza specifica del tipo di connessione a cui si desidera sostituire o passare.

* **Tipo di provider di archiviazione documenti (anche &quot;Tipo di integrazione esterna&quot;)**: Tipo di integrazione del provider di archiviazione documenti supportata da Workfront. Tramite un’integrazione dedicata o un’&quot;integrazione personalizzata&quot;.

* **Tipi di provider di archiviazione documenti correnti (providerType)**:

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

* **Documento collegato**: Una risorsa digitale ospitata in un provider di archiviazione documenti esterno. Workfront avrà il proprio &quot;ID documento&quot; interno per la risorsa, ma i byte vengono memorizzati esternamente. Per facilitare questa fase, Workfront memorizza anche un &quot;ID documento esterno&quot; per facilitare l’individuazione della risorsa di riferimento esterno all’interno dell’archivio o dell’archivio remoto.

* **Cartella documenti collegati**: Un contenitore per risorse digitali ospitato in un provider di archiviazione documenti esterno. Workfront avrà il proprio &quot;ID cartella documenti&quot; interno per la risorsa, ma i byte vengono memorizzati esternamente. Per facilitare questa fase, Workfront memorizza anche un &quot;ID documento esterno&quot; per facilitare l’individuazione della risorsa di riferimento esterno all’interno dell’archivio o dell’archivio remoto.

* **ID documento esterno**: ID assegnato quando le risorse vengono memorizzate al di fuori del workfront. Workfront mappa il proprio identificatore interno all’identificatore utilizzato per individuare la risorsa nel sistema esterno, tramite questo campo &quot;identificativo del documento esterno&quot;. Pertanto, quando si collega il documento o la cartella da un nuovo archivio esterno, è necessario comporre un nuovo identificativo del documento esterno nel formato appropriato per consentire al provider di documenti esterno di identificare il documento nel nuovo archivio o archivio.

   >[!NOTE]
   >
   > Workfront non dispone ancora di uno standard per gli identificatori dei documenti esterni. Per gli ID AEM viene utilizzata una nuova specifica, ma per altri ID, l’ID documento esterno può assumere moduli diversi a seconda del tipo di provider.


* **Tipo di oggetto**: Si tratta di un termine API solo ai fini del presente documento. È un tipo di oggetto generico all&#39;interno del workfront con cui si desidera interagire. In questi casi, interagirai con documenti e cartelle con i tipi &quot;DOCU&quot; e &quot;DOCFDR&quot; rispettivamente.

* **ID oggetto**: Identificatore Workfront interno per l&#39;oggetto generico con cui si desidera interagire. È possibile interagire con documenti e cartelle in modo che questo sia rispettivamente l&#39;ID del documento o l&#39;ID della cartella del documento.

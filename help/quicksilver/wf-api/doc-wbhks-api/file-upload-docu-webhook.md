---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Caricamento di file tramite webhook dei documenti
description: Caricamento di file tramite webhook dei documenti
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
TQID: https://experienceleague.adobe.com/qLRbcWkbOxvBp5Xw1aCLjGZXHMtu2k70NgOonZsZ0lk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 11%

---

# Caricamento di file tramite webhook dei documenti

Il caricamento di un file in un provider di archiviazione documenti è un processo in due fasi che richiede due endpoint API separati. Adobe Workfront avvia il processo di caricamento chiamando /uploadInit. Questo endpoint restituisce un ID documento che viene quindi passato a /upload durante il caricamento dei byte del documento. A seconda del sistema di archiviazione dei documenti sottostante, potrebbe essere necessario creare un documento a lunghezza zero, quindi aggiornare il contenuto del documento in un secondo momento.

Aggiunto alla versione 1.1 di questa specifica, l&#39;ID documento e l&#39;ID versione documento possono essere utilizzati per recuperare informazioni aggiuntive da Workfront.

**Esempio:** se il sistema di gestione dei documenti desidera ulteriori informazioni sul documento, il codice di implementazione del webhook potrebbe utilizzare l&#39;ID del documento per recuperare tali informazioni utilizzando l&#39;API RESTful di Workfront. È buona norma che queste informazioni provengano dai campi dati personalizzati del documento che contengono l&#39;attività, il problema o il progetto.

## Metodo POST

**URL**

POST /uploadInit

### Parametri di query

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>ID della cartella principale, come indicato dal provider del webhook.</td> 
  </tr> 
  <tr> 
   <td>nome file </td> 
   <td>Nome del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>ID documento Workfront (aggiunto nella versione 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>ID versione documento Workfront (aggiunto nella versione 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## Risposta

I metadati del file, come definito dall’endpoint /metadata. Questo include l’ID documento utilizzato dal provider.

**Esempio:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Metodo PUT

Carica i byte di un documento nel provider del webhook.

**URL**

PUT/upload

## Parametri di query

| Nome  | Descrizione |
|---|---|
| ID  |  ID del documento appena creato. |


**Corpo richiesta**

Byte di contenuto non elaborato per il documento.

**Risposta**

```
{
result: "success"
}
```

oppure

```
{
result: "fail"
}
```

**Esempio**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

risposta

```
{
result:"success"
}
```

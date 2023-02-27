---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Caricamento di file tramite Webhook di documenti
description: Caricamento di file tramite Webhook di documenti
author: Becky
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# Caricamento di file tramite Webhook di documenti

Il caricamento di un file in un provider di archiviazione dei documenti è un processo in due fasi che richiede due endpoint API separati. Adobe Workfront inizia il processo di caricamento chiamando /uploadInit . Questo endpoint restituisce un ID documento che viene quindi passato a /upload durante il caricamento dei byte del documento. A seconda del sistema di archiviazione dei documenti sottostante, potrebbe essere necessario creare un documento a lunghezza zero, quindi aggiornare il contenuto del documento in un secondo momento.

Aggiunto alla versione 1.1 di questa specifica, l’ID del documento e l’ID della versione del documento possono essere utilizzati per recuperare ulteriori informazioni da Workfront.

**Esempio:** Se il sistema di gestione dei documenti desidera ulteriori informazioni sul documento, il codice di implementazione del webhook potrebbe utilizzare l’ID del documento per recuperare tali informazioni utilizzando l’API RESTful di Workfront. Come procedura ottimale, queste informazioni possono provenire da campi di dati personalizzati nel documento e contengono attività, problemi o progetti.

## Metodo POST

**URL**

POST /uploadInit

### Parametri query

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
   <td>ID della cartella principale, a cui fa riferimento il provider webhook.</td> 
  </tr> 
  <tr> 
   <td>nomefile </td> 
   <td>Nome del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>ID del documento Workfront (aggiunto nella versione 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>ID versione del documento Workfront (aggiunto nella versione 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## risposta

I metadati per il file, come definito dall&#39;endpoint /metadata. Questo include l&#39;ID del documento utilizzato dal provider.

**Esempio:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Metodo PUT

Carica i byte di un documento nel provider webhook.

**URL**

PUT /upload

## Parametri query

| Nome  | Descrizione |
|---|---|
| id  |  ID documento appena creato. |


**Corpo della richiesta**

Byte di contenuto non elaborati per il documento.

**Risposta**

```
{
result: “success”
}
```

oppure

```
{
result: “fail”
}
```

**Esempio**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

response

```
{
result:"success"
}
```

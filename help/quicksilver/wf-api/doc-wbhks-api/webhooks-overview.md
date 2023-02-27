---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Panoramica dei webhook
description: Panoramica dei webhook
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Panoramica dei webhook

Adobe Workfront Document Webhooks definisce un set di endpoint API attraverso i quali Workfront effettua chiamate API autorizzate a un provider di documenti esterno. Questo consente a chiunque di creare un plug-in middleware per qualsiasi provider di archiviazione documenti.

![](assets/mceclip0-350x262.png)

L’esperienza utente per le integrazioni basate su webhook sarà simile a quella delle integrazioni di documenti esistenti, come Google Drive, Box e Dropbox. Ad esempio, un utente di Workfront sarà in grado di eseguire le azioni seguenti:

* Spostarsi nella struttura delle cartelle del provider di documenti esterno
* File di ricerca
* Collegare file in Workfront
* Caricare file nel provider di documenti esterno
* Visualizzare una miniatura del documento

**Implementazione di riferimento**

Per aiutarti a dare un impulso allo sviluppo di una nuova implementazione dei webhook, Workfront fornisce un’implementazione di riferimento. Il codice è disponibile all&#39;indirizzo [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Questa implementazione è basata su Java e consente a Workfront di collegare documenti a un file system di rete. 

## Versioni

* Versione 1.0 (data di rilascio - maggio 2015): Specifica iniziale

* Versione 1.1 (data di rilascio - giugno 2015). Aggiornati /uploadInit - Aggiunti documentId e documentVersionId

* Versione 1.2 (data di rilascio - ottobre 2015): Aggiunto /createFolder

* Versioni successive (Data di rilascio - TBD):

   * Aggiunto /delete
   * Aggiunto/rinomina
   * Aggiunto /serviceInfo
   * Aggiunto /customAction
   * Aggiungi pagination e parentId a /search

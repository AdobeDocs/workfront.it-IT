---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Panoramica dei webhook
description: Panoramica dei webhook
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: eb738fa8cadaafb0332c5c78a3816d5c346c33b2
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Panoramica dei webhook

Adobe Workfront Document Webhooks definisce un set di endpoint API attraverso i quali Workfront effettua chiamate API autorizzate a un provider di documenti esterno. Questo consente a chiunque di creare un plug-in middleware per qualsiasi provider di archiviazione dei documenti.

![](assets/mceclip0-350x262.png)

L’esperienza utente per le integrazioni basate su webhook sarà simile a quella delle integrazioni di documenti esistenti, come Google Drive, Box e Dropbox. Ad esempio, un utente di Workfront sarà in grado di eseguire le azioni seguenti:

* Spostarsi nella struttura di cartelle del provider di documenti esterno
* Cerca file
* Collegare i file in Workfront
* Carica file nel provider di documenti esterno
* Visualizza una miniatura per il documento

**Implementazione di riferimento**

Per aiutarti a iniziare lo sviluppo di una nuova implementazione di webhook, Workfront fornisce esempi di implementazione di riferimento. Questi esempi sono disponibili all&#39;indirizzo [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Gli esempi sono basati su Java e consentono a Workfront di collegare documenti su un file system di rete. 

>[!NOTE]
>
>Le risorse su GitHub sono solo esempi e non sono in grado di eseguire un’implementazione.

## Versioni

* Versione 1.0 (Data di rilascio: maggio 2015): specifiche iniziali

* Versione 1.1 (Data di rilascio: giugno 2015). Aggiornato /uploadInit - Aggiunti documentId e documentVersionId

* Versione 1.2 (Data di rilascio: ottobre 2015): aggiunta di /createFolder

* Versioni future (data di rilascio - da definire):

   * Aggiunto/elimina
   * Aggiunto /rename
   * Aggiunto /serviceInfo
   * Aggiunta di /customAction
   * Aggiungi paginazione e parentId a /search

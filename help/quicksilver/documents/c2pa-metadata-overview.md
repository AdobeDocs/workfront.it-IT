---
product-area: documents
navigation-topic: documents-navigation-topic
title: Metadati C2PA in Adobe Workfront
description: Scopri cosa sono i metadati C2PA e come Adobe Workfront li conserva nei documenti che carichi, archivi e scarichi.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Metadati C2PA in Adobe Workfront

I metadati C2PA sono informazioni sicure e in grado di evidenziare eventuali manomissioni che viaggiano con un contenuto. Quando si utilizza l&#39;intelligenza artificiale generativa (GenAI) per creare o modificare un&#39;immagine, un video o un file audio, i metadati C2PA registrano tale fatto in modo che chiunque riceva il file possa vedere come è stato creato.

I metadati C2PA si basano sullo standard aperto [C2PA](https://c2pa.org/).

## Cosa contengono i metadati C2PA

I metadati C2PA includono:

* Nome del provider che ha fornito lo strumento GenAI.
* Nome e numero di versione del sistema GenAI utilizzato per creare o modificare il contenuto.
* La data e l’ora in cui il contenuto è stato creato o modificato.
* Un identificatore univoco.

I metadati C2PA non includono informazioni personali (PII, personally identifiable information).

## Gestione dei metadati C2PA in Workfront

Adobe Workfront non modifica i metadati dei file con cui lavori. Quando caricate un file che contiene già metadati C2PA, Workfront mantiene tali informazioni invariate in quanto il file viene memorizzato in e scaricato da Workfront.

Poiché i metadati sono incorporati nel file stesso, rimangono intatti attraverso i flussi di lavoro di Workfront, in modo che le informazioni sulla provenienza rimangano con il contenuto quando lascia Workfront.

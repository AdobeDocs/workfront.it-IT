---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Risoluzione dei problemi di creazione della bozza
description: Il processo di creazione delle prove include sia l'importazione che la generazione della bozza. Talvolta, durante la creazione di una bozza, è possibile che l’importazione di un file non riesca o che la bozza non venga generata dopo l’importazione del file.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Risoluzione dei problemi di creazione della bozza

Il processo di creazione delle prove include sia l&#39;importazione che la generazione della bozza. Talvolta, durante la creazione di una bozza, è possibile che l’importazione di un file non riesca o che la bozza non venga generata dopo l’importazione del file.

>[!NOTE]
>
> Se il documento che stai tentando di provare non soddisfa nessuno dei criteri elencati in questa sezione, contatta il supporto Adobe Workfront per ulteriori indagini.

## Motivi dell’errore di importazione

* È stata creata una bozza combinata contenente più di 50 file.

## Motivi dell’errore di generazione della prova

* Il tipo di file non è supportato.\
   Per un elenco dei tipi di file supportati, consulta [Panoramica sui tipi di file di correzione supportati e sui limiti di dimensione](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La struttura del file è una struttura non standard per il tipo di file.
* Il file è protetto da una password o la copia del contenuto è disabilitata.

   A differenza di altri tipi di file, i file PDF possono essere generati nelle bozze se l’impostazione di sicurezza per la copia dei contenuti è impostata su Consentito in PDF.

* La lunghezza o il conteggio delle pagine supera il limite.

   La lunghezza massima consentita della pagina è di 195 pollici dopo la rasterizzazione; il numero massimo consentito di pagine è 1.000 pagine per una singola bozza.

* Il file è danneggiato o danneggiato.
* La scadenza del flusso di lavoro per una nuova versione di prova è passata.

   Ciò si verifica quando si crea una nuova versione di prova utilizzando un metodo di prova rapida e **Generazione automatica di bozze durante il caricamento di documenti** è selezionato. La nuova versione di prova tenta di prendere le scadenze del flusso di lavoro dalla bozza generata in precedenza. La generazione di prove fallisce se queste scadenze sono passate. Per ovviare a questo problema, puoi impostare le scadenze del flusso di lavoro per la versione precedente in futuro o generare una nuova versione di prova. Se generi una nuova versione, utilizza **Altro > Nuova versione > Prova** e seleziona **Tempistiche per i flussi di lavoro in futuro**.

* Durante la correzione dei file PDF, i motivi dell’errore di generazione della bozza includono:

   * I font e le immagini sono collegati da origini esterne (ad esempio dal file system locale)

      I font e le immagini devono essere incorporati nel file PDF per poter essere visualizzati su un altro computer o in Workfront Proof.

   * Il file PDF contiene livelli vuoti o campi trasparenti o sovrapposti.

      Se non è possibile determinare quale livello o oggetto causa questo problema, esportare la progettazione o il documento come PDF ottimizzato (questo rimuove tutti gli elementi indesiderati).


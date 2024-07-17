---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Risoluzione dei problemi di creazione delle bozze
description: Il processo di creazione della bozza include sia l’importazione che la generazione della bozza. Talvolta, durante la creazione di una bozza, un file potrebbe non essere importato o la bozza potrebbe non essere generata dopo l’importazione.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Risoluzione dei problemi di creazione delle bozze

Il processo di creazione della bozza include sia l’importazione che la generazione della bozza. Talvolta, durante la creazione di una bozza, un file potrebbe non essere importato o la bozza potrebbe non essere generata dopo l’importazione.

>[!NOTE]
>
> Se il documento che stai tentando di verificare non soddisfa nessuno dei criteri elencati in questa sezione, contatta il supporto Adobe Workfront per ulteriori indagini.

## Motivi di un errore di importazione

* È stata creata una bozza combinata contenente oltre 50 file.

## Motivi per la mancata generazione della bozza

* Tipo di file non supportato.\
  Per un elenco dei tipi di file supportati, vedere [Panoramica sui tipi di file di verifica supportati e sui limiti di dimensione](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La struttura del file non è standard per il tipo di file.
* Il file è protetto da password o la copia del contenuto è disabilitata.

  A differenza di altri tipi di file, i file PDF possono essere generati in bozze se l’impostazione di sicurezza per la copia del contenuto è impostata su Consentita in PDF.

* La lunghezza della pagina o il numero di pagine supera il limite consentito.

  La lunghezza massima consentita per la pagina è di 195 pollici dopo la rasterizzazione; il numero massimo consentito di pagine è di 1.000 pagine per una singola bozza.

* Il file è danneggiato.
* La scadenza del flusso di lavoro per una nuova versione della bozza è nel passato.

  Ciò si verifica quando si crea una nuova versione della bozza utilizzando un metodo di bozza rapido e si seleziona **Genera automaticamente bozze durante il caricamento dei documenti**. La nuova versione della bozza tenta di recuperare le scadenze del flusso di lavoro dalla bozza generata in precedenza. La generazione della bozza non riesce se queste scadenze sono passate. Per ovviare a questo problema, puoi impostare le scadenze del flusso di lavoro sulla versione precedente in futuro o generare una nuova versione di bozza. Se si genera una nuova versione, utilizzare **Altro > Nuova versione > Bozza** e selezionare **Scadenze del flusso di lavoro future**.

* Quando si esegue la verifica dei file PDF, i motivi degli errori di generazione della bozza includono:

   * I font e le immagini sono collegati da fonti esterne (ad esempio dal file system locale)

     Per poter essere visualizzati su un altro computer o in Workfront Proof, i tipi di carattere e le immagini devono essere incorporati nel file PDF.

   * Il file PDF contiene livelli vuoti o campi trasparenti o sovrapposti.

     Se non siete in grado di determinare quale livello o oggetto causa questo problema, esportate la progettazione o il documento come PDF ottimizzato (rimuovendo tutti gli elementi indesiderati).


---
product-area: documents
navigation-topic: proofing-overview
title: Panoramica delle bozze dei contenuti interattivi
description: Il contenuto interattivo fornisce diversi metodi per coinvolgere i visualizzatori. Le agenzie possono misurare il successo delle loro campagne utilizzando le analisi raccolte dalle risposte a questo contenuto.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Panoramica delle bozze dei contenuti interattivi

<!-- Audited: 01/2024 -->

Il contenuto interattivo fornisce diversi metodi per coinvolgere i visualizzatori. Le agenzie possono misurare il successo delle loro campagne utilizzando le analisi raccolte dalle risposte a questo contenuto.

Alcuni esempi di contenuti interattivi:

* Siti Web
* Video incorporati o in streaming
* Banner interattivi
* Animazioni HTML5
* Micrositi
* E-mail interattive

## Informazioni sulla creazione di bozze per contenuti interattivi

Puoi creare una bozza per il contenuto interattivo in uno dei seguenti modi:

* Crea una bozza da un file ZIP contenente il contenuto interattivo.

  Adobe Workfront decomprime il contenuto dal file ZIP e lo memorizza su un server Workfront. Poiché viene memorizzato in questo modo, è possibile fare affidamento sul fatto che il contenuto rimanga invariato durante tutto il ciclo di revisione della bozza.

* Specifica l’URL per il contenuto.

  Questo è il modo più semplice per creare una bozza per i contenuti interattivi. Questo è anche l’unico modo in cui puoi rivedere i contenuti in modo interattivo, poiché gli utenti li sperimentano su Internet.

  Con questo approccio, un server esterno sconosciuto a Workfront memorizza e ospita il contenuto.

  È consigliabile utilizzare questo metodo per i siti Web di grandi dimensioni, in quanto è difficile raccogliere tutti i file che costituiscono un sito Web di grandi dimensioni. Tuttavia, poiché il contenuto della bozza è memorizzato esternamente, Workfront non è in grado di proteggerlo dalle modifiche apportate dagli sviluppatori che vi lavorano, pertanto potresti non essere in grado di fare affidamento sul fatto che il contenuto rimanga invariato durante tutto il ciclo di revisione della bozza.

## Informazioni sulla preparazione di contenuto interattivo in un file ZIP per la verifica

Quando riunisci il contenuto interattivo in un file ZIP per la verifica, assicurati che includa le seguenti specifiche:

* Tutte le risorse, come CSS, JavaScript, video, suoni e immagini devono essere incluse nel file del bundle.
* Il contenuto interattivo deve includere il file principale (index.html, index.htm). Se il file non viene inserito nella posizione principale, lo strumento cerca automaticamente la cartella per trovarlo. Non è necessario che il file principale sia denominato index.html/index.htm, tuttavia nel percorso principale può essere presente un solo file .html/.htm.
* Il file deve contenere almeno una pagina Web con file statico.
* La dimensione massima del bundle è di 500 MB.
* Nel caso di file .zip creati in iOS, lo strumento identifica automaticamente la cartella in cui si trova il contenuto.
* I progetti interattivi sono supportati solo come archivi .zip. L’invio di file .zip standard non riuscirà.
* Il sito web deve essere protetto (HTTPS).

  Questo non è un requisito quando si utilizza il Visualizzatore bozze desktop.

  Per ulteriori informazioni, consulta [Informazioni su Visualizzatore bozze desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Il sito web deve poter essere visualizzato in un iframe.

  Questo non è un requisito quando si utilizza il Visualizzatore bozze desktop.

  Per ulteriori informazioni, consulta [Informazioni su Visualizzatore bozze desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Informazioni sulla creazione di una bozza interattiva

Dopo aver preparato il file del bundle ZIP, crea una bozza interattiva.

Per ulteriori informazioni, consulta [Creare una bozza per il contenuto interattivo in un file ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Oppure, se utilizzi Workfront Proof, consulta la sezione [Generare una bozza per il contenuto interattivo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) nell’articolo [Genera bozze in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Informazioni sulla revisione delle bozze interattive

È consigliabile utilizzare il Visualizzatore bozze desktop autonomo come visualizzatore predefinito per le bozze interattive. Tuttavia, se i criteri dell’organizzazione non consentono l’utilizzo dell’app Visualizzatore bozze desktop, l’amministratore di Workfront può configurare il sistema in modo da poter esaminare il contenuto interattivo, incluso in un file di archivio ZIP, nel Visualizzatore bozze web. Per informazioni comparative sul Visualizzatore bozze desktop e sul Visualizzatore bozze web, vedere [Panoramica sulle differenze tra il visualizzatore bozze web e il visualizzatore bozze desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

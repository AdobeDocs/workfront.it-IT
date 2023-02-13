---
product-area: documents
navigation-topic: proofing-overview
title: Panoramica delle bozze dei contenuti interattivi
description: Il contenuto interattivo fornisce diversi metodi per coinvolgere i visualizzatori. Le agenzie possono misurare il successo delle loro campagne utilizzando le analisi raccolte dalle risposte a questo contenuto.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Panoramica delle bozze dei contenuti interattivi

Il contenuto interattivo fornisce diversi metodi per coinvolgere i visualizzatori. Le agenzie possono misurare il successo delle loro campagne utilizzando le analisi raccolte dalle risposte a questo contenuto.

Esempi di contenuto interattivo includono:

* Siti Web
* Video incorporati o in streaming
* Banner interattivi
* Animazioni HTML5
* Micrositi
* E-mail interattive

Questo articolo fornisce le seguenti informazioni sulla correzione del contenuto interattivo:

## Informazioni sulla creazione di bozze per il contenuto interattivo

Puoi creare una bozza per il contenuto interattivo in uno dei seguenti modi:

* Crea una bozza da un file ZIP contenente il contenuto interattivo.

   Adobe Workfront estrae il contenuto dal file ZIP e lo memorizza su un server Workfront. Poiché è memorizzato in questo modo, puoi contare sul fatto che il contenuto rimanga lo stesso durante tutto il ciclo di revisione della bozza.

* Specifica l’URL per il contenuto.

   Questo è il modo più semplice per creare una bozza per il contenuto interattivo. Questo è anche l’unico modo per rivedere i contenuti in modo interattivo, in quanto gli utenti lo sperimentano su Internet.

   Con questo approccio, un server esterno sconosciuto a Workfront memorizza e ospita il contenuto.

   Raccomandiamo questo metodo per un grande sito web perché è difficile raccogliere tutti i file che compongono un grande sito web. Tuttavia, poiché il contenuto della bozza viene archiviato esternamente, Workfront non può proteggerlo dalle modifiche apportate dagli sviluppatori che vi lavorano, pertanto potresti non essere in grado di fare affidamento sul contenuto che rimane invariato durante tutto il ciclo di revisione della bozza.

## Informazioni sulla preparazione del contenuto interattivo in un file ZIP per la correzione del contenuto

Quando raccogli il contenuto interattivo in un file ZIP a scopo di correzione, accertati che includa le seguenti specifiche:

* Tutte le risorse, come CSS, JavaScript, video, suoni e immagini, devono essere incluse nel file del bundle.
* Il contenuto interattivo deve includere il file principale (index.html, index.htm). Se questo file non viene inserito nella posizione principale, lo strumento cerca automaticamente la cartella per trovarla. Il file principale non deve essere denominato index.html/index.htm, tuttavia, può esserci un solo file .html/.htm posizionato nel percorso principale.
* Il file deve contenere almeno una pagina Web del file statico.
* La dimensione massima del bundle è 500 MB.
* Nel caso di file .zip creati in iOS, lo strumento identifica automaticamente la cartella in cui si trova il contenuto
* I progetti interattivi sono supportati solo come archivi .zip. Gli invii standard di file .zip non riusciranno.
* Il sito web deve essere protetto (HTTPS).

   Questo non è un requisito quando si utilizza il visualizzatore per correzione desktop.

   Per ulteriori informazioni, consulta [Comprendere il visualizzatore di correzione del desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Il sito web deve poter essere visualizzato in un iframe.

   Questo non è un requisito quando si utilizza il visualizzatore per correzione desktop.

   Per ulteriori informazioni, consulta [Comprendere il visualizzatore di correzione del desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Creazione di una bozza interattiva

Dopo aver preparato il file del bundle ZIP, crea una bozza interattiva.

Per ulteriori informazioni, consulta [Creare una bozza per il contenuto interattivo in un file ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Oppure, se utilizzi Workfront Proof, consulta la sezione . [Genera una bozza per il contenuto interattivo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) nell&#39;articolo [Genera bozze in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Informazioni sulla revisione delle bozze interattive

È consigliabile utilizzare il visualizzatore indipendente per la correzione del desktop come visualizzatore predefinito per le bozze interattive. Tuttavia, se i criteri dell’organizzazione non consentono l’utilizzo dell’app Visualizzatore correzione desktop, l’amministratore di Workfront può configurare il sistema in modo da poter rivedere il contenuto interattivo, incluso in un file di archivio ZIP, nel Visualizzatore correzione Web. Per informazioni comparative sul visualizzatore per correzione desktop e sul visualizzatore per correzione Web, vedere [Panoramica sulle differenze tra il visualizzatore per correzione web e il visualizzatore per correzione desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

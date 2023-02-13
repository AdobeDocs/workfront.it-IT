---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Risoluzione dei problemi - [!DNL Workfront Proof] visualizzatore di correzione
description: Se il contenuto della bozza non viene caricato e puoi visualizzare solo un visualizzatore di correzione vuoto, è molto probabile che qualcosa stia bloccando questa azione localmente. Prova le possibili soluzioni riportate di seguito.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Risoluzione dei problemi - [!DNL Workfront Proof] visualizzatore di correzione

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se il contenuto della bozza non viene caricato e puoi visualizzare solo un visualizzatore di correzione vuoto, è molto probabile che qualcosa stia bloccando questa azione localmente. Prova le possibili soluzioni riportate di seguito.

## Assicurati che il browser e [!DNL Flash Player] Le versioni sono aggiornate

Tutti gli sviluppatori lavorano costantemente sulle loro applicazioni e rilasciano regolarmente nuove funzioni e correzioni per i loro prodotti. In questo modo è possibile migliorare l’esperienza utente e mantenere il livello di sicurezza, in modo da utilizzare solo le versioni più recenti. In questo modo si evitano i conflitti tra le applicazioni.

### [!DNL Flash Player] Versione plugin

Per controllare la corrente [!DNL Flash Player] visita la [[!DNL Adobe] sito web](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

Se il numero di versione è diverso da quello elencato per la piattaforma, passa alla [[!DNL Flash Player] pagina di download](http://get.adobe.com/flashplayer/otherversions/) e ottieni la versione più recente.

Nota: si consiglia di utilizzare l&#39;originale [!DNL Adobe] quindi, se il browser utilizza una soluzione incorporata, disattivala e installa il [!DNL Adobe] soluzione.

### Versione browser

Al giorno d&#39;oggi la maggior parte dei browser si aggiorna automaticamente, ma se si verificano problemi vale la pena controllare quale versione si sta utilizzando ed eseguire l&#39;aggiornamento, se necessario.

Nel browser vai a [!UICONTROL Menu] e individua le [!UICONTROL Informazioni] (in alcuni casi può essere visibile in [!UICONTROL Aiuto] menu). In [!UICONTROL Informazioni] pop-up troverai informazioni sulla versione corrente del browser e anche un&#39;opzione per aggiornare/controllare gli aggiornamenti.

Vedi in Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

Una volta che il tuo [!DNL Flash Player] il plug-in e la versione del browser installati tentano di riaprire la bozza e scopri se il problema è risolto.

## Assicurati che il tuo locale [!DNL Flash] Archiviazione disponibile

Nostro [!DNL Workfront Proof] Il visualizzatore si basa sul Flash e vengono memorizzati alcuni dati sulle bozze (ad esempio, commenti, riquadri di prova, [!DNL Workfront Proof] Impostazioni visualizzatore) sul computer utilizzando [!DNL Flash Player]. Se la [!DNL Workfront Proof] Il visualizzatore si apre, ma non è presente alcun contenuto al suo interno, per essere sicuri che l’archiviazione Flash sia disponibile sul computer e che [!DNL Workfront Proof] è autorizzato a utilizzarlo.

Se è stato allocato spazio di archiviazione, ma si sta lavorando con le bozze più grandi con più pagine e commenti cercando di aumentare il [!DNL Flash] Archiviazione e ricarica della bozza.

Consulta la nostra [Problemi Di Visualizzazione Delle Prove - [!DNL Flash] Spiegazione di oggetti condivisi](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) per le istruzioni dettagliate.

## Identificare la posizione del problema

* Le bozze si aprono in un browser diverso?
* Se utilizzi un browser ogni giorno e hai problemi a visualizzare le bozze, prova ad aprire la stessa bozza in un browser diverso sul tuo computer. A questo scopo, copia semplicemente il collegamento della bozza dalla barra dell’URL del browser principale e incollalo in un altro browser. Se la bozza si apre qui, controlla la configurazione del browser principale, i plug-in e le estensioni in quanto questi potrebbero interferire.
* Non disponiamo di alcun browser preferibile, ma se riscontri problemi di prestazioni nel browser corrente consigliamo di passare a uno diverso.
* Le bozze si aprono su un altro computer nella tua posizione?
Se la bozza non viene aperta in alcun browser del computer, provare ad aprirla in un computer diverso nel percorso e/o all&#39;esterno del sito. Questo ti consente di determinare se un problema è dovuto a una particolare macchina o se si tratta di un problema presente nella tua rete locale.
Se il livello di sicurezza è superiore, le connessioni a [!DNL Workfront Proof] può essere bloccato da:

   * Software AV locale
   * La tua soluzione di sicurezza di rete
   * Configurazione di DNS, firewall o proxy
   * Queste sono le impostazioni che sono fuori dal nostro controllo. Sono disponibili diverse soluzioni di sicurezza e non siamo in grado di sapere quali sono implementate nella rete e quali potrebbero bloccare le connessioni a [!DNL Workfront Proof]. Inoltre, non è possibile [!DNL Workfront Proof] per decidere la configurazione di sicurezza interna. In caso di problemi con l&#39;apertura delle bozze sui più computer della posizione/rete, consigliamo di contattare il team IT per verificare le impostazioni di rete e autorizzare o aggiungere il [!DNL Workfront Proof] all&#39;inserire nell&#39;elenco Consentiti, se necessario.

* Sono le connessioni a [!DNL Workfront Proof] consentito nella rete?
All’interno del Visualizzatore di prove carichiamo le tessere - frammenti delle pagine. Se il contenuto non viene caricato correttamente alla fine, è possibile che alcune connessioni a [!DNL Workfront Proof] sono bloccati nella rete. Assicurati che tutte le connessioni e tutti i contenuti da *.proofhq.com siano aggiunti all&#39;inserire nell&#39;elenco Consentiti. Il team IT deve essere in grado di contribuire alla verifica di questo problema.

## Rivedi plug-in

Se il browser e [!DNL Flash Player] il plug-in è aggiornato e la rete non blocca le connessioni a [!DNL Workfront Proof] nel browser potrebbe esserci qualcosa che influisce sulla visualizzazione delle bozze. Al giorno d&#39;oggi ci sono più plug-in ed estensioni disponibili nel tuo browser e alcuni di loro interferiscono o sono in conflitto con gli altri.

La best practice consiste nel rimuovere tutti i componenti aggiuntivi sconosciuti e mantenere solo quelli utilizzati e considerati attendibili. Ogni browser dovrebbe fornire opzioni per controllare/modificare/eliminare i plug-in e le estensioni. Nostro [!DNL Workfront Proof] Il visualizzatore si basa su [!DNL Flash] e utilizziamo JavaScript per caricare il visualizzatore in modo che tu voglia rivedere in modo particolare i plug-in che potrebbero influenzare questi.

Visita le pagine elencate di seguito per istruzioni più dettagliate dagli sviluppatori su come disabilitare i componenti aggiuntivi del browser:

* Chrome: [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB) / [estensioni](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [componenti aggiuntivi](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [componenti aggiuntivi](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [componenti aggiuntivi](http://support.apple.com/en-gb/HT203353)

Se c&#39;è un particolare componente aggiuntivo che interferisce con il caricamento delle bozze, puoi provare a controllare i dettagli nella console del browser.

![ProofView_4.png](assets/proofview-4-350x57.png)

Nella maggior parte dei browser più recenti sono disponibili alcuni strumenti per sviluppatori aggiuntivi che possono essere utilizzati per la risoluzione dei problemi più avanzata.

In caso di problemi nella visualizzazione delle bozze:

* Apri la console del browser e ricarica la bozza.
* Controlla se ci sono avvisi o messaggi nella console. Questi dettagli possono aiutare a identificare la causa principale dei problemi.
* Chiedi al tuo team IT di analizzare i risultati. Dovrebbero essere in grado di consigliare e aiutare a risolvere il problema locale.
* Condividi i risultati con il nostro [Team di supporto](https://support.workfront.com/hc/en-us/requests/new). Saremo felici di aiutare.

Se non sai come aprire la console nel browser, vedi i passaggi registrati:

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

Puoi anche consultare la documentazione dello sviluppatore del browser per istruzioni più dettagliate.

## Controllare le impostazioni dei contenuti misti

Tutte le connessioni a [!DNL Workfront Proof] sono su HTTPS. Tuttavia, nella [!DNL Workfront Proof] Il visualizzatore carica i riquadri su HTTP e i dati sono protetti con i token. Questo crea contenuti misti che alcuni browser o soluzioni di sicurezza potrebbero bloccare (per impostazione predefinita o secondo la configurazione manuale).

Se questo è il motivo per cui le bozze non si aprono sul tuo computer (dovresti essere in grado di vedere gli avvisi pertinenti nella console del browser) autorizzare tali connessioni per [!DNL Workfront Proof] o modificare le impostazioni per consentire il contenuto misto passivo sulla macchina. I contenuti misti possono essere bloccati dal tuo browser, software AV, configurazione di rete, ecc - per determinare la causa esatta contattare il tuo team IT/amministratori di rete. Devono anche essere in grado di aiutare ad abilitare il contenuto misto sul computer.

Contatta il nostro [Team di supporto](https://support.workfront.com/hc/en-us/requests/new) se hai bisogno di assistenza da parte nostra.

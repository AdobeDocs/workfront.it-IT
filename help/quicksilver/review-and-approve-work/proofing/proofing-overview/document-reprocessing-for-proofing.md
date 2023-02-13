---
product-area: documents
navigation-topic: proofing-overview
title: Panoramica sulla rielaborazione dei documenti per la correzione
description: Quando si invia un documento (DOCX, PDF, XLSX, AI) per la correzione, Adobe Workfront lo rielabora in modo che possa essere visualizzato nel visualizzatore di correzione senza l’applicazione software utilizzata per crearlo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Panoramica sulla rielaborazione dei documenti per la correzione

Quando si invia un documento (DOCX, PDF, XLSX, AI) per la correzione, Adobe Workfront lo rielabora in modo che possa essere visualizzato nel visualizzatore di correzione senza l’applicazione software utilizzata per crearlo. 

Ogni pagina del documento viene visualizzata nel visualizzatore di correzione come immagine miniatura. Quando si fa clic su una miniatura, è possibile eseguire lo zoom in una versione bitmap della pagina al 100%, 200% e 400%. Per le prove di altezza o larghezza superiori a 800 mm, lo zoom massimo è del 200%.

I colori nel documento vengono visualizzati in sRGB con conversione dei colori dall&#39;ultima libreria di Adobi. Il visualizzatore di correzione supporta qualsiasi profilo ICC (International Color Consortium) incorporato nel documento.

Tutto il testo del font viene estratto nel relativo livello purché durante il caricamento del documento nel sistema sia inclusa l’estensione corretta del file. Il testo incluso come immagini o curve non viene visualizzato.

>[!NOTE]
>
>Workfront supporta attualmente documenti contenenti fino a 2000 pagine. Questo include le bozze combinate. Per ulteriori informazioni, consulta [Creare una bozza a più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Suggerimenti generali

* Poiché i file PDF sono i più standardizzati e affidabili, è consigliabile convertire i documenti in questo formato prima di caricarli.
* Utilizzare la versione più recente del software per creare i documenti originali.
* Se non si è sicuri delle impostazioni da utilizzare per salvare o esportare i documenti nell&#39;applicazione in cui sono stati creati, utilizzare le impostazioni predefinite. 
* Assicurarsi di incorporare tutti i font utilizzati in un documento al suo interno. Se si utilizzano font personalizzati, tali font verranno visualizzati nel documento solo sui computer in cui sono installati.
* Se possibile, posizionate tutti gli elementi di testo nei livelli superiori della progettazione. Questo dovrebbe garantire che il testo sia estratto e selezionabile nello strumento di annotazione testo.
* Posizionare al suo interno tutte le immagini e gli elementi del documento. Se le colleghi dalle sorgenti esterne, ad esempio un altro file sul computer, non verranno visualizzate nella bozza creata.
* Crea il documento utilizzando gli standard consigliati per il suo tipo e ottimizzalo prima di caricarlo. In questo modo il documento verrà aperto correttamente nel visualizzatore di correzione e in tutte le altre applicazioni e piattaforme.
* Nel software di progettazione, prova ad eseguire le opzioni di &quot;verifica preliminare&quot; per vedere se il documento genera avvisi. Queste opzioni sono disponibili nella maggior parte delle applicazioni come anteprima di output, produzione di stampa e così via. Per ulteriori informazioni, consulta la documentazione dell’applicazione.
* Assicurati che le impostazioni del colore siano coerenti in tutto il documento.
* Se il documento è protetto da azioni quali la copia dei file, lo strumento di estrazione della correzione potrebbe non essere in grado di accedere al relativo contenuto.

## Tempi di elaborazione

Normalmente, l&#39;elaborazione richiede alcuni secondi per pagina. Tuttavia, diversi fattori possono prolungare questo processo, come il traffico/larghezza di banda della rete, la velocità di connessione locale e la velocità di connessione internazionale (per gli utenti al di fuori degli Stati Uniti). Possono inoltre influire sui tempi di elaborazione:

* Per documenti e immagini statici: conteggio delle pagine, dimensioni della pagina, volume del testo, complessità delle immagini e degli oggetti (elementi come più elementi vettoriali, livelli, trasparenza).
* Per i video: durate lunghe, dimensioni grandi e codec utilizzati.
* Per le acquisizioni web: tempi di caricamento della pagina web e dimensioni della pagina.

## Passaggi del processo

I file inviati passano attraverso alcuni o tutti i seguenti passaggi:

1. **Invio**. Quando carichi un documento nel sistema, lo fai utilizzando la pagina Nuova bozza o un’interfaccia API (Application Programming Interface). 
1. **Coda**. Durante i periodi di traffico pesante, Workfront potrebbe dover mettere in coda gli invii per evitare di sovraccaricare il sistema. La maggior parte delle bozze passa solo pochi secondi in una coda. 
1. **Elaborazione in corso.** I file raggiungono i computer di elaborazione in base al tipo di contenuto. Usiamo diversi strumenti per elaborare bozze video, immagini web, immagini statiche e documenti. I contenitori Rich Media (ZIP) e gli invii di acquisizione web interattivi non richiedono elaborazione.

---
product-area: documents
navigation-topic: proofing-overview
title: Panoramica sulla rielaborazione dei documenti per la verifica
description: Quando si invia un documento (DOCX, PDF, XLSX, AI) per la verifica, Adobe Workfront lo rielabora in modo che possa essere visualizzato nel visualizzatore di prove senza l'applicazione software utilizzata per la creazione.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Panoramica sulla rielaborazione dei documenti per la verifica

Quando si invia un documento (DOCX, PDF, XLSX, AI) per la verifica, Adobe Workfront lo rielabora in modo che possa essere visualizzato nel visualizzatore di prove senza l&#39;applicazione software utilizzata per la creazione. 

Ogni pagina del documento viene visualizzata nel visualizzatore di bozze come miniatura. Quando si fa clic su una miniatura, è possibile eseguire lo zoom di una versione bitmap della pagina al 100%, 200% e 400%. Per bozze che superano gli 800 mm in altezza o larghezza, il livello di zoom massimo è 200%.

I colori del documento vengono visualizzati in sRGB con la conversione dei colori dalla libreria di Adobi più recente. Il visualizzatore di bozze supporta qualsiasi profilo International Color Consortium (ICC) incorporato nel documento.

Tutto il testo del font viene estratto nel relativo livello, a condizione di includere la corretta estensione del file durante il caricamento del documento nel sistema. Il testo incluso come immagini o curve non viene visualizzato.

>[!NOTE]
>
>Workfront attualmente supporta documenti contenenti fino a 2000 pagine. Sono incluse le bozze combinate. Per ulteriori informazioni, consulta [Creare una bozza con più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Suggerimenti generali

* Poiché i file PDF sono i più standardizzati e affidabili, si consiglia di convertire i documenti in questo formato prima di caricarli.
* Utilizzare la versione più recente del software per creare i documenti originali.
* Se non si è certi delle impostazioni da utilizzare per il salvataggio o l&#39;esportazione dei documenti nell&#39;applicazione in cui sono stati creati, utilizzare le impostazioni predefinite. 
* Assicurarsi di incorporare tutti i tipi di carattere utilizzati in un documento al suo interno. Se si utilizzano tipi di carattere personalizzati, tali tipi di carattere verranno visualizzati solo nei computer in cui sono installati. Tuttavia, poiché i caratteri personalizzati non sono inclusi nel sistema di bozze, non è possibile utilizzarli durante la generazione del file, anche quando è incorporato.
* Se possibile, posizionate tutti gli elementi di testo nei livelli superiori del progetto. In questo modo il testo verrà estratto e sarà possibile selezionarlo nello strumento di annotazione Testo.
* Inserire tutte le immagini e gli elementi del documento al suo interno. Se li colleghi da fonti esterne, ad esempio un altro file sul computer, la bozza creata non verrà visualizzata.
* Crea il documento utilizzando gli standard consigliati per il relativo tipo e ottimizzalo prima di caricarlo. In questo modo il documento verrà aperto correttamente nel visualizzatore di bozze e in tutte le altre applicazioni e piattaforme.
* Nel software di progettazione provare a eseguire le opzioni di verifica preliminare per verificare se il documento genera avvisi. Queste opzioni sono disponibili nella maggior parte delle applicazioni, come l&#39;anteprima di output, la stampa e così via. Per ulteriori informazioni, consulta la documentazione dell’applicazione.
* Verificare che le impostazioni dei colori siano coerenti in tutto il documento.
* Se il documento è protetto da azioni quali la copia dei file, è possibile che lo strumento di estrazione degli elementi di correzione non sia in grado di accedere al contenuto.

## Tempi di elaborazione

In genere, l’elaborazione richiede alcuni secondi per pagina. Tuttavia, questo può essere prolungato da vari fattori, come il traffico di rete/larghezza di banda, la velocità di connessione locale e la velocità di connessione internazionale (per gli utenti al di fuori degli Stati Uniti). I seguenti elementi possono influire anche sul tempo di elaborazione:

* Per documenti e immagini statici: conteggio delle pagine, dimensioni della pagina, volume del testo, complessità delle immagini e degli oggetti (elementi come più elementi vettoriali, livelli, lucidi).
* Per i video: lunga durata, grandi dimensioni e codec utilizzati.
* Per le web clip: tempi di caricamento delle pagine web e dimensioni della pagina.

## Passaggi del processo

I file inviati seguono alcuni o tutti i passaggi seguenti:

1. **Invio**. Quando carichi un documento nel sistema, lo fai utilizzando la pagina New proof (Nuova bozza) o un’interfaccia API (Application Programming Interface). 
1. **Coda**. Durante i periodi di traffico intenso, Workfront potrebbe dover mettere in coda gli invii per evitare di sovraccaricare il sistema. La maggior parte delle bozze passa solo pochi secondi in coda. 
1. **Elaborazione.** I file raggiungono le macchine di elaborazione in base al tipo di contenuto. Usiamo diversi strumenti per elaborare bozze video, acquisizioni web, immagini statiche e documenti. I contenitori per contenuti multimediali avanzati (ZIP) e gli invii di acquisizione web interattiva non richiedono l’elaborazione.

---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Creare una bozza statica del sito web utilizzando [!DNL Workfront Proof]
description: Puoi creare bozze statiche dalle pagine web. Inoltre, è possibile simulare vari dispositivi definendo la risoluzione dello schermo delle immagini.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Creare una bozza statica del sito web utilizzando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Puoi creare bozze statiche dalle pagine web. Inoltre, è possibile simulare vari dispositivi definendo la risoluzione dello schermo delle immagini.

## Creazione di una bozza statica del sito web

1. Apri [!UICONTROL Nuova prova] come descritto in [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Incolla o digita l’URL nel **www.shareyourlink.com** scatola.
1. Puoi ripetere questo passaggio per aggiungere più URL.
1. Sotto questa casella, fai clic sulla risoluzione (il valore predefinito è 1366x768), quindi seleziona le risoluzioni desiderate nel **[!UICONTROL Risoluzione dello schermo]** scatola.
Seleziona una risoluzione più piccola se desideri provare le progettazioni per i dispositivi mobili. In genere, le progettazioni vengono caricate in base alla risoluzione dello schermo/della finestra del browser.

1. Fai clic su **[!UICONTROL Cercare pagine secondarie]** se desideri includere pagine connesse che si trovano nello stesso dominio/sottodominio dell’URL immesso.
   [!DNL Workfront Proof] analizza le pagine collegate e le elenca sotto la sezione **[!UICONTROL Cercare pagine secondarie]** opzione . Puoi selezionare le pagine da includere.

1. Con la [!UICONTROL Combinare bozze] è possibile inviare tutte le pagine web come una singola bozza a più pagine.
1. Fai clic su **[!UICONTROL Fine]**, quindi completa la configurazione della bozza come spiegato in [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Informazioni su pagine e pagine protette da password che richiedono autorizzazione

[!DNL Workfront Proof] impossibile acquisire un sito web protetto da password come bozza statica.

Per creare bozze da pagine che richiedono l’autorizzazione, il team IT deve aggiungere uno dei seguenti URL all’Inserire nell&#39;elenco Consentiti dell’azienda attraverso cui il nostro strumento di acquisizione Web si connette:

**Cluster AWS negli Stati Uniti**: webcapture.proofhq.com

**Cluster GCP negli Stati Uniti**: webcapture.gcp.proofhq.com

**Cluster EMEA**: webcapture.proofhq.eu

>[!NOTE]
>
>Si consiglia di eseguire prove interattive anziché prove statiche per le pagine interne che richiedono autorizzazioni e i siti web protetti da password. Per ulteriori informazioni, consulta [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Informazioni sull’elaborazione delle bozze statiche dei siti web

* Le animazioni, i video incorporati, gli script e le interazioni non possono essere inclusi nelle bozze dei siti web statici. Per verificare il contenuto interattivo, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Le pagine di prova vengono generalmente preparate acquisite alla velocità di circa 20 secondi per pagina. Tuttavia, il tempo complessivo di preparazione dipende anche dai server in cui sono ospitate le pagine. Lo strumento attende 60 secondi per il caricamento di ogni URL inviato. Se questo tempo di attesa viene superato, la prova non riesce.
* Per le bozze combinate, se uno degli URL non risponde allo strumento di acquisizione, la bozza non riesce.
* [!DNL Workfront Proof] acquisisce pagine web fino a 195 pollici dopo la rasterizzazione. Se la pagina web è più lunga di questa, la bozza non riesce.
* L’estrazione del testo è disponibile su tutti gli elementi di testo, ma il testo inserito come immagini non viene estratto.
* I collegamenti ipertestuali sono selezionabili nelle bozze e le pagine collegate si aprono nelle nuove schede del browser.
* I collegamenti ipertestuali sulle immagini non possono essere cliccati se gli elementi style=&quot;display:block&quot; sono utilizzati all’interno della `<a>` tag. È consigliabile regolare queste parti della progettazione della pagina.
* Per ottenere i migliori risultati, consigliamo di creare le pagine utilizzando le best practice di codifica e gli standard riconosciuti.

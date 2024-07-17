---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Crea bozza sito Web statico utilizzando  [!DNL Workfront Proof]
description: Puoi creare bozze statiche dalle pagine web. Inoltre, è possibile simulare vari dispositivi definendo la risoluzione dello schermo delle clip.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Creare una bozza statica del sito Web utilizzando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Puoi creare bozze statiche dalle pagine web. Inoltre, è possibile simulare vari dispositivi definendo la risoluzione dello schermo delle clip.

## Creazione di una bozza statica di un sito web

1. Aprire la pagina [!UICONTROL Nuova bozza], come descritto in [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Incolla o digita l&#39;URL nella casella **www.shareyourlink.com**.
1. Puoi ripetere questo passaggio per aggiungere più URL.
1. Fai clic sulla risoluzione (il valore predefinito è 1366x768) nella casella **[!UICONTROL Risoluzione schermo]**, quindi seleziona le risoluzioni desiderate.
Seleziona una risoluzione inferiore se desideri verificare le progettazioni per i dispositivi mobili. In genere, le progettazioni vengono caricate in base alla risoluzione dello schermo o della finestra del browser.

1. Fare clic su **[!UICONTROL Cerca pagine secondarie]** se si desidera includere pagine connesse che si trovano nello stesso dominio/sottodominio dell&#39;URL immesso.
   [!DNL Workfront Proof] analizza le pagine collegate e le elenca sotto l&#39;opzione **[!UICONTROL Cerca pagine secondarie]**. Puoi selezionare le pagine da includere.

1. Con la funzionalità [!UICONTROL Combina bozze] è possibile inviare tutte le pagine Web come una bozza multipagina singola.
1. Fai clic su **[!UICONTROL Fine]**, quindi completa la configurazione della bozza come descritto in [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Informazioni sulle pagine protette da password e sulle pagine che richiedono l’autorizzazione

[!DNL Workfront Proof] non è in grado di acquisire come bozza statica un sito Web protetto da password.

Per creare bozze da pagine che richiedono un’autorizzazione, il team IT deve aggiungere uno dei seguenti URL al Inserisco nell&#39;elenco Consentiti di acquisizione dei dati dell’azienda tramite il quale si connette il nostro strumento di acquisizione web:

**Cluster AWS negli Stati Uniti**: webcapture.proofhq.com

**Cluster GCP negli Stati Uniti**: webcapture.gcp.proofhq.com

**Cluster EMEA**: webcapture.probhq.eu

>[!NOTE]
>
>Consigliamo di eseguire prove interattive anziché statiche per le pagine interne che richiedono autorizzazioni e siti web protetti da password. Per ulteriori informazioni, vedere [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Informazioni sull’elaborazione di bozze statiche per siti web

* Animazioni, video incorporati, script e interazioni non possono essere inclusi nelle bozze statiche del sito web. Per verificare il contenuto interattivo, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Le pagine delle bozze vengono generalmente preparate e acquisite alla velocità di circa 20 secondi per pagina. Tuttavia, il tempo di preparazione complessivo dipende anche dai server in cui sono ospitate le pagine. Lo strumento attende 60 secondi per ogni URL inviato da caricare. Se questo tempo di attesa viene superato, la bozza non riesce.
* Per le bozze combinate, se uno degli URL non risponde allo strumento di acquisizione, la bozza non riesce.
* [!DNL Workfront Proof] acquisisce le pagine Web fino a 195 pollici dopo la rasterizzazione. Se la pagina web è più lunga di questa, la bozza non riesce.
* L’estrazione del testo è disponibile su tutti gli elementi di testo, ma il testo inserito come immagine non viene estratto.
* È possibile fare clic sui collegamenti ipertestuali nelle bozze e aprire le pagine collegate nelle nuove schede del browser.
* I collegamenti ipertestuali sulle immagini non sono cliccabili se gli elementi style=&quot;display:block&quot; sono utilizzati all&#39;interno dei tag `<a>`. È consigliabile regolare queste parti della progettazione della pagina.
* Per ottenere risultati ottimali, consigliamo di creare le pagine utilizzando le best practice di codifica e gli standard riconosciuti.

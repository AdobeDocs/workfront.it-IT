---
product-area: documents
navigation-topic: proofing-overview
title: Rivedi il contenuto interattivo nell’estensione del visualizzatore di bozze web
description: Lo strumento di revisione Adobe Workfront è un’estensione del browser che consente di verificare il contenuto interattivo in un file ZIP o con un URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 5a8bfdeae7f5d23ecf835e652cf0ff5efd5aa410
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 1%

---

# Rivedere i contenuti interattivi con lo strumento di revisione Adobe Workfront

<span class="preview">Lo strumento Adobe Workfront Review è stato reso disponibile il 7 novembre 2024. Questa estensione è attualmente in versione beta.</span>

Lo strumento di revisione Adobe Workfront è un’estensione del browser basata sul web che consente di verificare il contenuto interattivo in un file ZIP o con un URL. Lo strumento di revisione di Adobe Workfront è disponibile nei seguenti browser:

* Firefox
* Chrome
* Edge
* Safari

>[!IMPORTANT]
>
>Questa estensione è necessaria per rivedere il contenuto in GenStudio for Performance Marketing e Creative Cloud Express. Assets si aprirà automaticamente nel visualizzatore web. Non è necessario aggiornare le impostazioni dell&#39;account.


## Installare l’estensione

### Prerequisiti

* Per utilizzare lo strumento Adobe Workfront Review, è necessario rimuovere l’estensione Legacy Web Viewer.

### Installare l’estensione

I revisori e gli approvatori devono installare lo strumento di revisione Adobe Workfront. in uno dei seguenti browser:

* [Estensione Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Estensione Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


Affinché le bozze interattive possano essere aperte automaticamente nello strumento di revisione di Adobe Workfront, un amministratore di Workfront deve aggiornare le impostazioni di bozza in Workfront come descritto nelle sezioni seguenti.

## Aggiorna i valori predefiniti di verifica di Workfront

Per utilizzare lo strumento di revisione di Workfront come visualizzatore predefinito per il contenuto interattivo, è necessario aggiornare le impostazioni predefinite di verifica in Workfront.

>[!NOTE]
>
>È consigliabile utilizzare il Visualizzatore bozze desktop se il contenuto da esaminare si trova su un sito Web che
>
>* Richiede autenticazione SSO
>* Impedisce l&#39;apertura del sito in iFrame, ad esempio Figma

### Imposta lo strumento di revisione Adobe Workfront come visualizzatore predefinito per le bozze URL e ZIP

Per utilizzare lo strumento di revisione web per le bozze URL e ZIP, un amministratore di Workfront deve regolare l’impostazione predefinita per le bozze interattive.

1. Nel menu principale di Workfront, fare clic su **Strumenti di correzione**.
1. Fai clic su **Impostazioni account**, quindi sulla scheda **Impostazioni**.
1. Nella sezione **Proof Defaults** (Impostazioni predefinite bozza), individua **Desktop Proofing Viewer for Interactive proofing** e fai clic su **Setup**.
1. Scegliere **Disabilitato** dal menu a discesa. Le bozze interattive create da un file URL o ZIP ora si aprono automaticamente nello strumento Adobe Workfront Review, un browser basato su web.
1. Fai clic su **Salva**.

>[!NOTE]
>
>Questa modifica si applica a tutte le bozze interattive nell’istanza Workfront. È consigliabile testare la nuova esperienza nell’ambiente di anteprima prima di abilitarla in produzione. È possibile tornare facilmente al Visualizzatore desktop modificando l&#39;impostazione dell&#39;account **Visualizzatore bozze desktop per bozze interattive** su **Abilitato per tutte le bozze interattive**.

### Imposta lo strumento di revisione Adobe Workfront come visualizzatore predefinito solo per le bozze ZIP

Per utilizzare lo strumento di revisione web solo per le bozze ZIP, un amministratore di Workfront deve regolare l’impostazione predefinita per le bozze interattive.

1. Nel menu principale di Workfront, fare clic su **Strumenti di correzione**.
1. Fai clic su **Impostazioni account**, quindi sulla scheda **Impostazioni**.
1. Nella sezione **Proof Defaults** (Impostazioni predefinite bozza), individua **Desktop Proofing Viewer for Interactive proofing** e fai clic su **Setup**.
1. Nel menu a discesa scegliere **Abilitato solo per le bozze interattive create da un URL**. Le bozze interattive create da un file ZIP ora si aprono automaticamente nello strumento Adobe Workfront Review, un browser basato su web. Le bozze interattive create da un URL sono ancora aperte nel Visualizzatore bozze desktop.
1. Fai clic su **Salva**.

>[!NOTE]
>
>Questa modifica si applica a tutte le bozze ZIP nella tua istanza Workfront. È consigliabile testare la nuova esperienza nell’ambiente di anteprima prima di abilitarla in produzione. È possibile tornare facilmente al Visualizzatore desktop modificando l&#39;impostazione dell&#39;account **Visualizzatore bozze desktop per bozze interattive** su **Abilitato per tutte le bozze interattive**.


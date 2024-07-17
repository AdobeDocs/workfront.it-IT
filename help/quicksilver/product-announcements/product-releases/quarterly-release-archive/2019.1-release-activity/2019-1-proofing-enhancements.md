---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Miglioramenti alla bozza 2019.1
description: Questa pagina descrive tutti i miglioramenti relativi alle prove inclusi nella versione 2019.1. Questa funzionalità è ora disponibile nell’ambiente di produzione.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Miglioramenti alla bozza 2019.1

Questa pagina descrive tutti i miglioramenti relativi alle prove inclusi nella versione 2019.1. Questa funzionalità è ora disponibile nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2019.1, consulta [Panoramica delle attività sulla versione 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Per gli amministratori

* [Configurare il ruolo di bozza predefinito per i non destinatari che aprono una bozza](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Per tutti gli utenti

* [Contenuto interattivo bozza nel visualizzatore bozze Web](#proof-interactive-content-in-the-web-proofing-viewer)
* [L&#39;ordinamento predefinito per i commenti nel visualizzatore bozze è ora dal meno recente al più recente](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Revisione avanzata per commenti nel visualizzatore bozze associato a un intervallo di video](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Collegamento a dettagli documento da una notifica bozza o dal visualizzatore bozze](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Modifica le notifiche e-mail nel visualizzatore bozze](#change-your-email-notifications-in-the-proofing-viewer)
* [Modificare il colore di sfondo nel Visualizzatore bozze desktop](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Cancellare i dati del browser memorizzati nella cache da una bozza in Desktop Proofing Viewer](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Configurare il ruolo di bozza predefinito per i non destinatari che aprono una bozza {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Gli amministratori di Workfront ora possono configurare il ruolo di bozza predefinito per gli utenti che non sono destinatari designati nel flusso di lavoro della bozza, ma che hanno accesso alla bozza tramite il relativo oggetto Workfront (ad esempio progetto, attività o problema).

In precedenza, quando utenti e ospiti avevano accesso a una bozza senza essere aggiunti al flusso di lavoro, il loro ruolo di bozza predefinito era Revisore.

Questa funzionalità si applica solo alle bozze create in Workfront, non in Workfront Proof.

## Contenuto interattivo bozza nel visualizzatore bozze web {#proof-interactive-content-in-the-web-proofing-viewer}

Se i criteri di sicurezza dell&#39;organizzazione non consentono l&#39;utilizzo dell&#39;app per il visualizzatore di bozze desktop autonomo, l&#39;amministratore di Workfront può ora abilitare il contenuto interattivo nel visualizzatore di bozze Web. Prima di creare la bozza, il contenuto deve essere incluso in un file ZIP.

Per ulteriori informazioni, consulta l’articolo .

VIDEO

## L&#39;ordinamento predefinito per i commenti nel visualizzatore bozze è ora dal meno recente al più recente  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

In Proofing Viewer (Visualizzatore di bozze), l’ordine predefinito per i commenti su una bozza è ora Dal meno recente al più recente, come in una conversazione verbale.

In precedenza, l’ordinamento predefinito era Dal più recente al meno recente.

Puoi selezionare un’opzione di ordinamento diversa, che verrà memorizzata per tutte le altre bozze aperte.

Per ulteriori informazioni, consulta la sezione nell’articolo .

## Revisione migliorata per i commenti nel visualizzatore bozze associato a una serie di video {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Durante la revisione di un commento associato a un intervallo di metraggio video nel Visualizzatore bozze, potete ora fare clic su Riproduci per visualizzare l&#39;intero intervallo di metraggio. La riproduzione si interrompe quando raggiunge la fine dell’intervallo. Il commento rimane aperto in modo da non perdere traccia di dove sei.

In precedenza, quando si apriva un commento per un intervallo di metraggio video, era necessario trovare l&#39;inizio dell&#39;intervallo manualmente osservando i numeri dei fotogrammi visualizzati sul commento prima di fare clic su Riproduci. In caso contrario, Proofing Viewer (Visualizzatore di bozze) ha iniziato la riproduzione ovunque si fosse fatto clic l’ultima volta nella timeline del video e non si è fermato alla fine dell’intervallo. Inoltre, il commento è stato compresso quando si è fatto clic su Riproduci, quindi non era più chiaro quale commento si stava esaminando.

Per informazioni sulla revisione delle bozze video, consulta .

VIDEO

## Collegamento ai dettagli del documento da una notifica di bozza o dal visualizzatore bozze {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Quando ricevi un’e-mail che ti invita a rivedere una bozza o stai esaminando una bozza nel Proofing Viewer (Visualizzatore di bozze), ora puoi accedere rapidamente alla pagina dei dettagli del documento per la bozza. In questa pagina è possibile visualizzare l’oggetto Workfront (ad esempio un’attività, un progetto o un problema) associato alla bozza. Questo fornisce un contesto che consente di comprendere il lavoro da eseguire sulla bozza.

Questa funzionalità può essere utilizzata solo per i nuovi utenti aggiunti al sistema. Questo problema è temporaneo.

Per ulteriori informazioni, consulta l’articolo .

VIDEO

## Modificare le notifiche e-mail nel visualizzatore bozze {#change-your-email-notifications-in-the-proofing-viewer}

Ora tutti i revisori di bozze possono specificare quali notifiche di bozze desiderano ricevere per una bozza. Ciò è particolarmente importante quando si collabora con soggetti esterni.

In precedenza, solo il proprietario della bozza o il gestore del traffico poteva configurare gli avvisi e-mail di una bozza per i revisori aggiunti alla bozza. I collaboratori esterni non sono stati in grado di controllare gli avvisi e-mail ricevuti sulla bozza perché non disponevano dell’accesso richiesto a Workfront né del livello di autorizzazione appropriato.

Queste impostazioni sono separate dalle impostazioni degli avvisi e-mail che puoi configurare in Workfront.

Per ulteriori informazioni, consulta [Gestire le notifiche per i commenti e le decisioni relative alle bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDEO

## Modificare il colore di sfondo nel Visualizzatore bozze desktop {#change-the-background-color-in-the-desktop-proofing-viewer}

Ora è possibile modificare il colore di sfondo del Visualizzatore bozze desktop dal colore quasi nero predefinito al bianco. In questo modo è più facile visualizzare i contenuti di verifica con uno sfondo trasparente.

Per ulteriori informazioni, vedere [Configurare le impostazioni del visualizzatore di verifica](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

## Cancellare i dati del browser memorizzati nella cache da una bozza in Desktop Proofing Viewer {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Quando il cookie e le impostazioni della cache del browser sono impostati per bloccare contenuti come i popup, questo comportamento di blocco può verificarsi anche nel Visualizzatore bozze desktop, rendendo impossibile per i revisori visualizzare e commentare il contenuto pop-up nella bozza.

Ora è possibile cancellare i dati della cache del browser che possono essere salvati con una bozza in modo che tutto il contenuto venga visualizzato nel Visualizzatore bozze desktop e che i revisori possano visualizzarlo e commentare.

Per ulteriori informazioni, vedere [Configurare le impostazioni del visualizzatore di verifica](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

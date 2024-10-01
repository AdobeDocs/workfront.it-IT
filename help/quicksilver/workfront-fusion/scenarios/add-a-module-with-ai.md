---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generare un segmento di scenario utilizzando IA
description: È possibile immettere un prompt di testo per creare un modulo HTTP configurato per il prompt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 7013c8a88f047c5c8e769a4d7b71f2033c767b4a
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Generare un segmento di scenario utilizzando IA

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Poiché questa funzione è disponibile in Beta, è disponibile solo per alcuni utenti di Workfront.

Puoi utilizzare l’intelligenza artificiale per immettere un prompt di testo che descriva ciò che occorre fare in una sezione dello scenario. Fusion genera quindi moduli che eseguiranno tali azioni, che puoi utilizzare nello scenario.

Come per tutto ciò che viene generato dall’intelligenza artificiale, ti consigliamo di controllare e testare i moduli generati per verificare che funzionino come previsto.

## Applicazioni del modulo di IA attualmente supportate

Fusion AI può attualmente generare moduli che si connettono alle seguenti applicazioni:

* Adobe Firefly
* Azure OpenAI
* Grafico Microsoft
* Adobe Workfront Planning
* Adobe Analytics
* Servizi Adobe PDF
* Adobe Marketo
* Frame.io Adobe
* Dropbox
* NetSuite
* Calendario Google
* Jira Atlassian
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Genera moduli

1. Inizia ad aggiungere un modulo e seleziona **Genera con IA** dall&#39;elenco delle applicazioni.

   Oppure

   Fai clic sull&#39;icona Genera con IA ![Genera con IA](assets/generate-with-ai-icon-beta.png) nella parte inferiore della pagina dell&#39;editor di scenari.

   Viene aperto il pannello Assistente AI.
1. Immettere un prompt di testo nella casella.

   Per suggerimenti sui prompt, vedere [Suggerimenti per la creazione di prompt di testo](#tips-for-creating-text-prompts) in questo articolo.

   Viene generato il modulo o il set di moduli.
1. (Condizionale) Se necessario, aggiungi il token API per l’applicazione ai moduli.
1. Controlla i moduli per assicurarti che siano configurati per l’applicazione e l’azione appropriate.
1. (Condizionale) Se la sezione dello scenario generato non è associata allo scenario, trascinala nella posizione desiderata.

È consigliabile testare i moduli per verificare che funzionino come previsto.

## Suggerimenti per la creazione di prompt di testo

I prompt di testo devono includere almeno le seguenti informazioni:

* Applicazione a cui ci si connette
* Azione o azioni da eseguire

>[!IMPORTANT]
>
>È possibile generare più di un modulo alla volta, ma è possibile generare moduli solo per un&#39;applicazione alla volta.

>[!INFO]
>
>**Esempi**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Ciò include l&#39;applicazione `Workfront Planning` e l&#39;azione `delete records`. Questo prompt crea tre moduli, uno per ogni record che verrà eliminato.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Ciò include l&#39;applicazione `Workfront Planning` e l&#39;azione `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Ciò include l&#39;applicazione `Workfront Planning` e l&#39;azione `get field details`.
>
>L’esempio seguente NON è corretto:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Questo esempio non è corretto perché include più di un&#39;applicazione

Durante la creazione di prompt di testo, tenete presente quanto segue:

* Utilizza un linguaggio semplice e diretto.
* Verifica e verifica i moduli. Se non funziona come previsto, perfeziona la richiesta e riprova.

---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generare un modulo utilizzando IA
description: È possibile immettere un prompt di testo per creare un modulo HTTP configurato per il prompt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 5623ca255478757c58605d05f2f24e56b21a5d78
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Generare un modulo utilizzando IA

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Poiché questa funzione è ancora nelle prime fasi di sviluppo, è disponibile solo per gli utenti interni di Workfront.

È possibile utilizzare l’intelligenza artificiale per immettere un prompt di testo che descriva le operazioni che devono essere eseguite da un modulo. Fusion genera quindi un modulo HTTP che si connette all’endpoint corretto dell’API desiderata.

Come per tutto ciò che viene generato dall’intelligenza artificiale, ti consigliamo di controllare e testare il modulo generato per verificare che funzioni come previsto.

## Applicazioni del modulo di IA attualmente supportate

Fusion AI può attualmente generare moduli che si connettono alle seguenti applicazioni:

* Maestro Adobe
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

## Generare un modulo

1. Aggiungi un modulo e seleziona **Genera con IA** dall’elenco delle applicazioni.

   Oppure

   Fai clic con il pulsante destro del mouse su un’area vuota dell’editor di scenari, quindi seleziona **Genera con IA**.
1. Immettere un prompt di testo nella casella.

   Per suggerimenti sulle richieste, consulta [Suggerimenti per la creazione di prompt di testo](#tips-for-creating-text-prompts) in questo articolo.
1. Aggiungi il token API per l’applicazione al modulo.
1. Controlla il modulo per assicurarti che sembri configurato per l’applicazione e l’azione appropriate.
1. (Condizionale) Se il modulo non è allegato allo scenario, trascinalo nella posizione desiderata.

È consigliabile eseguire il test del modulo per verificare che il modulo generato funzioni come previsto.

## Suggerimenti per la creazione di prompt di testo

I prompt di testo devono includere almeno le seguenti informazioni:

* Applicazione a cui ci si connette
* Azione che si desidera eseguire

>[!INFO]
>
>**Esempi**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Ciò include l&#39;applicazione `Google Calendar` e l&#39;azione `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Ciò include l&#39;applicazione `Spotify` e l&#39;azione `Retrieve popular songs`.

Durante la creazione di prompt di testo, tenete presente quanto segue:

* Poiché ogni modulo di Fusion esegue una singola azione, il prompt di testo deve descrivere un&#39;azione specifica.
* Utilizza un linguaggio semplice e diretto.
* Verifica e verifica il modulo. Se non funziona come previsto, perfeziona la richiesta e riprova.




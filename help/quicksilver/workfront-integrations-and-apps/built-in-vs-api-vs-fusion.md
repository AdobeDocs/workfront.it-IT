---
content-type: reference
product-area: workfront-integrations
keywords: nativo,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Metodi di integrazione di Adobe Workfront
description: È possibile integrare [!DNL Adobe Workfront] con applicazioni di terze parti. Queste integrazioni possono estendere l'utilità di [!DNL Workfront] e adattalo alle esigenze della tua organizzazione. Puoi utilizzare una o tutte queste integrazioni, a seconda di quale risulta più utile per una determinata attività.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Metodi di integrazione di Adobe Workfront

È possibile integrare [!DNL Adobe Workfront] con applicazioni di terze parti e con altri [!DNL Adobe] prodotti. Queste integrazioni possono estendere l&#39;utilità di [!DNL Workfront] e adattalo alle esigenze della tua organizzazione. Puoi utilizzare una o tutte queste integrazioni, a seconda di quale risulta più utile per una determinata attività.

## Integrazioni integrate

Workfront fornisce varie integrazioni che è possibile configurare direttamente da Workfront o da un’altra applicazione installando il componente aggiuntivo Workfront per tale applicazione. Queste integrazioni integrate coprono molti scenari di casi d’uso comuni e si concentrano sull’estensione e la connessione di esperienze utente per gli utenti finali.

Le integrazioni integrate di Workfront si concentrano in gran parte sulla produttività e sulla collaborazione personali. Queste integrazioni riducono le interruzioni nel flusso di lavoro di un singolo utente, consentendo loro di ricevere notifiche Workfront, accedere alle informazioni e agire sugli elementi di lavoro Workfront senza uscire dall&#39;applicazione integrata.

I vantaggi delle integrazioni integrate possono includere:

* Molte di queste integrazioni integrate sono disponibili senza costi aggiuntivi. (Altri richiedono un acquisto aggiuntivo.)
* Le integrazioni integrate coprono molte delle applicazioni più comuni utilizzate dalle aziende, come [!DNL Slack], [!DNL Google Drive]oppure [!DNL Adobe] prodotti quali [!DNL Adobe Creative Cloud] o [!DNL Adobe Experience Manager] Risorse. Se l’azienda utilizza già queste app, l’integrazione avverrà senza problemi nel flusso di lavoro esistente degli utenti.
* Integrazione [!DNL Workfront] con un&#39;applicazione di uso frequente può aumentare l&#39;adozione tra gli utenti.

>[!INFO]
>
>**Esempio:**
>
>Con la [!DNL Workfront for Microsoft Teams integration], puoi ricevere notifiche in [!DNL Microsoft Teams] informazioni [!DNL Workfront] oggetti di lavoro. Senza partire [!DNL Microsoft Teams], è possibile eseguire azioni quali approvare, commentare o modificare lo stato degli elementi di lavoro. Qualsiasi modifica apportata agli elementi di lavoro [!DNL Microsoft Teams] sono riflessi in [!DNL Workfront] anche.

Per ulteriori informazioni sulle integrazioni integrate, incluso un elenco delle integrazioni integrate attualmente disponibili, consulta [[!DNL Adobe Workfront] panoramica delle integrazioni integrate](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Applicazioni OAuth2 personalizzate

Adobe [!DNL Workfront] gli amministratori possono creare applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono l&#39;accesso ad altre applicazioni [!DNL Workfront]. Gli utenti possono quindi concedere l&#39;autorizzazione a tali altre applicazioni per accedere ai loro [!DNL Workfront] dati. In questo modo, è possibile integrare Workfront con applicazioni a scelta, incluse le applicazioni interne.

>[!NOTE]
>
>Nel contesto di OAuth2, per &quot;creazione di un’app&quot; si intende il processo di creazione di questo tipo di collegamento di accesso tra un’app e un server come Workfront.

Vantaggi della creazione di un [!UICONTROL OAuth2] la domanda può comprendere quanto segue:

* Gli utenti possono utilizzare queste integrazioni direttamente in [!DNL Workfront], simile alle integrazioni integrate.
* Configurazione o utilizzo di un [!UICONTROL OAuth2] l&#39;applicazione non richiede conoscenze tecniche aggiuntive, come la familiarità con [!DNL Workfront] API.
* La tua organizzazione può utilizzare software non offerto come [!DNL Workfront] applicazione integrata. È ancora possibile integrare questo software con [!DNL Workfront] utilizzando un [!UICONTROL OAuth2] anche se il software è di proprietà dell&#39;organizzazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] offre un’API pubblica (interfaccia di programmazione dell’applicazione) che ti consente di estendere e migliorare la tua esperienza Workfront. L&#39;obiettivo per [!DNL Workfront] L’API è utile per semplificare la creazione di integrazioni personalizzate con [!DNL Workfront] introducendo un’architettura REST-ful che funziona tramite HTTP. La [!DNL Workfront] L’API richiede alcune conoscenze tecniche, ma è uno strumento molto potente per recuperare, creare e modificare i dati. Puoi personalizzare le chiamate API per eseguire funzioni molto specifiche.

Inoltre, [!DNL Workfront] offre un’API iscrizione agli eventi. Quando si verifica un&#39;azione su un [!DNL Workfront] oggetto supportato dalle sottoscrizioni di eventi, è possibile configurare [!DNL Workfront] per inviare una risposta all’endpoint desiderato. Ciò significa che le applicazioni di terze parti possono ricevere aggiornamenti da [!DNL Workfront] interazioni tramite [!DNL Workfront] API subito dopo il loro verificarsi.

Vantaggi dell&#39;utilizzo del [!DNL Workfront] L’API può includere quanto segue:

* È possibile utilizzare [!DNL Workfront] API per connettersi a quasi tutti gli altri servizi web o app che offrono un’API pubblica. È quindi possibile integrare [!DNL Workfront] con quasi tutti i servizi web o le app che desideri utilizzare.
* La [!DNL Workfront] La flessibilità dell&#39;API si estende anche al software proprietario dell&#39;azienda. Puoi utilizzare e modificare [!DNL Workfront] i dati contenuti all&#39;interno del software.
* Poiché le API sono così comuni al software, i tuoi sviluppatori interni probabilmente le conoscono. [!DNL Workfront] utilizza un’API REST-ful, il tipo di API più comune, che rende ancora più semplice per i tuoi sviluppatori avvicinarsi rapidamente.

>[!INFO]
>
>**Esempio:**
>
>La seguente chiamata API inserisce un commento nel flusso di aggiornamento dell’attività con l’ID specificato.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Per ulteriori informazioni sulla [!DNL Workfront] API, vedi [Nozioni di base sulle API](../wf-api/general/api-basics.md).

Per ulteriori informazioni sugli abbonamenti agli eventi, vedi [API iscrizione agli eventi](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] consente di automatizzare i flussi di lavoro. Con la [!DNL Workfront Fusion for Work Automation and Integration] In licenza, puoi creare queste automatizzazioni in più app e servizi web, creando scenari in cui le app lavorano insieme per eseguire un&#39;attività. Uno scenario è una rappresentazione visiva dell’attività o del flusso di lavoro generato utilizzando i moduli, che sono attività discrete come &quot;Scarica un documento&quot; o &quot;Crea un progetto&quot;. Si concatenano i moduli per definire il flusso di lavoro, quindi il flusso di lavoro viene eseguito automaticamente quando viene soddisfatta una condizione di attivazione.

Vantaggi per [!DNL Workfront Fusion] possono comprendere:

* [!DNL Workfront Fusion] non richiede tanto conoscenze tecniche quanto l’API, perché l’interfaccia visiva facilita la comprensione e la configurazione del flusso di lavoro. Ciò significa che può essere utilizzato da persone esterne a un team di sviluppo, il che può risparmiare tempo e denaro.
* Da [!DNL Workfront Fusion] funziona tramite l’API e può accedere alla maggior parte delle app e dei servizi web. Molte app dispongono di moduli per effettuare chiamate API, oppure è possibile utilizzare i moduli HTTP, SOAP o JSON per interagire con i servizi web che non dispongono di un [!DNL Workfront Fusion] connettore.

>[!INFO]
>
>**Esempio:**
>
>I seguenti [!DNL Workfront] modulo in [!DNL Workfront Fusion] è impostato per aggiungere un commento al progetto selezionato. Dopo l’esecuzione del modulo, il commento è visibile nel flusso di aggiornamento del progetto in Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Per ulteriori informazioni [!DNL Workfront Fusion], vedi [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).

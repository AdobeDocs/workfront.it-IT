---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Metodi di integrazione di Adobe Workfront
description: Puoi integrare [!DNL Adobe Workfront] con applicazioni di terze parti. Queste integrazioni possono estendere l'utilità di  [!DNL Workfront]  e personalizzarla in base alle esigenze della tua organizzazione. Puoi utilizzare una o tutte queste integrazioni, a seconda di quale sia più utile per una determinata attività.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Metodi di integrazione di Adobe Workfront

È possibile integrare [!DNL Adobe Workfront] con applicazioni di terze parti e altri prodotti [!DNL Adobe]. Queste integrazioni possono estendere l&#39;utilità di [!DNL Workfront] e adattarla alle esigenze della tua organizzazione. Puoi utilizzare una o tutte queste integrazioni, a seconda di quale sia più utile per una determinata attività.

## Integrazioni incorporate

Workfront offre varie integrazioni che è possibile configurare direttamente da Workfront o da un&#39;altra applicazione installando il componente aggiuntivo Workfront per tale applicazione. Queste integrazioni integrate coprono molti scenari di casi d’uso comuni e si concentrano sull’estensione e la connessione delle esperienze utente per gli utenti finali.

Le integrazioni integrate di Workfront si concentrano in larga misura sulla produttività personale e sulla collaborazione. Queste integrazioni riducono le interruzioni nel flusso di lavoro di un singolo utente, consentendo di ricevere notifiche Workfront, accedere alle informazioni e agire sugli elementi di lavoro di Workfront senza uscire dall’applicazione integrata.

I vantaggi delle integrazioni integrate possono includere quanto segue:

* Molte di queste integrazioni integrate sono disponibili senza costi aggiuntivi. (Altri richiedono un acquisto aggiuntivo).
* Le integrazioni incorporate coprono molte delle app più comuni utilizzate dalle aziende, ad esempio [!DNL Slack], [!DNL Google Drive] o [!DNL Adobe] prodotti come l&#39;Assets [!DNL Adobe Creative Cloud] o [!DNL Adobe Experience Manager]. Se la tua azienda utilizza già queste app, l’integrazione si realizzerà senza problemi all’interno del flusso di lavoro esistente degli utenti.
* L&#39;integrazione di [!DNL Workfront] con un&#39;applicazione utilizzata di frequente può aumentare il tasso di adozione tra gli utenti.

>[!INFO]
>
>**Esempio:**
>
>Con [!DNL Workfront for Microsoft Teams integration], puoi ricevere notifiche in [!DNL Microsoft Teams] sui tuoi [!DNL Workfront] elementi di lavoro. Senza uscire da [!DNL Microsoft Teams], è possibile eseguire azioni quali l&#39;approvazione, il commento o la modifica dello stato degli elementi di lavoro. Qualsiasi modifica apportata agli elementi di lavoro da [!DNL Microsoft Teams] si riflette anche in [!DNL Workfront].

Per ulteriori informazioni sulle integrazioni incorporate, incluso un elenco delle integrazioni incorporate attualmente disponibili, vedere [[!DNL Adobe Workfront] panoramica delle integrazioni incorporate](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Applicazioni OAuth2 personalizzate

Gli amministratori di Adobe [!DNL Workfront] possono creare applicazioni OAuth2 per l&#39;istanza di [!DNL Workfront], che consentono ad altre applicazioni di accedere a [!DNL Workfront]. Gli utenti potranno quindi concedere a queste altre applicazioni l&#39;autorizzazione di accesso ai propri dati di [!DNL Workfront]. In questo modo, è possibile integrare Workfront con le applicazioni di propria scelta, incluse quelle interne.

>[!NOTE]
>
>Nel contesto di OAuth2, &quot;creazione di un&#39;app&quot; si riferisce al processo di creazione di questo tipo di collegamento di accesso tra un&#39;app e un server come Workfront.

I vantaggi della creazione di un&#39;applicazione [!UICONTROL OAuth2] includono:

* Gli utenti possono utilizzare queste integrazioni direttamente in [!DNL Workfront], in modo analogo alle integrazioni incorporate.
* La configurazione o l&#39;utilizzo di un&#39;applicazione [!UICONTROL OAuth2] non richiede ulteriori conoscenze tecniche, ad esempio familiarità con l&#39;API [!DNL Workfront].
* L&#39;organizzazione può utilizzare software non disponibile come applicazione incorporata di [!DNL Workfront]. È comunque possibile integrare questo software con [!DNL Workfront] utilizzando un&#39;applicazione [!UICONTROL OAuth2], anche se il software è proprietario della tua organizzazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API [!DNL Workfront]

[!DNL Workfront] offre un&#39;API pubblica (interfaccia di programmazione dell&#39;applicazione) che consente di estendere e migliorare l&#39;esperienza Workfront. L&#39;obiettivo dell&#39;API [!DNL Workfront] è semplificare la creazione di integrazioni personalizzate con [!DNL Workfront] introducendo un&#39;architettura REST-ful che funzioni tramite HTTP. L&#39;API [!DNL Workfront] richiede alcune conoscenze tecniche, ma è uno strumento molto potente per recuperare, creare e modificare i dati. Puoi personalizzare le chiamate API per eseguire funzioni molto specifiche.

Inoltre, [!DNL Workfront] offre un&#39;API di sottoscrizione eventi. Quando si verifica un&#39;azione su un oggetto [!DNL Workfront] supportato dalle sottoscrizioni di eventi, è possibile configurare [!DNL Workfront] per inviare una risposta all&#39;endpoint desiderato. Ciò significa che le applicazioni di terze parti possono ricevere aggiornamenti dalle interazioni [!DNL Workfront] tramite l&#39;API [!DNL Workfront] subito dopo che si verificano.

I vantaggi dell&#39;utilizzo dell&#39;API [!DNL Workfront] possono essere i seguenti:

* È possibile utilizzare l&#39;API [!DNL Workfront] per connettersi a quasi tutti gli altri servizi Web o app che offrono un&#39;API pubblica. È quindi possibile integrare [!DNL Workfront] con quasi tutti i servizi Web o le app che si desidera utilizzare.
* La flessibilità dell&#39;API [!DNL Workfront] si estende anche al software proprietario dell&#39;azienda. Puoi utilizzare e modificare i dati di [!DNL Workfront] direttamente dal tuo software.
* Poiché le API sono così comuni al software, gli sviluppatori interni hanno probabilmente familiarità con esse. [!DNL Workfront] utilizza un&#39;API REST-ful, il tipo di API più comune, che rende ancora più semplice per gli sviluppatori mettersi al corrente rapidamente.

>[!INFO]
>
>**Esempio:**
>
>La seguente chiamata API inserisce un commento nel flusso di aggiornamento dell’attività con l’ID specificato.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Per ulteriori informazioni sull&#39;API [!DNL Workfront], vedere [Nozioni di base sull&#39;API](../wf-api/general/api-basics.md).

Per ulteriori informazioni sulle sottoscrizioni di eventi, vedere [API sottoscrizione eventi](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] consente di automatizzare i flussi di lavoro. Con la licenza [!DNL Workfront Fusion for Work Automation and Integration], è possibile creare tali automazioni in più app e servizi Web, creando scenari in cui le app collaborano per eseguire un&#39;attività. Uno scenario è una rappresentazione visiva dell&#39;attività o del flusso di lavoro creato utilizzando moduli, ovvero attività discrete quali &quot;Download di un documento&quot; o &quot;Creazione di un progetto&quot;. Puoi concatenare i moduli per definire il flusso di lavoro, che viene quindi eseguito automaticamente quando viene soddisfatta una condizione di attivazione.

I vantaggi di [!DNL Workfront Fusion] possono includere i seguenti:

* [!DNL Workfront Fusion] non richiede le stesse conoscenze tecniche dell&#39;API, in quanto l&#39;interfaccia visiva facilita la comprensione e l&#39;impostazione del flusso di lavoro. Ciò significa che può essere utilizzato da singoli utenti al di fuori di un team di sviluppo, risparmiando tempo e denaro all’organizzazione.
* Poiché [!DNL Workfront Fusion] funziona tramite l&#39;API, può accedere alla maggior parte delle app e dei servizi Web. Molte app dispongono di moduli per effettuare chiamate API, oppure puoi utilizzare i moduli HTTP, SOAP o JSON per interagire con servizi Web che non dispongono di un connettore [!DNL Workfront Fusion] dedicato.

>[!INFO]
>
>**Esempio:**
>
>Il seguente modulo [!DNL Workfront] in [!DNL Workfront Fusion] è configurato per aggiungere un commento al progetto selezionato. Dopo l’esecuzione del modulo, il commento è visibile nel flusso di aggiornamento del progetto in Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Per ulteriori informazioni su [!DNL Workfront Fusion], vedere [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).

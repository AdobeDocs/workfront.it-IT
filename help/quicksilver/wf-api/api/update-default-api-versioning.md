---
content-type: api
navigation-topic: api-navigation-topic
title: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
description: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito

Rilasceremo nuove versioni dell’API Adobe Workfront su base biennale. Ogni versione è supportata per tre anni dopo il rilascio, con un anno aggiuntivo in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Le integrazioni che non specificano una versione dell’API nell’URI vengono automaticamente indirizzate a Predefinito, che è stato dichiarato obsoleto. Affinché le integrazioni Workfront siano valide, devi specificare una versione API supportata nelle richieste API Workfront.

Per informazioni su come specificare una versione nelle richieste API, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

## Informazioni sulla versione predefinita dell’API

L’intento originale di &quot;default API&quot; (API predefinita), era quello di mapparla alla versione più recente dell’API Workfront. In questo modo i clienti con integrazioni di base denominate Predefinito non dovranno mai aggiornare le proprie richieste API.

Nel 2011, Workfront ha rilasciato la versione 3.0 dell’API. Il valore predefinito è stato spostato automaticamente nella versione 3.0, che ha interrotto molte integrazioni dei clienti che erano troppo complesse per utilizzare la versione 3.0 senza essere aggiornate. Di conseguenza, Workfront ha ripristinato questa modifica e ha lasciato la versione predefinita alla versione 2.

Sfortunatamente, questo argomento non è mai stato rivisto e ora, poiché abbiamo intenzione di aumentare notevolmente la funzionalità API, siamo costretti ad escludere le versioni precedenti della nostra API, incluso Default. Invece di aggiornare Default, che indubbiamente interromperebbe altre integrazioni, stiamo rimuovendo completamente il concetto di una versione predefinita. Questo è per incoraggiare i nostri clienti a utilizzare versioni stabili delle nostre API e a mantenere le loro integrazioni su un ciclo di, al massimo, tre anni.

## Impostazione predefinita obsoleta

Per migliorare l’API di Workfront, stiamo rimuovendo le versioni precedenti dell’API che hanno superato la finestra di supporto di tre anni. Una di queste versioni è la Versione 2, a cui è mappato il valore Predefinito. Questa versione è stata rilasciata nel 2010 e gran parte della logica supportata all’epoca nell’applicazione Attask/Workfront non esiste più o è sostanzialmente cambiata.

L’impostazione predefinita è stata rimossa a luglio 2017 e non verrà più designata come versione predefinita una versione specifica dell’API. Invece, tutte le richieste API di Workfront devono specificare una versione API specifica.

>[!IMPORTANT]
>
> Entro il 1° luglio 2018 tutte le integrazioni Workfront che utilizzano Default devono essere aggiornate per chiamare una versione API supportata specifica. Dopo tale data, tutte le richieste API di Workfront utilizzate dalle integrazioni che non specificano una versione avranno esito negativo.

Per informazioni sulla cadenza di obsolescenza di Workfront, consulta [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

## Aggiornamento delle integrazioni alle versioni API supportate

Se le richieste API di Workfront non specificano una versione, utilizzano Default. Devi aggiornare le richieste API per specificare una versione supportata dell’API, preferibilmente all’API supportata più recente.

Ad esempio, la seguente richiesta API di Workfront non specifica una versione API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando viene effettuata questa richiesta, ricevi una risposta con testo codificato JSON che specifica i dati dall’istanza Workfront. Poiché in questo URI non è specificata alcuna versione API, la chiamata passa a Predefinito.

Per trasformare una richiesta API predefinita in una richiesta API con versione, è sufficiente chiamare una versione API supportata. Ad esempio, il seguente URI richiede la versione 9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Quando aggiorni le richieste API di Workfront, puoi specificare qualsiasi versione supportata della nostra API. Per ulteriori informazioni sui riferimenti a un’API specifica, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

Per garantire la finestra di supporto massima, è necessario chiamare la versione più recente (Versione 9). Puoi trovare un elenco delle API supportate in [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

È fondamentale aggiornare le integrazioni che utilizzano Default. Se al momento disponi di integrazioni che non specificano una versione, potresti ricevere una notifica dal tuo venditore Workfront, dal responsabile del successo del cliente o dal rappresentante del supporto, o da un messaggio del centro annunci.

Al più presto, assicurati che le integrazioni siano aggiornate per chiamare una versione supportata della nostra API.

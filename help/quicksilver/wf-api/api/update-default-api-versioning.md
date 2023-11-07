---
content-type: api
navigation-topic: api-navigation-topic
title: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
description: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito

Rilasciamo nuove versioni dell’API di Adobe Workfront su base semestrale. Ogni versione è supportata per tre anni dopo il rilascio, con un ulteriore anno in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Le integrazioni che non specificano una versione dell’API nell’URI vengono instradate automaticamente all’impostazione predefinita. Se desideri che la chiamata API utilizzi una versione specifica dell’API, è necessario specificare tale versione nelle richieste API di Workfront.

>[!NOTE]
>
>Se l’organizzazione utilizza attualmente l’API predefinita, l’amministratore di Workfront ha ricevuto un messaggio Centro notifiche con ulteriori istruzioni relative all’API predefinita.

Per informazioni su come specificare una versione nelle richieste API, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

## Considerazioni durante l’utilizzo dell’API predefinita

Quando si lavora con l’API predefinita di Workfront, tieni presente quanto segue:

* La versione predefinita dell’API corrisponde alla versione più recente. Qualsiasi chiamata API senza la versione specificata utilizzerà la versione predefinita. Ogni volta che Workfront rilascia una nuova versione dell’API, la versione predefinita viene aggiornata alla versione più recente. **Pertanto, dopo il rilascio di una nuova versione dell’API Workfront, tutte le chiamate API che utilizzano la versione predefinita devono essere controllate per assicurarsi che la funzionalità sia ancora supportata**.
* Se l’organizzazione utilizza attualmente l’API predefinita obsoleta, l’amministratore di Workfront ha ricevuto un messaggio Centro notifiche con ulteriori istruzioni relative all’API predefinita.

Per visualizzare la versione più recente dell’API, consulta [Pianificazione del supporto e del controllo delle versioni API](../../wf-api/api/api-version-support-schedule.md).

## Aggiornamento delle integrazioni alle versioni API supportate

Se le richieste API di Workfront non specificano una versione, vengono utilizzate le impostazioni predefinite. È consigliabile che le richieste API specifichino una versione supportata dell’API, preferibilmente la più recente.

Ad esempio, la seguente richiesta API di Workfront non specifica una versione API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando viene effettuata questa richiesta, si riceve una risposta con testo codificato JSON che specifica i dati dell’istanza di Workfront. Poiché in questo URI non è specificata alcuna versione API, la chiamata viene impostata su Default.

Per trasformare una richiesta API predefinita in una richiesta API con versione, è sufficiente chiamare una versione API supportata. Ad esempio, l’URI seguente richiede la versione 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Quando aggiorni le richieste API di Workfront, puoi specificare qualsiasi versione supportata della nostra API. Per ulteriori informazioni sul riferimento a un’API specifica, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

Per garantire la finestra di supporto massima, è necessario chiamare la versione più recente. Puoi trovare un elenco delle API supportate in [Pianificazione del supporto e del controllo delle versioni API](../../wf-api/api/api-version-support-schedule.md).

## Cronologia della versione predefinita dell’API

L’obiettivo originale di &quot;Default API&quot; (API predefinita) era mapparla alla versione più recente dell’API di Workfront. In questo modo, i clienti con integrazioni di base che hanno chiamato Default non dovranno mai aggiornare le loro richieste API.

Nel 2011, Workfront ha rilasciato la versione 3.0 dell&#39;API. L’impostazione predefinita è stata spostata automaticamente nella versione 3.0, interrompendo così molte integrazioni dei clienti che erano troppo complesse per utilizzare la versione 3.0 senza essere aggiornate. Di conseguenza, Workfront ha annullato questa modifica e ha lasciato la versione predefinita alla versione 2.

Dal 2011, Workfront ha notevolmente aumentato la funzionalità API. Per questo motivo, le versioni precedenti delle nostre API sono state dichiarate obsolete. Nel 2017, invece di aggiornare Default, è stato completamente rimosso il concetto di versione predefinita. Questo era per incoraggiare i nostri clienti a utilizzare versioni stabili delle nostre API e a mantenere le loro integrazioni in un ciclo di, al massimo, tre anni.

Workfront sta ripristinando la versione API predefinita. L’API predefinita è impostata sulla versione più recente dell’API di Workfront e verrà aggiornata alla versione più recente ogni volta che viene rilasciata una nuova versione.


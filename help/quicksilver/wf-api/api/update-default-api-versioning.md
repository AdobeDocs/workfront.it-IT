---
content-type: api
navigation-topic: api-navigation-topic
title: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
description: Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito

Rilasceremo nuove versioni dell’API Adobe Workfront su base biennale. Ogni versione è supportata per tre anni dopo il rilascio, con un anno aggiuntivo in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Le integrazioni che non specificano una versione dell’API nell’URI vengono automaticamente indirizzate a Predefinito. Se desideri che la chiamata API utilizzi una versione specifica dell’API, devi specificarla nelle richieste API di Workfront.

>[!NOTE]
>
>Se l’organizzazione utilizza l’API predefinita, l’amministratore di Workfront ha ricevuto un messaggio Centro annunci con ulteriori istruzioni relative all’API predefinita.

Per informazioni su come specificare una versione nelle richieste API, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

## Considerazioni sull’utilizzo dell’API predefinita

Quando si lavora con l’API predefinita di Workfront, considera quanto segue:

* La versione predefinita dell’API, la versione più recente. Qualsiasi chiamata API senza la versione specificata utilizzerà la versione predefinita. Ogni volta che Workfront rilascia una nuova versione dell’API, la versione predefinita viene aggiornata alla versione più recente. **Pertanto, dopo aver rilasciato una nuova versione dell’API Workfront, tutte le chiamate API che utilizzano la versione predefinita devono essere verificate per assicurarti che la funzionalità sia ancora supportata**.
* Se l’organizzazione utilizza l’API predefinita precedente, obsoleta, l’amministratore di Workfront ha ricevuto un messaggio Centro annunci con ulteriori istruzioni relative all’API predefinita.

Per visualizzare la versione più recente dell’API, consulta [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

## Aggiornamento delle integrazioni alle versioni API supportate

Se le richieste API di Workfront non specificano una versione, utilizzano Default. È consigliabile che le richieste API specifichino una versione supportata dell’API, preferibilmente l’API supportata più recente.

Ad esempio, la seguente richiesta API di Workfront non specifica una versione API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Quando viene effettuata questa richiesta, ricevi una risposta con testo codificato JSON che specifica i dati dall’istanza Workfront. Poiché in questo URI non è specificata alcuna versione API, la chiamata passa a Predefinito.

Per trasformare una richiesta API predefinita in una richiesta API con versione, è sufficiente chiamare una versione API supportata. Ad esempio, il seguente URI richiede la versione 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Quando aggiorni le richieste API di Workfront, puoi specificare qualsiasi versione supportata della nostra API. Per ulteriori informazioni sui riferimenti a un’API specifica, consulta [Specificare una versione API nelle integrazioni](../../wf-api/api/specify-api-version-integrations.md).

Per garantire la finestra di supporto massima, è necessario chiamare la versione più recente. Puoi trovare un elenco delle API supportate in [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

## Cronologia della versione predefinita dell’API

L’intento originale di &quot;default API&quot; (API predefinita), era quello di mapparla alla versione più recente dell’API Workfront. In questo modo i clienti con integrazioni di base denominate Predefinito non dovranno mai aggiornare le proprie richieste API.

Nel 2011, Workfront ha rilasciato la versione 3.0 dell’API. Il valore predefinito è stato spostato automaticamente nella versione 3.0, che ha interrotto molte integrazioni dei clienti che erano troppo complesse per utilizzare la versione 3.0 senza essere aggiornate. Di conseguenza, Workfront ha ripristinato questa modifica e ha lasciato la versione predefinita alla versione 2.

Dal 2011, Workfront ha migliorato notevolmente le funzionalità API. Per questo motivo, abbiamo dichiarato obsolete le versioni precedenti della nostra API. Nel 2017, invece di aggiornare Default, abbiamo rimosso completamente il concetto di una versione predefinita. Questo era per incoraggiare i nostri clienti a utilizzare versioni stabili delle nostre API e a mantenere le loro integrazioni su un ciclo di, al massimo, tre anni.

Workfront sta ripristinando la versione API predefinita. L’API predefinita è impostata sulla versione più recente dell’API Workfront e viene aggiornata alla versione più recente ogni volta che viene rilasciata una nuova versione.


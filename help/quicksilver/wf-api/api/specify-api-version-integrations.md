---
content-type: api
navigation-topic: api-navigation-topic
title: Specificare una versione API nelle integrazioni
description: Specificare una versione API nelle integrazioni
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Specifica una versione API nelle integrazioni

Tutti gli URI di Adobe Workfront devono fare riferimento a una versione specifica dell’API dopo la porzione &quot;attask/api&quot; dell’URI. Nell&#39;esempio seguente viene chiamata la versione 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Assicurati che tutte le integrazioni chiamino le API Workfront attualmente supportate.

## Pianificazione della versione e obsolescenza delle API di Workfront

Vengono rilasciate regolarmente nuove versioni dell’API, in genere due volte all’anno. Ogni versione è supportata per tre anni dopo la data di rilascio, con un ulteriore anno in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Per ulteriori informazioni sulla cadenza della versione e sulla pianificazione delle versioni obsolete delle API di Workfront, consulta [Pianificazione del supporto e del controllo delle versioni API](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* La versione predefinita dell’API è impostata sulla versione più recente. Qualsiasi chiamata API senza la versione specificata utilizzerà la versione predefinita. Ogni volta che Workfront rilascia una nuova versione dell’API, la versione predefinita viene aggiornata alla versione più recente. **Pertanto, dopo il rilascio di una nuova versione dell’API Workfront, tutte le chiamate API che utilizzano la versione predefinita devono essere controllate per assicurarsi che la funzionalità sia ancora supportata.**
>
>* Se l’organizzazione utilizza attualmente l’API predefinita, l’amministratore di Workfront ha ricevuto un messaggio Centro notifiche con ulteriori istruzioni relative all’API predefinita.
>
>Per visualizzare la versione più recente dell’API, consulta [Pianificazione del supporto e del controllo delle versioni API](../../wf-api/api/api-version-support-schedule.md).


## Determinazione della versione API in uso

Puoi determinare la versione dell’API che stai utilizzando controllando l’URI di una richiesta HTTP inviata all’API Workfront. L’esempio seguente mostra un URI di richiesta Workfront che specifica la versione 15 dell’API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se un URI non specifica una versione, utilizza la versione predefinita dell’API, come illustrato nell’esempio seguente:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Le integrazioni che non specificano una versione dell’API nell’URI vengono instradate automaticamente alla versione predefinita dell’API.

## Aggiornamento delle integrazioni in base alle versioni API supportate

Quando crei o gestisci le integrazioni Workfront, devi includere un metodo per aggiornare dinamicamente la versione API e altre proprietà soggette a modifiche (come la chiave API).

Per rendere più efficiente l’aggiornamento delle integrazioni, prendi in considerazione i seguenti suggerimenti per la registrazione dei valori di integrazione:

* Memorizza i valori soggetti a modifiche future in un file di proprietà che tieni aggiornato
* Creare un servizio web per gestire le proprietà in tempo reale
* Memorizza i valori delle proprietà in un archivio dati che l&#39;applicazione può leggere

La progettazione delle integrazioni Workfront in quest’ottica riduce la necessità di un ampio lavoro di sviluppo quando tali valori inevitabilmente cambiano.

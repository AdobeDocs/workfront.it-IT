---
content-type: api
navigation-topic: api-navigation-topic
title: Specificare una versione API nelle integrazioni
description: Specificare una versione API nelle integrazioni
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Specificare una versione API nelle integrazioni

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Sandbox di anteprima.</span>

Tutti gli URI Adobe Workfront sono necessari per fare riferimento a una versione specifica dell’API dopo la parte &quot;attask/api&quot; dell’URI. L&#39;esempio seguente chiama la versione 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Assicurati che tutte le chiamate di integrazione siano API Workfront attualmente supportate.

## Pianificazione del rilascio e della rimozione delle API Workfront

Le nuove versioni dell’API vengono rilasciate regolarmente, di solito due volte all’anno. Ogni versione è supportata per tre anni dopo la data di rilascio, con un anno aggiuntivo in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Per ulteriori informazioni sulla cadenza del rilascio e sulla pianificazione della rimozione dalle API di Workfront, consulta [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Dopo la versione 23.2, la versione predefinita dell’API sarà impostata sulla versione più recente. Qualsiasi chiamata API senza la versione specificata utilizzerà la versione predefinita. Ogni volta che Workfront rilascia una nuova versione dell’API, la versione predefinita viene aggiornata alla versione più recente. Pertanto, dopo la pubblicazione di una nuova versione dell’API Workfront, tutte le chiamate API che utilizzano la versione predefinita devono essere verificate per assicurarsi che la funzionalità sia ancora supportata.
>
>* Se l’organizzazione utilizza l’API predefinita, l’amministratore di Workfront ha ricevuto un messaggio Centro annunci con ulteriori istruzioni relative all’API predefinita.
>
>* <span class="preview">L’API predefinita nell’ambiente Anteprima è impostata sulla versione più recente. L’API predefinita nell’ambiente di produzione sarà impostata sulla versione più recente dopo la versione 23.2 (aprile 2023)</span>.
>
>Per visualizzare la versione più recente dell’API, consulta [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).


## Determinazione della versione API in uso

Puoi determinare la versione dell’API che utilizzi controllando l’URI di una richiesta HTTP inviata all’API Workfront. L’esempio seguente mostra un URI di richiesta Workfront che specifica la versione 15 dell’API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se un URI non specifica una versione, utilizza la versione predefinita dell’API, come illustrato nell’esempio seguente:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Le integrazioni che non specificano una versione dell’API nell’URI vengono automaticamente indirizzate alla versione predefinita dell’API.

## Aggiornamento delle integrazioni per utilizzare le versioni API supportate

Quando crei o gestisci le integrazioni Workfront, devi includere un metodo per aggiornare dinamicamente la versione API e altre proprietà soggette a modifica (ad esempio la chiave API).

Per rendere l’aggiornamento delle integrazioni più efficiente, prendi in considerazione i seguenti suggerimenti per la registrazione dei valori di integrazione:

* Memorizza valori soggetti a modifiche future in un file di proprietà che mantieni aggiornato
* Creare un servizio Web per gestire le proprietà in tempo reale
* Memorizzazione dei valori delle proprietà in un archivio dati leggibile dall&#39;applicazione

Progettare le integrazioni Workfront tenendo presente questo aspetto riduce la necessità di un ampio lavoro di sviluppo quando tali valori inevitabilmente cambiano.

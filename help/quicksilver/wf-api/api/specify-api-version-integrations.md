---
content-type: api
navigation-topic: api-navigation-topic
title: Specificare una versione API nelle integrazioni
description: Specificare una versione API nelle integrazioni
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Specificare una versione API nelle integrazioni

Tutti gli URI Adobe Workfront sono necessari per fare riferimento a una versione specifica dell’API dopo la parte &quot;attask/api&quot; dell’URI. L&#39;esempio seguente chiama la versione 7.0:
`attask/api/v7.0/<objectName>/<objectId>` Assicurati che tutte le chiamate di integrazione siano API Workfront attualmente supportate.

## Pianificazione del rilascio e della rimozione delle API Workfront

Le nuove versioni dell’API vengono rilasciate ogni due mesi, ogni sei-otto mesi. Ogni versione è supportata per tre anni dopo la data di rilascio, con un anno aggiuntivo in uno stato obsoleto in cui la versione è disponibile ma non supportata.

Per ulteriori informazioni sulla cadenza del rilascio e sulla pianificazione della rimozione dalle API di Workfront, consulta [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

A partire da luglio 2017, Workfront ha dichiarato obsoleta la versione predefinita dell’API. Ciò significa che Workfront non designa più una versione specifica dell’API come versione predefinita. Per essere valido, tutti gli URI API futuri devono specificare una versione dell’API.

>[!IMPORTANT]
>
> Eventuali integrazioni che utilizzano la versione API predefinita devono essere aggiornate per chiamare una versione API supportata specifica entro il 1° luglio 2018.

## Determinazione della versione API in uso

Puoi determinare la versione dell’API che utilizzi controllando l’URI di una richiesta HTTP inviata all’API Workfront. L’esempio seguente mostra un URI di richiesta Workfront che specifica la versione 7 dell’API:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se un URI non specifica una versione, utilizza la versione predefinita dell’API, come illustrato nell’esempio seguente:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Le integrazioni che non specificano una versione dell’API nell’URI vengono automaticamente indirizzate alla versione predefinita dell’API e non possono funzionare dopo il 1° luglio 2018.

## Aggiornamento delle integrazioni per utilizzare le versioni API supportate

Quando crei o gestisci le integrazioni Workfront, devi includere un metodo per aggiornare dinamicamente la versione API e altre proprietà soggette a modifica (ad esempio la chiave API).

Per rendere l’aggiornamento delle integrazioni più efficiente, prendi in considerazione i seguenti suggerimenti per la registrazione dei valori di integrazione:

* Memorizza valori soggetti a modifiche future in un file di proprietà che mantieni aggiornato
* Creare un servizio Web per gestire le proprietà in tempo reale
* Memorizzazione dei valori delle proprietà in un archivio dati leggibile dall&#39;applicazione

Progettare le integrazioni Workfront tenendo presente questo aspetto riduce la necessità di un ampio lavoro di sviluppo quando tali valori inevitabilmente cambiano.

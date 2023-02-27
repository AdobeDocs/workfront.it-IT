---
content-type: api
keywords: API,dati,sincronizzazione,diario,entrata,oggetto
navigation-topic: general-api
title: Utilizza l’API per sincronizzare i dati per programmi e servizi
description: Utilizza l’API per sincronizzare i dati per programmi e servizi
author: Becky
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Utilizzo dell’API per sincronizzare i dati per programmi e servizi

Questi sono alcuni modi comuni per utilizzare l’API per sincronizzare i dati per programmi e servizi.

## Aggiornamenti in tempo reale

Adobe Workfront utilizza &quot;Sottoscrizioni evento&quot; (comunemente chiamati anche webhook) per inviare aggiornamenti in tempo reale sugli oggetti e le azioni supportati, tramite l’API, agli endpoint desiderati. È previsto di ricevere un aggiornamento relativo ai nuovi oggetti e azioni entro 5 secondi, ma in media gli aggiornamenti arrivano tra circa 1 secondo. Per ulteriori informazioni sul tipo di oggetti supportati, sui tipi di azioni supportati, sui dettagli tecnici e sugli esempi di configurazione delle sottoscrizioni di eventi, consulta [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md) e [Requisiti di consegna abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Aggiornamenti in batch

Gli aggiornamenti in batch sono un modo per configurare il sistema per gli aggiornamenti effettuando richieste periodiche ai server Workfront. Esistono molti modi per farlo, ma in genere il processo consiste nel richiedere al servizio di effettuare una richiesta ai server API di Workfront e nella ricerca di oggetti creati o modificati dall’ultima chiamata di richiesta. Per informazioni sulle chiamate potenziali e sui parametri utili, consulta la sezione [Comportamento GET](../../wf-api/general/api-basics.md#get-behavior) dalla sezione [Nozioni di base sulle API](../../wf-api/general/api-basics.md) articolo.

Mentre si sta impostando il servizio per gli aggiornamenti batch qui ci sono alcune cose importanti da tenere a mente:

### Date di ingresso

Le date di ingresso vengono memorizzate utilizzando la formattazione ISO 8601. Questo standard include informazioni su data, ora e fuso orario.

**Esempio:** Formato data ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Sia la data di creazione di un oggetto che l&#39;ultima data di modifica dell&#39;oggetto sono memorizzate rispettivamente come &quot;entryDate&quot; e &quot;lastUpdateDate&quot;. Per informazioni approfondite sugli oggetti Workfront, i campi associati e i nomi dei campi, consultare la sezione [Esplora API](../../wf-api/general/api-explorer.md). Si noti che l&#39;entryDate per un determinato oggetto Workfront non cambia, dove man mano che l&#39;oggetto viene modificato l&#39;ultimoUpdatedDate ogni volta che l&#39;oggetto viene modificato.

**Esempio:** richiesta di GET per un oggetto problema, utilizzando **lastUpdateDate** campo . Questa richiesta restituirà tutti i problemi aggiornati a partire da quella data specificata.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Oggetto Journal Entry

Se si desidera ottenere le modifiche relative a un campo specifico di un oggetto, è possibile eseguire una query sull&#39;oggetto &quot;Journal Entry&quot;. È possibile impostare l&#39;oggetto Workfront Journal Entry per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati, vedere [Configurare gli aggiornamenti di sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) per ulteriori dettagli.

Quando un campo è configurato per essere registrato come parte dell&#39;oggetto Journal Entry, ogni volta che tale campo viene modificato viene creata una voce Journal corrispondente. Quindi, puoi eseguire una query sull&#39;oggetto Journal Entry utilizzando una chiamata API simile alla seguente:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; viene utilizzato per esaminare una scrittura contabile di una modifica, invece di guardare l&#39;oggetto modificato stesso.

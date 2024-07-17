---
content-type: api
keywords: API,dati,sincronizzazione,diario,voce,oggetto
navigation-topic: general-api
title: Utilizzare l’API per sincronizzare i dati per programmi e servizi
description: Utilizzare l’API per sincronizzare i dati per programmi e servizi
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Utilizzo dell’API per sincronizzare i dati per programmi e servizi

Di seguito sono riportati alcuni modi comuni per utilizzare l’API per sincronizzare i dati per programmi e servizi.

## Aggiornamenti quasi in tempo reale

Adobe Workfront utilizza &quot;Sottoscrizioni eventi&quot; (comunemente noti anche come webhook) per inviare aggiornamenti in tempo quasi reale, tramite l’API, sugli oggetti e le azioni supportati agli endpoint desiderati. È possibile ricevere un aggiornamento relativo a nuovi oggetti e azioni entro 5 secondi, ma in media gli aggiornamenti arrivano in circa 1 secondo. Per ulteriori informazioni sul tipo di oggetti supportati, sui tipi di azioni supportati, sui dettagli tecnici e sugli esempi per la configurazione delle sottoscrizioni di eventi, vedere [API sottoscrizione eventi](../../wf-api/general/event-subs-api.md) e [Requisiti di consegna sottoscrizione eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Aggiornamenti batch

Gli aggiornamenti in batch consentono di configurare il sistema per gli aggiornamenti effettuando richieste periodiche ai server Workfront. Esistono molti modi per farlo, ma in genere il processo consiste nel richiedere al servizio di effettuare una richiesta ai server API di Workfront e nel cercare oggetti creati o modificati dopo l’ultima chiamata della richiesta. GET Per informazioni sulle potenziali chiamate di richieste e sui parametri utili, consulta la sezione [Comportamento](../../wf-api/general/api-basics.md#get-behavior) dell&#39;articolo [Nozioni di base sulle API](../../wf-api/general/api-basics.md).

Durante la configurazione del servizio per gli aggiornamenti in batch, tieni presente alcuni aspetti importanti:

### Date di ingresso

Le date di ingresso vengono memorizzate utilizzando la formattazione ISO 8601. Questo standard include informazioni su data, ora e fuso orario.

**Esempio:** formato data ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

La data di creazione e l&#39;ultima data di modifica dell&#39;oggetto vengono memorizzate rispettivamente come &quot;entryDate&quot; e &quot;lastUpdateDate&quot;. Per informazioni dettagliate sugli oggetti Workfront, sui campi associati e sui nomi dei campi, vedere [API Explorer](../../wf-api/general/api-explorer.md). Si noti che entryDate per un determinato oggetto Workfront non viene modificato, in quanto lastUpdatedDate cambia ogni volta che l&#39;oggetto viene modificato.

**Esempio:** GET richiesta per un oggetto problema, utilizzando il campo **lastUpdateDate**. Con questa richiesta vengono restituiti tutti i problemi aggiornati a partire dalla data specificata.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Oggetto voce diario

Se si desidera ottenere modifiche relative a un campo specifico di un oggetto, è possibile eseguire una query sull&#39;oggetto &quot;Voce diario&quot;. L&#39;oggetto Workfront Journal Entry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che questi campi vengono modificati. Per ulteriori informazioni, vedere [Configurare gli aggiornamenti del sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Quando un campo viene impostato per essere registrato come parte dell&#39;oggetto Voce diario, verrà creata una voce diario corrispondente ogni volta che tale campo viene modificato. È quindi possibile eseguire una query sull&#39;oggetto Voce diario utilizzando una chiamata API simile alla seguente:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; viene utilizzato per esaminare una voce del diario di una modifica, anziché esaminare l&#39;oggetto modificato stesso.

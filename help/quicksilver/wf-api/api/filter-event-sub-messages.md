---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrare i messaggi di abbonamento agli eventi
description: Filtrare i messaggi di abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 0%

---

# Filtrare i messaggi di abbonamento agli eventi

Puoi creare componenti di elaborazione intermediari che ti aiutino a filtrare ed elaborare solo i messaggi di abbonamento agli eventi di cui la tua azienda ha bisogno.

Per informazioni sulle sottoscrizioni di eventi, vedere [API sottoscrizione eventi](../../wf-api/general/event-subs-api.md).

## Filtraggio dei messaggi di evento

Questa sezione contiene snippet di codice di filtro che puoi implementare per ridurre il caricamento dei messaggi di abbonamento agli eventi.  Per illustrare le differenze nella sintassi delle varie lingue, questi snippet illustrano lo stesso set di filtri scritti nelle seguenti lingue:

Puoi visualizzare esempi di filtro in [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), dove puoi vedere le differenze di sintassi per ogni linguaggio e i mezzi di interazione con l&#39;SDK di AWS.Questi esempi sono scritti come AWS Lambdas, un metodo comune per l&#39;utilizzo di componenti di filtro ed elaborazione intermediari.

I seguenti snippet di codice sono pronti per la distribuzione e possono essere utilizzati come punto di partenza per aiutarti a scrivere filtri e componenti di elaborazione personalizzati e più complessi.

### Java

L&#39;esempio seguente in Java mostra come filtrare i payload del progetto in base all&#39;ID gruppo del progetto, come fatto in [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Stabilisci l’ID gruppo che stai cercando e crealo come costante statica.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   In questo esempio, il metodo handleRequest, che è un nome di metodo standard AWS Lambda, utilizza come primo parametro un tipo Map, ovvero il contenuto del messaggio di sottoscrizione dell&#39;evento.\
   Il secondo parametro utilizzato è il contesto della richiesta proxy Lambda corrente.\
   L’oggetto Context viene utilizzato per ottenere un logger Lambda, utilizzato per scrivere un messaggio in CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Quando si richiama il metodo handleRequest, ottenere l&#39;attributo &quot;newState&quot; del messaggio di sottoscrizione dell&#39;evento, che rappresenta lo stato aggiornato della risorsa.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Per informazioni sul formato newState, vedere [Formato dei messaggi in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

3. Dopo aver analizzato la mappa &quot;newState&quot; dal messaggio, assicurati che l’ID gruppo dell’oggetto corrisponda all’ID gruppo identificato nel passaggio 1.

4. (Condizionale) Se gli ID **non corrispondono**, elimina il messaggio in modo che venga restituita una risposta vuota.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >La restituzione di una risposta vuota e di successo è fondamentale. Qualsiasi cosa che non sia una risposta di 200 livelli è considerata una consegna non riuscita.

5. Elabora il messaggio.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, responsabile della distribuzione del messaggio filtrato all’endpoint desiderato.

   Lo scopo di trasferire la responsabilità della consegna del messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout consentito per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione, puoi elaborare la richiesta, ma il servizio Sottoscrizione eventi si interrompe e rientra in un ciclo di nuovi tentativi fino a quando non riceve una risposta di 200 livelli entro il periodo di timeout.

   Per ulteriori informazioni sulla gestione della consegna dei messaggi, vedere [Miglioramento della consegna dei messaggi durante la gestione dei timeout](#improving-message-delivery-while-accommodating-timeouts).

### Python

La differenza principale tra gli esempi Java e Python è che nell&#39;esempio Java il messaggio di abbonamento all&#39;evento viene ricevuto come primo parametro, e nell&#39;esempio Python il primo parametro è un &quot;evento&quot; proxy Lambda, che contiene il messaggio di abbonamento all&#39;evento insieme alle informazioni sulla richiesta proxy AWS Lambda.

L&#39;esempio seguente in Python mostra come filtrare i payload del progetto in base all&#39;ID gruppo del progetto, come fatto in [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Stabilisci l’ID gruppo che stai cercando e crealo come costante statica.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Il primo parametro è il proxy Lambda &quot;event&quot;, che contiene il messaggio di abbonamento all’evento e alcune informazioni aggiuntive da analizzare.\
   Il secondo parametro è il contesto della richiesta proxy Lambda corrente.\
   In questo esempio, l&#39;oggetto Context viene utilizzato per ottenere un Logger Lambda, utilizzato per scrivere un messaggio in CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analizza il messaggio dell’evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Ottieni l’attributo &quot;newState&quot; del messaggio di abbonamento dell’evento.\
   L&#39;attributo newState rappresenta lo stato aggiornato della risorsa.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Per informazioni sul formato newState, vedere [Formato dei messaggi in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

1. Dopo aver analizzato la mappa &quot;newState&quot; dal messaggio, assicurati che l’ID gruppo dell’oggetto corrisponda all’ID gruppo identificato nel passaggio 1.

1. (Condizionale) Se gli ID non corrispondono, rilascia il messaggio in modo che venga restituita una risposta vuota.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >La restituzione di una risposta vuota e di successo è fondamentale. Qualsiasi cosa che non sia una risposta di 200 livelli è considerata una consegna non riuscita.

1. Elabora il messaggio.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, responsabile della distribuzione del messaggio filtrato all’endpoint desiderato.

   Lo scopo di trasferire la responsabilità della consegna del messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione, puoi elaborare la richiesta, ma il servizio Sottoscrizione eventi si interrompe e rientra in un ciclo di nuovi tentativi fino a quando non riceve una risposta di 200 livelli entro il periodo di timeout.


### Node.js

L’esempio di Node.js del filtro degli ID del gruppo di progetti è simile agli esempi Java e Python. Come nell&#39;esempio di Python, il primo parametro è un evento proxy Lambda e il secondo parametro è il contesto Lambda.

L&#39;esempio seguente in Node.js mostra come filtrare i payload del progetto in base all&#39;ID gruppo del progetto, come fatto in [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Stabilisci l’ID gruppo che stai cercando e crealo come costante statica.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Il primo parametro è il proxy Lambda &quot;event&quot;, che contiene il messaggio di abbonamento all’evento e alcune informazioni aggiuntive da analizzare.\
   Il secondo parametro è il contesto della richiesta proxy Lambda corrente.\
   In questo esempio, l&#39;oggetto Context viene utilizzato per ottenere un Logger Lambda, utilizzato per scrivere un messaggio in CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analizza il messaggio dell’evento.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Ottieni projectGroupID dall’attributo &quot;newState&quot; del messaggio di abbonamento all’evento, quindi confrontalo con l’ID del gruppo identificato nel passaggio 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Per informazioni sul formato newState, vedere [Formato dei messaggi in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

4. (Condizionale) Se gli ID non corrispondono, rilascia il messaggio in modo che venga restituita una risposta vuota.\
   L’esempio seguente mostra gli ID gruppo corrispondenti:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >La restituzione di una risposta vuota e di successo è fondamentale. Qualsiasi cosa che non sia una risposta di 200 livelli è considerata una consegna non riuscita.

5. Elabora il messaggio.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, responsabile della distribuzione del messaggio filtrato all’endpoint desiderato.\
   Lo scopo di trasferire la responsabilità della consegna del messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione, puoi elaborare la richiesta, ma il servizio Sottoscrizione eventi si interrompe e rientra in un ciclo di nuovi tentativi fino a quando non riceve una risposta di 200 livelli entro il periodo di timeout.\
   Per informazioni sulla gestione della consegna dei messaggi, vedere [Miglioramento della consegna dei messaggi durante la gestione dei timeout](#improving-message-delivery-while-accommodating-timeouts).

## Miglioramento Della Consegna Dei Messaggi Durante La Gestione Dei Timeout

Il servizio Sottoscrizione eventi ha un timeout rigoroso di **cinque secondi** per tutte le richieste di consegna. Nel caso in cui la consegna di un messaggio superi il tempo consentito, il servizio Sottoscrizione eventi avvia un ciclo di nuovi tentativi per tale messaggio.

Ad esempio, si crea un filtro ID gruppo di progetti simile a uno degli esempi trovati in [Filtraggio dei messaggi evento](#filtering-event-messages) e si include una ricerca nel database per determinare se il messaggio è necessario. È possibile che la ricerca nel database e il tempo necessario per l’elaborazione richiesta e per l’avvio a freddo di Lambda possano richiedere più di cinque secondi, causando un nuovo tentativo di consegna del messaggio da parte del servizio Sottoscrizione eventi.

È possibile evitare un nuovo tentativo separando le parti del processo che richiedono tempo dalla logica responsabile di determinare se il messaggio deve essere elaborato e consegnato. In questo modo, è possibile accettare il messaggio e inviare una risposta di 200 livelli al servizio Sottoscrizione eventi, continuando in modo asincrono a elaborare o filtrare il messaggio in background (vedi il passaggio 5 in [Java](#java) per un esempio).


Anche se l’elaborazione o il filtro non supera il timeout di cinque secondi, è comunque vantaggioso separare il primo punto di contatto del filtro o dell’elaborazione dei messaggi dagli altri passaggi di elaborazione o consegna sul lato client. In questo modo il passaggio del messaggio alla destinazione dal servizio di abbonamento agli eventi ha un impatto minimo su entrambe le parti in termini di tempo e prestazioni.

Per ulteriori informazioni sul meccanismo di esecuzione dei nuovi tentativi, vedere [Nuovi tentativi di sottoscrizione evento](../../wf-api/api/event-sub-retries.md).

## Implementazione dei filtri in hosting nell’architettura cloudless

Se non riesci a sfruttare un&#39;architettura cloud per filtrare gli abbonamenti agli eventi, puoi comunque utilizzare gli esempi in [Filtro dei messaggi agli eventi](#filtering-event-messages) come roadmap per implementare i filtri ospitati o i componenti di elaborazione.

### Regolazione degli esempi di filtro per i servizi autonomi

Prima di utilizzare gli esempi di filtro in un ambiente senza cloud, effettua le seguenti operazioni:

* Ometti le parti specifiche per Lambda degli esempi, ad esempio il parametro Context.

* Modifica le chiamate di altri Lambda negli esempi per effettuare richieste HTTP asincrone aggiuntive ad altri filtri o componenti di elaborazione che ospiti.

* Se fai riferimento agli esempi Python e Node.js, sostituisci il primo parametro evento con il primo parametro payload mostrato nell’esempio Java. Vedi il passaggio 1 in [Java](#java).

* Distribuisci filtri o processori con un’API basata su web.

### Prevenzione dei messaggi di abbonamento agli eventi mancanti

A volte, in un’architettura senza cloud, i servizi responsabili della ricezione dei messaggi di abbonamento agli eventi potrebbero non essere raggiungibili. In questo caso, i messaggi potrebbero superare il limite di tentativi e andare persi, senza poter recuperare le informazioni all’interno dei messaggi.

All’avvio del servizio, consigliamo di implementare una query per richiedere lo stato più recente di tutte le risorse che potrebbero essere state incluse nei messaggi non recapitati. Come mostrato nell’esempio seguente, è possibile utilizzare i criteri di filtro per eseguire query sulle risorse che corrispondono a tali criteri e quindi elaborarne lo stato corrente.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Ricercando le risorse, assicurati che i sistemi di integrazione dispongano della versione più recente.

### Implementazione dell’elaborazione asincrona nella consegna dei messaggi

Tutti gli esempi nella sezione [Filtro dei messaggi evento](#filtering-event-messages) passano la responsabilità di consegnare i messaggi filtrati a un altro AWS Lambda. Questa operazione viene eseguita per evitare di superare il timeout di cinque secondi nella richiesta di consegna, applicato dal servizio Sottoscrizione eventi che emette la richiesta.

In un’architettura senza cloud, potrebbe essere necessario implementare un meccanismo di elaborazione asincrona simile a quello dell’SDK di AWS per le chiamate asincrone ad altri AWS Lambda. La maggior parte dei linguaggi di programmazione moderni dispone di librerie di terze parti o core che gestiscono l’elaborazione asincrona, consentendo di sfruttare lo stile di elaborazione asincrona implementato nei nostri esempi.

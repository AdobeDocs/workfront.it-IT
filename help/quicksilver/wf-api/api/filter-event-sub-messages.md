---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrare i messaggi di abbonamento agli eventi
description: Filtrare i messaggi di abbonamento agli eventi
author: Becky
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Filtrare i messaggi di abbonamento agli eventi

Puoi creare componenti di elaborazione intermedie che ti aiutano a filtrare ed elaborare solo i messaggi di abbonamento agli eventi di cui hai bisogno.

Per informazioni sugli abbonamenti agli eventi, vedi [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md).

## Filtrare i messaggi evento

Questa sezione contiene frammenti di codice di filtro che puoi implementare per ridurre il carico dei messaggi di abbonamento agli eventi.  Per aiutare a mostrare le differenze nella sintassi di varie lingue, questi snippet illustrano lo stesso set di filtri scritti nelle seguenti lingue:

Puoi visualizzare esempi di filtraggio in [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), dove puoi vedere le differenze nella sintassi per ogni lingua e i mezzi di interazione con l’SDK di AWS. Questi esempi sono scritti come AWS Lambdas, un metodo comune per l’utilizzo dei componenti di filtraggio e elaborazione intermedi.

I seguenti snippet di codice sono quasi pronti per l’implementazione e possono essere utilizzati come punto di partenza per la scrittura di filtri e componenti di elaborazione personalizzati e più complessi.

### Java

L’esempio seguente in Java mostra come filtrare i payload del progetto in base all’ID gruppo del progetto, come avviene in [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Stabilisci l&#39;ID gruppo che stai cercando e crealo come costante statica.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   In questo esempio, il metodo handleRequest, che è un nome di metodo standard AWS Lambda, prende un tipo Map come primo parametro, che è il contenuto del messaggio di abbonamento all&#39;evento.\
   Il secondo parametro necessario è il contesto della richiesta Lambda Proxy corrente.\
   L&#39;oggetto Context viene utilizzato per ottenere un logger Lambda, utilizzato per scrivere un messaggio su CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Dopo aver invocato il metodo handleRequest, ottieni l’attributo &quot;newState&quot; del messaggio di sottoscrizione dell’evento, che rappresenta lo stato aggiornato della risorsa.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Per informazioni sul formato newState, vedi [Formato del messaggio in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

3. Dopo aver analizzato la mappa &quot;newState&quot; dal messaggio, assicurati che l’ID gruppo dell’oggetto corrisponda all’ID gruppo identificato al passaggio 1.

4. (Condizionale) Se gli ID sono **non** match, rilascia il messaggio in modo che venga restituita una risposta vuota.

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
   >È fondamentale restituire una risposta vuota e di successo. Qualsiasi elemento oltre a una risposta a 200 livelli è considerato una consegna non riuscita.

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

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, che è responsabile della consegna del messaggio filtrato all’endpoint desiderato.

   Lo scopo di trasferire la responsabilità di consegnare il messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout consentito per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione , puoi elaborare la richiesta, ma il servizio di abbonamento agli eventi scadrà e passerà in un ciclo di tentativi fino a quando non riceverà una risposta a 200 livelli entro il periodo di timeout.

   Per ulteriori informazioni sulla gestione della consegna dei messaggi, consulta [Miglioramento Della Distribuzione Dei Messaggi Durante L&#39;Alloggio Dei Timeout](#improving-message-delivery-while-accommodating-timeouts).

### Pitone

La differenza principale tra gli esempi Java e Python è che nell&#39;esempio Java il messaggio di abbonamento all&#39;evento viene ricevuto come primo parametro, e nell&#39;esempio Python il primo parametro è un proxy Lambda &quot;event&quot;, che contiene il messaggio di abbonamento all&#39;evento insieme a informazioni sulla richiesta proxy AWS Lambda.

L’esempio seguente in Python mostra come filtrare i payload del progetto in base all’ID gruppo del progetto, come avviene in  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Stabilisci l&#39;ID gruppo che stai cercando e crealo come costante statica.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Il primo parametro è il proxy Lambda &quot;event&quot;, che contiene il messaggio di abbonamento all’evento e alcune informazioni aggiuntive da analizzare.\
   Il secondo parametro è il contesto dell&#39;attuale richiesta del proxy Lambda.\
   In questo esempio, l&#39;oggetto Context viene utilizzato per ottenere un logger Lambda, utilizzato per scrivere un messaggio su CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analizza il messaggio dall’evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Ottieni l’attributo &quot;newState&quot; del messaggio di sottoscrizione dell’evento.\
   L&#39;attributo newState rappresenta lo stato aggiornato della risorsa.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Per informazioni sul formato newState, vedi [Formato del messaggio in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

1. Dopo aver analizzato la mappa &quot;newState&quot; dal messaggio, assicurati che l’ID gruppo dell’oggetto corrisponda all’ID gruppo identificato al passaggio 1.

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
   >È fondamentale restituire una risposta vuota e di successo. Qualsiasi elemento oltre a una risposta a 200 livelli è considerato una consegna non riuscita.

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

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, che è responsabile della consegna del messaggio filtrato all’endpoint desiderato.

   Lo scopo di trasferire la responsabilità di consegnare il messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione , puoi elaborare la richiesta, ma il servizio di abbonamento agli eventi scadrà e passerà in un ciclo di tentativi fino a quando non riceverà una risposta a 200 livelli entro il periodo di timeout.


### Node.js

L&#39;esempio Node.js di filtro ID gruppo di progetti legge simili agli esempi Java e Python. Come per l&#39;esempio Python, il primo parametro è un evento proxy Lambda e il secondo parametro è il contesto Lambda.

L’esempio seguente in Node.js mostra come filtrare i payload del progetto in base all’ID gruppo del progetto, come fatto in  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Stabilisci l&#39;ID gruppo che stai cercando e crealo come costante statica.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Il primo parametro è il proxy Lambda &quot;event&quot;, che contiene il messaggio di abbonamento all’evento e alcune informazioni aggiuntive da analizzare.\
   Il secondo parametro è il contesto dell&#39;attuale richiesta del proxy Lambda.\
   In questo esempio, l&#39;oggetto Context viene utilizzato per ottenere un logger Lambda, utilizzato per scrivere un messaggio su CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analizza il messaggio dall’evento.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Ottieni il projectGroupID dall&#39;attributo &quot;newState&quot; del messaggio di abbonamento all&#39;evento, quindi confrontalo con l&#39;ID gruppo del gruppo identificato al passaggio 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Per informazioni sul formato newState, vedi [Formato del messaggio in uscita per le sottoscrizioni di eventi](../../wf-api/api/message-format-event-subs.md).

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
   >È fondamentale restituire una risposta vuota e di successo. Qualsiasi elemento oltre a una risposta a 200 livelli è considerato una consegna non riuscita.

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

   L’SDK di AWS viene utilizzato per richiamare un altro Lambda, che è responsabile della consegna del messaggio filtrato all’endpoint desiderato.\
   Lo scopo di trasferire la responsabilità di consegnare il messaggio a un altro Lambda è quello di evitare un timeout della richiesta di consegna proveniente dal servizio di abbonamento agli eventi. Attualmente, il timeout per la consegna è impostato su cinque secondi. Se il filtro richiede più tempo di quanto consentito dall’impostazione , puoi elaborare la richiesta, ma il servizio di abbonamento agli eventi scadrà e passerà in un ciclo di tentativi fino a quando non riceverà una risposta a 200 livelli entro il periodo di timeout.\
   Per informazioni sulla gestione della consegna dei messaggi, consulta [Miglioramento Della Distribuzione Dei Messaggi Durante L&#39;Alloggio Dei Timeout](#improving-message-delivery-while-accommodating-timeouts).

## Miglioramento Della Distribuzione Dei Messaggi Durante L&#39;Alloggio Dei Timeout

Il servizio di abbonamento agli eventi ha un timeout rigoroso di **cinque secondi** per tutte le richieste di consegna. Nel caso in cui la consegna di un messaggio superi il tempo consentito, il servizio di abbonamento agli eventi avvia un ciclo di tentativi per quel messaggio.

Ad esempio, puoi creare un filtro ID gruppo di progetti simile a uno degli esempi disponibili in [Filtrare i messaggi evento](#filtering-event-messages) e includi una ricerca del database per determinare se il messaggio è necessario. È possibile che la ricerca del database insieme al tempo necessario per l&#39;elaborazione richiesta e per l&#39;avvio a freddo di Lambda possa richiedere più di cinque secondi, causando un nuovo tentativo del servizio di abbonamento agli eventi di consegnare il messaggio.

È possibile evitare un nuovo tentativo separando le parti del processo che richiedono molto tempo dalla logica responsabile per determinare se il messaggio deve essere elaborato e consegnato. In questo modo, puoi accettare il messaggio e inviare una risposta a 200 livelli al servizio di abbonamento agli eventi, mentre continui in modo asincrono a elaborare o filtrare il messaggio in background (vedi il passaggio 5 in [Java](#java) per un esempio).


Anche se l’elaborazione o il filtro non supera il timeout di cinque secondi, è comunque vantaggioso separare il primo punto di contatto del filtro o dell’elaborazione dei messaggi dagli altri passaggi di elaborazione o consegna sul lato client. In questo modo la consegna del messaggio alla destinazione dal servizio di abbonamento agli eventi ha un impatto minimo su tempo e prestazioni per entrambe le parti.

Per ulteriori informazioni sul meccanismo di esecuzione dei nuovi tentativi, consulta [Tentativi di abbonamento agli eventi](../../wf-api/api/event-sub-retries.md).

## Implementazione dei filtri in hosting nell’architettura senza cloud

Se non riesci a sfruttare un’architettura cloud per filtrare l’abbonamento agli eventi, puoi comunque utilizzare gli esempi in [Filtrare i messaggi evento](#filtering-event-messages) come roadmap su come implementare filtri o componenti di elaborazione personalizzati in hosting.

### Regolazione degli esempi di filtro per i servizi autonomi

Prima di utilizzare gli esempi di filtro in un ambiente senza cloud, procedi come segue:

* Ometti gli esempi specifici di Lambda, ad esempio il parametro Context.

* Modifica le chiamate di altri Lambdas negli esempi per effettuare richieste HTTP asincrone aggiuntive ad altri filtri o componenti di elaborazione che ospiti.

* Se fai riferimento agli esempi Python e Node.js, sostituisci il primo parametro evento con il primo parametro di payload mostrato nell’esempio Java. Vedere il passaggio 1 in [Java](#java).

* Distribuire i filtri o i processori con un’API basata sul Web.

### Impedire messaggi di abbonamento agli eventi persi

Talvolta, in un&#39;architettura senza nuvole, i servizi responsabili della ricezione dei messaggi di abbonamento agli eventi possono essere irraggiungibili. In questo caso, i messaggi potrebbero superare il limite di tentativi ed essere persi, senza alcun modo per recuperare le informazioni all’interno dei messaggi.

Durante l’avvio del servizio, si consiglia di implementare una query che richiede lo stato più recente di tutte le risorse che potrebbero essere state incluse nei messaggi persi. Come mostrato nell’esempio seguente, puoi utilizzare i criteri di filtro per eseguire una query per individuare le risorse che corrispondono a tali criteri ed elaborarne lo stato corrente.

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

Eseguendo una query delle risorse, assicurati che i sistemi di integrazione dispongano della versione più recente delle risorse.

### Implementazione dell’elaborazione asincrona nella distribuzione dei messaggi

Tutti gli esempi nel [Filtrare i messaggi evento](#filtering-event-messages) passa la responsabilità di inviare messaggi filtrati a un altro AWS Lambda. Questo viene fatto per evitare di superare il timeout di cinque secondi nella richiesta di consegna, che viene applicata dal servizio di abbonamento agli eventi che invia la richiesta.

In un’architettura senza cloud, potrebbe essere necessario implementare un meccanismo di elaborazione asincrona simile a come l’SDK di AWS consente le chiamate asincrone ad altri AWS Lambdas. La maggior parte dei linguaggi di programmazione moderni dispone di librerie di terze parti o di base che gestiscono l’elaborazione asincrona, consentendoti di sfruttare lo stile asincrono dell’elaborazione implementato nei nostri esempi.

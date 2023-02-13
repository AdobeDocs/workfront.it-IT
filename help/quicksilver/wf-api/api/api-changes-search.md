---
filename: api-changes-search
content-type: api
keywords: oggetto,stato,ricerca,best,pratica,risposta
navigation-topic: api-navigation-topic
title: '''Modifiche API di base: Risposte alla ricerca dello stato'
description: Modifiche nel modo in cui Workfront memorizza gli oggetti di stato.
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# Modifiche API di base: Risposte alla ricerca dello stato

Sono state apportate modifiche al modo in cui Workfront memorizza gli oggetti di stato. Queste modifiche non influiscono sulle modalità di esecuzione delle richieste di ricerca dello stato, ma influenzano la risposta restituita dalle richieste API che includono una ricerca di oggetti di stato restituendo un elenco incompleto di stati del gruppo.

## Best practice

Per recuperare in modo affidabile l’elenco completo degli stati disponibili per un gruppo, le seguenti richieste sono considerate best practice.

>[!NOTE]
>
>Queste strutture di richiesta sono consigliate per tutti gli utenti indipendentemente dal fatto che siano state apportate o meno le modifiche alla ricerca dello stato nel cluster.

Per lo stato del gruppo di progetto:

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Per Stato Gruppo Di Attività:

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Per Stato Gruppo Di Problemi:

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Tutti e tre questi endpoint accettano il **includeHidden=true** per recuperare gli stati nascosti di progetto/attività/problema di un determinato gruppo. Modellare le query di ricerca dello stato dopo questi esempi di best practice garantirà che tutte le informazioni sullo stato del gruppo siano incluse con ogni risposta.

Esempio di query di ricerca dello stato eseguita su un gruppo di attività che include uno stato bloccato a livello di sistema **Personalizzato_1** e uno stato sbloccato **Personalizzato_2**:

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

L’utilizzo di questo formato assicura che la risposta includa tutti i seguenti elementi:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Informazioni sulle modifiche apportate alla query di ricerca dello stato legacy

Nel sistema precedente, una query di ricerca dello stato copierebbe tutti gli stati del sistema disponibili per tutti i gruppi inclusi in una query. La risposta legacy includerebbe quindi tutti gli stati del sistema e gli stati a livello di gruppo disponibili per ciascun gruppo nella query.

Ad esempio, questa query (che non segue le best practice consigliate correnti):

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

La risposta seguente viene fornita nel sistema legacy, che include tutti gli stati dell’oggetto:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Tuttavia, in seguito agli aggiornamenti apportati al modo in cui gli stati vengono memorizzati e utilizzati, gli stati non vengono copiati per i gruppi e vengono ereditati da ciascun gruppo a livello di sistema. Di conseguenza, la query API di ricerca legge solo gli stati direttamente associati a un particolare gruppo, pertanto la risposta include gli stati bloccati e sbloccati del sistema, ma solo per i gruppi creati dopo l’aggiunta dello stato in questione.

Se non si utilizzano i metodi best practice aggiornati per eseguire query di ricerca dello stato dopo l’aggiornamento del sistema precedente, nella risposta verrà restituito un elenco incompleto degli stati del gruppo.

Ecco un esempio di ciò che restituisce questa struttura di richiesta obsoleta dopo l’aggiornamento del sistema legacy:

>**Esempio:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Tieni presente che questa risposta include solo gli stati specifici del gruppo e lascia fuori gli stati dichiarati a livello di sistema:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```

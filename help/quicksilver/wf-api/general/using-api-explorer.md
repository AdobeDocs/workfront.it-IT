---
content-type: api
navigation-topic: general-api
title: Utilizzo di API Explorer
description: Utilizzo di API Explorer
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---


# Utilizzo di API Explorer

Quando utilizzi l’API core di Adobe Workfront, API Explorer è uno strumento di riferimento legacy che cataloga le relazioni tra risorse, parametri e variabili supportati.

## Accedi a API Explorer:

1. Utilizza un browser Web per passare a [API Explorer](https://developer.adobe.com/workfront/api-explorer/)\
   ![Passare a API Explorer](assets/mceclip1-350x149.png)

1. In alto a destra in API Explorer, seleziona la **versione API** di Workfront desiderata; per impostazione predefinita, viene selezionata automaticamente la versione più recente
1. Il campo **Filtro**, può essere utilizzato per filtrare gli oggetti elencati per nome e tronca l&#39;elenco di oggetti visualizzato di conseguenza:

   ![Campi API Explorer](assets/mceclip2-350x147.png)

   * **Campi**: campi disponibili nell&#39;oggetto specificato.
   * **Riferimenti**: variabili di riferimento disponibili per l&#39;oggetto specificato. Un riferimento è un alias per una variabile. Una volta inizializzato, un riferimento può essere utilizzato in modo intercambiabile con il nome della variabile. Un riferimento utilizza la memoria inizializzata.
   * **Raccolte**: raccolte disponibili per l&#39;oggetto. Le raccolte sono variabili che rappresentano una relazione uno-a-molti tra l’oggetto e la risorsa.
   * **Ricerca**: risorse di ricerca disponibili per l&#39;oggetto. I risultati di una ricerca si basano sui parametri di query specificati dalla risorsa di ricerca nella richiesta API.
   * **Azioni**: azioni supportate per l&#39;oggetto. Le azioni possono essere procedure semplici o complesse che vengono eseguite su una risorsa o un set di risorse. Una determinata azione può influire anche sulle risorse correlate.

1. Apri una scheda, quindi fai clic sull’ID oggetto per visualizzare le variabili applicabili.\
   ![Visualizza variabili](assets/approval-350x89.png)\
   A seconda dell’oggetto selezionato, possono essere applicate le seguenti variabili:

   | Variabile | Definizione |
   |---|---|
   | Nome Campo | Nome di un campo utilizzato in un’operazione all’interno dell’API Workfront. |
   | Tipo di campo | Tipo di valori che è possibile immettere in un campo specifico di una tabella dati. I possibili valori del tipo di campo includono string, double, int, dateTime. |
   | Tipo enumerato | Il tipo di valori che possono essere utilizzati per identificare un tipo di dati. |
   | Valori possibili | Valori accettabili per l&#39;oggetto. |
   | Tipo di attributo ObjCode | Attributi che possono essere utilizzati per modificare la classe oggetto. |
   | URL | Percorso di ingresso che consente all’app di comunicare con l’API Workfront. |
   | Argomenti | Le variabili dell&#39;oggetto che possono essere passate tra l&#39;applicazione e Workfront. |
   | Tipo di risultato | Tipi di dati consentiti che possono essere restituiti da un metodo. |

---
content-type: api
navigation-topic: general-api
title: Utilizzo di API Explorer
description: Utilizzo di API Explorer
author: John
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---


# Utilizzo di API Explorer

Quando utilizzi l’API core di Adobe Workfront, API Explorer è uno strumento di riferimento legacy che cataloga le relazioni tra risorse, parametri e variabili supportate.

## Accedi a API Explorer:

1. Utilizza un browser web per passare alla [Esplora API](https://one.workfront.com/s/api-explorer)\
   ![](assets/mceclip1-350x149.png)

1. In alto a destra di API Explorer, seleziona la cartella di lavoro desiderata **Versione API**, per impostazione predefinita viene selezionata automaticamente la versione più recente
1. La **Filtro** può essere utilizzato per filtrare gli oggetti elencati per nome e troncherà l’elenco degli oggetti visualizzati di conseguenza:

   ![](assets/mceclip2-350x147.png)

   * **Campi**: Campi disponibili all’interno dell’oggetto specificato.
   * **Riferimenti**: Variabili di riferimento disponibili per l&#39;oggetto specificato. Un riferimento è un alias per una variabile. Una volta inizializzato, un riferimento può essere utilizzato in modo intercambiabile con il nome della variabile. Un riferimento utilizza la memoria inizializzata.
   * **Raccolte**: Raccolte disponibili per l’oggetto. Le raccolte sono variabili che rappresentano una relazione uno-a-molti tra l’oggetto e la risorsa.
   * **Ricerca**: Risorse di ricerca disponibili per l’oggetto. I risultati di una ricerca si basano sui parametri di query specificati dalla risorsa di ricerca nella richiesta API.
   * **Azioni**: Azioni supportate per l’oggetto. Le azioni possono essere procedure semplici o complesse che vengono eseguite su una risorsa o su un insieme di risorse. Una determinata azione può anche incidere sulle risorse correlate.

1. Apri una scheda , quindi fai clic sull’ID oggetto per visualizzare le variabili applicabili.\
   ![](assets/approval-350x89.png)\
   A seconda dell’oggetto selezionato, possono essere applicabili le seguenti variabili:

   | Variabile | Definizione |
   |---|---|
   | Nome Campo | Nome di un campo utilizzato in un’operazione all’interno dell’API Workfront. |
   | Tipo di campo | Tipo di valori che è possibile immettere in un campo specifico di una tabella di dati. I valori dei tipi di campo possibili includono stringa, doppio, int, dateTime. |
   | Tipo enumerato | Il tipo di valori che può essere utilizzato per identificare un tipo di dati. |
   | Valori possibili | Valori accettabili per l’oggetto. |
   | Tipo di attributo ObjCode | Attributi che possono essere utilizzati per modificare la classe oggetto. |
   | URL | Percorso di ingresso che consente all’app di comunicare con l’API Workfront. |
   | Argomenti | Le variabili dell&#39;oggetto che possono essere trasmesse tra l&#39;applicazione e Workfront. |
   | Tipo di risultato | Tipi di dati consentiti che possono essere restituiti da un metodo . |

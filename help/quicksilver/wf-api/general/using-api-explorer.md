---
content-type: api
navigation-topic: general-api
title: Utilizzo di API Explorer
description: Utilizzo di API Explorer
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
TQID: https://experienceleague.adobe.com/Y-qv5r6ygRA-V7mQSM3wzjaOt58myb64Vxa7UZGsAVo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 368
ht-degree: 100%

---

# Utilizzo di API Explorer

Quando utilizzi l’API core di Adobe Workfront, API Explorer è uno strumento di riferimento legacy che cataloga le relazioni tra risorse, parametri e variabili supportati.

## Accedi ad API Explorer:

1. Utilizzare un browser web per accedere ad [API Explorer](https://developer.adobe.com/workfront/api-explorer/)\
   ![Accedere ad API Explorer](assets/mceclip1-350x149.png)

1. In alto a destra in API Explorer, selezionare la **versione API** di Workfront desiderata; per impostazione predefinita, viene selezionata automaticamente la versione più recente
1. Il campo **Filtro**, può essere utilizzato per filtrare gli oggetti elencati per nome e troncherà l’elenco di oggetti visualizzato di conseguenza:

   ![Campi API Explorer](assets/mceclip2-350x147.png)

   * **Campi**: campi disponibili nell’oggetto specificato.
   * **Riferimenti**: variabili di riferimento disponibili per l’oggetto specificato. Un riferimento è un alias di una variabile. Una volta inizializzato, un riferimento può essere utilizzato in modo intercambiabile con il nome della variabile. Un riferimento utilizza la memoria inizializzata.
   * **Raccolte**: raccolte disponibili per l’oggetto. Le raccolte sono variabili che rappresentano una relazione di tipo uno a molti tra l’oggetto e la risorsa.
   * **Ricerca**: risorse di ricerca disponibili per l’oggetto. I risultati di una ricerca sono basati sui parametri di query specificati dalla risorsa di ricerca nella richiesta API.
   * **Azioni**: azioni supportate per l’oggetto. Le azioni possono essere procedure semplici o complesse che vengono eseguite su una risorsa o un set di risorse. Una determinata azione può influire anche sulle risorse correlate.

1. Apri una scheda, quindi fai clic sull’ID oggetto per visualizzare le variabili applicabili.\
   ![Visualizzare le variabili](assets/approval-350x89.png)\
   A seconda dell’oggetto selezionato, possono essere applicate le seguenti variabili:

   | Variabile | Definizione |
   |---|---|
   | Nome campo | Nome di un campo utilizzato in un’operazione all’interno dell’API Workfront. |
   | Tipo di campo | Tipo di valori che è possibile inserire in un campo specifico di una tabella dati. I possibili valori del tipo di campo includono string, double, int, dateTime. |
   | Tipo enumerato | Il tipo di valori che possono essere utilizzati per identificare un tipo di dati. |
   | Valori possibili | Valori accettabili per l’oggetto. |
   | Tipo di attributo ObjCode | Attributi che possono essere utilizzati per modificare la classe dell’oggetto. |
   | URL | Percorso di ingresso che consente all’app di comunicare con l’API Workfront. |
   | Argomenti | Le variabili dell’oggetto che possono essere trasmesse tra l’applicazione e Workfront. |
   | Tipo di risultato: | Tipi di dati consentiti che possono essere restituiti da un metodo. |

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Esegui un’azione personalizzata
description: Esegui un’azione personalizzata
author: John
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# Esegui un’azione personalizzata (non ancora implementata)

Questo endpoint consente a un utente Adobe Workfront (o a un evento di flusso di lavoro automatizzato) di eseguire un&#39;azione nel sistema esterno. L&#39;endpoint /customAction accetta un parametro &quot;name&quot;, che consente al provider webhook di implementare più operazioni personalizzate.

Il provider webhook registra azioni personalizzate con Workfront includendo le azioni nella risposta /serviceInfo in customActions. Workfront carica questo elenco durante la configurazione o l’aggiornamento del provider di webhook in Configurazione > Documenti > Integrazioni personalizzate.

Gli utenti possono attivare l&#39;azione personalizzata selezionando la sezione in &quot;Azioni documento&quot;

**URL**

GET /customAction

## Parametri query

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>Identificatore che specifica il tipo di azione da eseguire. Questo valore corrisponde a uno dei valori customAction elencati restituiti dall’endpoint /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>ID del documento anteriore per il quale viene eseguita l'azione.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> ID versione del documento di lavoro per il quale viene eseguita l'azione.</td> 
  </tr> 
 </tbody> 
</table>

 

## risposta

Una stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito. In caso di errore (ovvero stato = &quot;errore&quot;), Workfront visualizza all’utente il messaggio di errore fornito.

**Esempio:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: “success”
}
```

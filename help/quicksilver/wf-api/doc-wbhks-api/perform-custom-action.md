---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Eseguire un’azione personalizzata
description: Eseguire un’azione personalizzata
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 2%

---


# Eseguire un’azione personalizzata (non ancora implementata)

Questo endpoint consente a un utente di Adobe Workfront (o a un evento di flusso di lavoro automatizzato) di eseguire un’azione nel sistema esterno. L’endpoint /customAction accetta un parametro &quot;name&quot; che consente al provider del webhook di implementare più operazioni personalizzate.

Il provider webhook registra le azioni personalizzate con Workfront includendo le azioni nella risposta /serviceInfo in customActions. Workfront carica questo elenco durante la configurazione o l’aggiornamento del provider del webhook in Configurazione > Documenti > Integrazioni personalizzate.

Gli utenti possono attivare l’azione personalizzata selezionando la sezione in &quot;Azioni documento&quot;

**URL**

GET /customAction

## Parametri di query

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
   <td> <p>Identificatore che specifica il tipo di azione da eseguire. Questo valore corrisponde a uno dei valori customAction elencati restituiti dall'endpoint /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>ID del documento Workfront per il quale viene eseguita l'azione.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> ID versione del documento Workfront per cui viene eseguita l'azione.</td> 
  </tr> 
 </tbody> 
</table>

 

## Risposta

Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito. In caso di errore (ossia stato = &quot;errore&quot;), Workfront visualizzerà il messaggio di errore fornito all’utente.

**Esempio:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

risposta

```
{
status: "success"
}
```

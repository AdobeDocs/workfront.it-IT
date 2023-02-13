---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]
description: Quando configuri una chiamata API in un modulo, devi compilare il campo per il metodo di richiesta HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]

Quando configuri una chiamata API in un modulo, devi compilare il campo per il metodo di richiesta HTTP.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Metodi HTTP

Utilizza uno dei seguenti metodi HTTP.

* **[!UICONTROL GET]**: Recupera i dati da un server web in base ai parametri. [!UICONTROL GET] richiede una rappresentazione della risorsa specificata e riceve un [!UICONTROL 200 OK] messaggio di risposta con il contenuto richiesto in caso di esito positivo.
* **[!UICONTROL POST]**: Invia dati a un server web in base ai parametri. [!UICONTROL POST] Le richieste includono azioni come il caricamento di un file. Multipli [!UICONTROL POST]s può comportare un risultato diverso rispetto a un singolo [!UICONTROL POST], quindi fai attenzione a inviare involontariamente più [!UICONTROL POST]s. Se [!UICONTROL POST] ha esito positivo, riceverai un [!UICONTROL 200 OK] messaggio di risposta.
* **[!UICONTROL PUT]**: Invia dati a una posizione nel server web in base ai parametri. [!UICONTROL PUT] Le richieste includono azioni come il caricamento di un file. Differenza tra [!UICONTROL PUT] e [!UICONTROL POST] è che PUT è ideale, il che significa che il risultato di un singolo successo [!UICONTROL PUT] è uguale a molti identici [!UICONTROL PUT]s. Se un PUT ha esito positivo, riceverai un messaggio di risposta di 200 (in genere 201 o 204).
* **[!UICONTROL PATCH]**: (Non disponibile per alcuni moduli di chiamata API) Applica modifiche parziali a una risorsa su un server web in base ai parametri. [!UICONTROL PATCH] non è idempotente, il che significa che il risultato di più [!UICONTROL PATCH]Le conseguenze potrebbero essere indesiderate. Se [!UICONTROL PATCH] In caso di esito positivo, riceverai un messaggio di risposta di 200 (in genere 204).
* **[!UICONTROL DELETE]**: Elimina la risorsa specificata dal server web in base ai parametri (se la risorsa esiste). Se [!UICONTROL DELETE] Se la risposta è corretta, riceverai un messaggio di risposta di 200 OK.

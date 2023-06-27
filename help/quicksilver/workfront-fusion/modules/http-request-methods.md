---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]
description: Quando configuri una chiamata API in un modulo, devi compilare il campo per il metodo di richiesta HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Metodi HTTP

Utilizza uno dei seguenti metodi HTTP.

* **[!UICONTROL GET]**: recupera dati da un server web in base ai parametri. [!UICONTROL GET] richiede una rappresentazione della risorsa specificata e riceve un [!UICONTROL 200 OK] messaggio di risposta con il contenuto richiesto, in caso di esito positivo.
* **[!UICONTROL POST]**: invia dati a un server web in base ai parametri. [!UICONTROL POST] Le richieste includono azioni come il caricamento di un file. Più [!UICONTROL POST]s può portare a un risultato diverso rispetto a un singolo [!UICONTROL POST], pertanto occorre prestare attenzione all&#39;invio involontario di più [!UICONTROL POST]s. Se un [!UICONTROL POST] è stato completato, si riceve un [!UICONTROL 200 OK] messaggio di risposta.
* **[!UICONTROL PUT]**: invia i dati a una posizione nel server web in base ai parametri. [!UICONTROL PUT] Le richieste includono azioni come il caricamento di un file. La differenza tra [!UICONTROL PUT] e [!UICONTROL POST] è che il PUT è idempotente, il che significa che il risultato di un singolo successo [!UICONTROL PUT] è uguale a molti identici [!UICONTROL PUT]s. In caso di esito positivo di un PUT, viene visualizzato un messaggio di risposta 200 (in genere 201 o 204).
* **[!UICONTROL PATCH]**: (non disponibile per alcuni moduli di chiamata API) Applica modifiche parziali a una risorsa su un server web in base ai parametri. [!UICONTROL PATCH] non è idempotente, il che significa che il risultato [!UICONTROL PATCH]Potrebbero esserci conseguenze indesiderate. Se un [!UICONTROL PATCH] Se l&#39;operazione ha esito positivo, riceverai un messaggio di risposta 200 (in genere 204).
* **[!UICONTROL DELETE]**: elimina la risorsa specificata dal server web in base ai parametri (se la risorsa esiste). Se un [!UICONTROL DELETE] Se l&#39;operazione ha esito positivo, viene visualizzato il messaggio di risposta 200 OK.

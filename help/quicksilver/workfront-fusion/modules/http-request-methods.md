---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Metodi di richiesta HTTP](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Metodi HTTP

Utilizza uno dei seguenti metodi HTTP.

* **[!UICONTROL GET]**: recupera i dati da un server Web in base ai parametri. [!UICONTROL GET] richiede una rappresentazione della risorsa specificata e, in caso di esito positivo, riceve un messaggio di risposta [!UICONTROL 200 OK] con il contenuto richiesto.
* **[!UICONTROL POST]**: invia dati a un server Web in base ai parametri. Le richieste di [!UICONTROL POST] includono azioni come il caricamento di un file. Più [!UICONTROL POST]s possono produrre un risultato diverso rispetto a un singolo [!UICONTROL POST]. Prestare quindi attenzione all&#39;invio involontario di più [!UICONTROL POST]s. Se un [!UICONTROL POST] ha esito positivo, verrà visualizzato un messaggio di risposta [!UICONTROL 200 OK].
* **[!UICONTROL PUT]**: invia dati a una posizione nel server Web in base ai parametri. Le richieste di [!UICONTROL PUT] includono azioni come il caricamento di un file. La differenza tra [!UICONTROL PUT] e [!UICONTROL POST] è che PUT è idempotente, il che significa che il risultato di un singolo [!UICONTROL PUT] riuscito è lo stesso di molti [!UICONTROL PUT] identici. In caso di esito positivo di un PUT, riceverai un messaggio di risposta 200 (in genere 201 o 204).
* **[!UICONTROL PATCH]**: (non disponibile per alcuni moduli di chiamata API) Applica modifiche parziali a una risorsa su un server Web in base ai parametri. [!UICONTROL PATCH] non è idempotente, il che significa che il risultato di più [!UICONTROL PATCH] potrebbe avere conseguenze indesiderate. Se un [!UICONTROL PATCH] ha esito positivo, riceverai un messaggio di risposta di 200 (in genere 204).
* **[!UICONTROL DELETE]**: elimina la risorsa specificata dal server Web in base ai parametri (se la risorsa esiste). Se un [!UICONTROL DELETE] ha esito positivo, viene visualizzato un messaggio di risposta di 200 OK.

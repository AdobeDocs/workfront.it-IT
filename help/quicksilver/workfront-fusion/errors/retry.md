---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Riprova la gestione degli errori in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Riprova la gestione degli errori in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Configura `retry` soluzione alternativa per la gestione degli errori](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/retry.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In alcuni casi è utile rieseguire un modulo non riuscito se è possibile che il motivo dell’errore passi nel tempo.

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

## Soluzioni per la direttiva di gestione degli errori [!UICONTROL Riprova]

[!UICONTROL Adobe Workfront Fusion] al momento non offre la direttiva di gestione degli errori [!UICONTROL Riprova], anche se è possibile utilizzare due soluzioni alternative per imitarne la funzionalità. Per ulteriori informazioni, vedere [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilizza la direttiva [!UICONTROL Break]

1. Nel pannello delle impostazioni dello scenario, abilita l&#39;opzione **[!UICONTROL Consenti archiviazione esecuzioni incomplete]**.

   Per ulteriori informazioni, vedere [Pannello impostazioni scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Allegare al modulo una route del gestore degli errori, come descritto in [Gestione degli errori in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Collega la direttiva [!UICONTROL Break] alla route del gestore degli errori e configurala.

   Per ulteriori informazioni, vedere [Direttive per la gestione degli errori in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Svantaggi

* L&#39;intervallo minimo tra i tentativi è di un minuto.
* Se il modulo elabora più bundle e l&#39;elaborazione di un bundle non riesce, l&#39;esecuzione parziale (solo il bundle che ha causato l&#39;errore) viene spostata nella cartella esecuzioni incomplete e pianificata per i nuovi tentativi in base alle impostazioni della direttiva [!UICONTROL Break]. Tuttavia, l’esecuzione corrente continua e il modulo continua a elaborare i bundle successivi. È possibile abilitare l&#39;opzione &quot;[!UICONTROL Elaborazione sequenziale]&quot; nelle [!UICONTROL Impostazioni scenario] per impedire che lo scenario venga eseguito nuovamente finché l&#39;esecuzione archiviata nella cartella Esecuzioni incomplete non viene risolta correttamente.

  Per ulteriori informazioni sulle esecuzioni incomplete, vedere [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilizza il modulo [!UICONTROL Repeater]

1. Impiega il modulo **[!UICONTROL Repeater]** e imposta il campo **[!UICONTROL Repeats]** sul numero massimo di tentativi.
1. Collegare il modulo che potrebbe non riuscire al modulo **[!UICONTROL Repeater]**.
1. Allegare al modulo una route di gestore degli errori (vedere [Gestione degli errori in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Collega il modulo **[!UICONTROL Strumenti] > [!UICONTROL Sospendi]** alla route del gestore errori e imposta il campo **[!UICONTROL Ritarda]** sul numero di secondi tra i tentativi.

1. Collega la direttiva **[!UICONTROL Ignora]** dopo il modulo **[!UICONTROL Strumenti] > [!UICONTROL Sospendi]** (consulta [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Collega il modulo **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** dopo il modulo che potrebbe non riuscire e configuralo per memorizzare il risultato del modulo in una variabile denominata, ad esempio `Result`.

1. Collega il modulo **[!UICONTROL Array aggregator]** dopo **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** e scegli il modulo **[!DNL Repeater]** nel campo Modulo Source.

1. Collegare il modulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** al modulo **[!UICONTROL Array aggregator]** e configurarlo per ottenere il valore della variabile `Result`.

1. Inserire il modulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** tra il modulo **[!UICONTROL Repeater]** e il modulo che potrebbe non riuscire e configurarlo per ottenere il valore della variabile `Result`.

1. Inserire un filtro tra il modulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** e il modulo che potrebbe non riuscire per continuare solo se la variabile `Result` non esiste.

>[!INFO]
>
>**Esempio:** Questo è uno scenario di esempio in cui il modulo [!UICONTROL HTTP] >[!UICONTROL Effettua una richiesta] rappresenta il modulo che potrebbe non riuscire:
>
>![](assets/http-make-request-350x116.png)
>
>Se il risultato del modulo con potenziale errore è troppo complesso per essere memorizzato in una variabile semplice, puoi utilizzare un archivio dati per memorizzare/recuperare il risultato. L’archivio dati conterrebbe un solo record. La chiave del record può essere ad esempio `Result`.
>
>Per ulteriori informazioni sugli archivi dati, vedere [Archivi dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Restituzione

Questa soluzione alternativa potrebbe apparire un po&#39; troppo complessa e risulta anche più impegnativa in termini di operazioni.

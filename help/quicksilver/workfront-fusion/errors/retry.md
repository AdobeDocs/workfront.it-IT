---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione degli errori dei tentativi in [!DNL Adobe Workfront Fusion]
description: In alcuni casi è utile rieseguire un modulo non riuscito per un paio di volte, se esiste la possibilità che il motivo dell’errore passi nel tempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Gestione degli errori dei tentativi in [!DNL Adobe Workfront Fusion]

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

## Soluzioni per il [!UICONTROL Riprova] direttiva sulla gestione degli errori

[!UICONTROL Adobe Workfront Fusion] attualmente non offre [!UICONTROL Riprova] direttiva sulla gestione degli errori, anche se è possibile utilizzare due soluzioni alternative per imitarne la funzionalità. Per ulteriori informazioni, consulta [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilizza il [!UICONTROL Interrompi] direttiva

1. Nel pannello delle impostazioni dello scenario, abilita **[!UICONTROL Consenti archiviazione esecuzioni incomplete]** opzione.

   Per ulteriori informazioni, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Allegare al modulo una route di gestore degli errori, come descritto in [Gestione degli errori in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Collega [!UICONTROL Interrompi] direttiva alla route del gestore degli errori e configurala.

   Per ulteriori informazioni, consulta [Direttive per la gestione degli errori in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Svantaggi

* L&#39;intervallo minimo tra i tentativi è di un minuto.
* Se il modulo elabora più bundle e l’elaborazione di un bundle non riesce, l’esecuzione parziale (solo il bundle che ha causato l’errore) viene spostata nella cartella esecuzioni incomplete e pianificata per i nuovi tentativi in base al [!UICONTROL Interrompi] impostazioni delle direttive. Tuttavia, l’esecuzione corrente continua e il modulo continua a elaborare i bundle successivi. Puoi abilitare &quot;[!UICONTROL Elaborazione sequenziale]Opzione &quot; in [!UICONTROL Impostazioni scenario] per impedire che lo scenario venga eseguito nuovamente finché l’esecuzione memorizzata nella cartella Esecuzioni incomplete non è stata risolta correttamente.

  Per ulteriori informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilizza il [!UICONTROL Ripetitore] modulo

1. Impiegare **[!UICONTROL Ripetitore]** e impostarne il **[!UICONTROL Si ripete]** al numero massimo di tentativi.
1. Collega il modulo con potenziale errore al **[!UICONTROL Ripetitore]** modulo.
1. Allega un percorso di handler degli errori a questo modulo (vedi [Gestione degli errori in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Sospendi]** al ciclo di lavorazione del gestore degli errori e impostarne **[!UICONTROL Ritardo]** al numero di secondi tra i tentativi.

1. Collega **[!UICONTROL Ignora]** direttiva dopo il **[!UICONTROL Strumenti] > [!UICONTROL Sospendi]** modulo (vedere [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** dopo il modulo che potrebbe generare un errore e configurarlo per memorizzare il risultato del modulo in una variabile denominata, ad esempio, `Result`.

1. Collega **[!UICONTROL Aggregatore array]** modulo dopo il **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** e scegli la **[!DNL Repeater]** nel campo del modulo di origine.

1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** al modulo **[!UICONTROL Aggregatore array]** e configurarlo per ottenere il valore del `Result` variabile.

1. Inserisci il **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** modulo tra **[!UICONTROL Ripetitore]** modulo e il modulo che potrebbe generare un errore e configurarlo per ottenere il valore del `Result` variabile.

1. Inserisci un filtro tra questi **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** e il modulo che potrebbe non riuscire a continuare solo se `Result` la variabile non esiste.

>[!INFO]
>
>**Esempio:** Ecco uno scenario di esempio in cui [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] Il modulo rappresenta il modulo che potrebbe generare errori:
>
>![](assets/http-make-request-350x116.png)
>
>Se il risultato del modulo con potenziale errore è troppo complesso per essere memorizzato in una variabile semplice, puoi utilizzare un archivio dati per memorizzare/recuperare il risultato. L’archivio dati conterrebbe un solo record. La chiave del record può essere, ad esempio, `Result`.
>
>Per ulteriori informazioni sugli archivi dati, consulta [Archivi dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Restituzione

Questa soluzione alternativa potrebbe apparire un po&#39; troppo complessa e risulta anche più impegnativa in termini di operazioni.

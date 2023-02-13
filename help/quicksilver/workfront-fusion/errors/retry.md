---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Riprova la gestione degli errori in [!DNL Adobe Workfront Fusion]
description: In alcuni casi è utile ripetere l’esecuzione di un modulo non riuscito per un paio di volte, se esiste la possibilità che il motivo dell’errore possa passare nel tempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Riprova la gestione degli errori in [!DNL Adobe Workfront Fusion]

In alcuni casi è utile ripetere l’esecuzione di un modulo non riuscito se esiste la possibilità che il motivo dell’errore possa passare nel tempo.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Soluzioni per [!UICONTROL Riprova] direttiva sulla gestione degli errori

[!UICONTROL Adobe Workfront Fusion] attualmente non offre [!UICONTROL Riprova] direttiva sulla gestione degli errori, anche se è possibile utilizzare due soluzioni alternative per imitarne la funzionalità. Per ulteriori informazioni, consulta [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilizza la [!UICONTROL Interruzione] direttiva

1. Nel pannello delle impostazioni dello scenario, abilita **[!UICONTROL Consenti archiviazione esecuzioni incomplete]** opzione .

   Per ulteriori informazioni, consulta [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Allega una route del gestore errori al modulo, come descritto in [Gestione degli errori in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Collega [!UICONTROL Interruzione] alla route del gestore di errori e configurala.

   Per ulteriori informazioni, consulta [Direttive sulla gestione degli errori [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Svantaggi

* L&#39;intervallo minimo di esecuzione dei tentativi è di un minuto.
* Se il modulo elabora più bundle e l&#39;elaborazione di un bundle non riesce, l&#39;esecuzione parziale (solo il bundle che ha causato l&#39;errore) viene spostata nella cartella esecuzioni incomplete e pianificata per i nuovi tentativi in base al [!UICONTROL Interruzione] impostazioni della direttiva. Tuttavia, l’esecuzione corrente continua e il modulo continua a elaborare i bundle successivi. Puoi abilitare il &quot;[!UICONTROL Elaborazione sequenziale]&quot; nella [!UICONTROL Impostazioni dello scenario] per evitare che lo scenario venga nuovamente eseguito finché l’esecuzione memorizzata nella cartella esecuzioni incomplete non è stata risolta correttamente.

Per ulteriori informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilizza la [!UICONTROL Ripetitore] modulo

1. Implementare **[!UICONTROL Ripetitore]** modulo e impostarne il [!UICONTROL Ripeti] al numero massimo di tentativi.
1. Collega il modulo potenzialmente non funzionante al **[!UICONTROL Ripetitore]** modulo .
1. Allega una route del gestore errori a questo modulo (vedi [Gestione degli errori in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Sonno]** modulo alla route del gestore di errori e impostarne la **[!UICONTROL Ritardo]** al numero di secondi tra i tentativi.

1. Collega **[!UICONTROL Ignora]** direttiva successiva **[!UICONTROL Strumenti] > [!UICONTROL Sonno]** modulo (vedi [Direttive per la gestione degli errori in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** modulo dopo il modulo potenzialmente non riuscito e configuralo per memorizzare il risultato del modulo in una variabile denominata, ad esempio, `Result`.

1. Collega **[!UICONTROL Aggregatore array]** modulo dopo **[!UICONTROL Strumenti] > [!UICONTROL Imposta variabile]** e scegli la **[!DNL Repeater]** modulo nel relativo campo modulo di origine.

1. Collega **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** al **[!UICONTROL Aggregatore array]** e configuralo per ottenere il valore del `Result` variabile.

1. Inserisci **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** tra **[!UICONTROL Ripetitore]** il modulo e il modulo potenzialmente difettoso e configurarlo ottengono il valore del `Result` variabile.

1. Inserisci un filtro tra questi **[!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]** il modulo e il modulo potenzialmente in errore continuano solo se `Result` variabile inesistente.

>[!INFO]
>
>**Esempio:** Di seguito è riportato uno scenario di esempio in cui la variabile [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] il modulo rappresenta il modulo potenzialmente in errore:
>
>![](assets/http-make-request-350x116.png)
>
>Se il risultato del modulo potenzialmente difettoso è troppo complesso per essere memorizzato in una variabile semplice, è possibile utilizzare un archivio dati per memorizzare/recuperare il risultato. L&#39;archivio dati conterrebbe un solo record. La chiave del record può essere, ad esempio, `Result`.
>
>Per ulteriori informazioni sugli archivi dati, consulta [Archivia dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Ritorno

Questa soluzione potrebbe apparire un po&#39; troppo complessa ed è anche più impegnativa in termini di operazioni.

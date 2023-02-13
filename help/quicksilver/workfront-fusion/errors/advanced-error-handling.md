---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione avanzata degli errori in [!DNL Adobe] Workfront Fusion
description: Le tecniche avanzate di gestione degli errori includono il filtro e la nidificazione.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Gestione avanzata degli errori in [!DNL Adobe Workfront Fusion]

Le tecniche avanzate di gestione degli errori includono il filtro e la nidificazione.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
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

## Filtro

Esistono due tipi di filtro che possono verificarsi su un percorso del gestore di errori.

* [Aggiunta di un filtro alla route del gestore di errori](#adding-a-filter-to-the-error-handler-route)
* [Aggiunta di un router seguito da filtri alla route del gestore errori](#adding-a-router-followed-by-filters-to-the-error-handler)

### Aggiunta di un filtro alla route del gestore di errori

È possibile utilizzare un filtro per controllare quali errori vengono gestiti dalla route del gestore errori. Questo consente di elaborare solo tipi specifici di errori. Se un errore non passa attraverso il filtro, viene trattato come se non ci fosse una route del gestore errori definita per il modulo specificato.

>[!INFO]
>
>**Esempio:**
>
>![](assets/filter-error-handling-350x238.png)

### Aggiunta di un [!UICONTROL Router] seguiti da filtri per il gestore degli errori

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>In questo esempio, l’errore si verifica nella [!UICONTROL Creare una cartella] modulo (A), che ha una rotta regolare e una route del gestore di errori. Quest&#39;ultimo è seguito da un router con una route con un filtro che definisce un tipo specifico di errore (Data Error Performed) e l&#39;altra che è la route predefinita per tutti gli altri errori. Il primo percorso termina con il [!UICONTROL Riprendi] direttiva che contiene valori sostitutivi dello scenario da riprendere dal modulo A ([!UICONTROL Creare una cartella]), mentre il secondo percorso termina con il [!UICONTROL Ripristino] direttiva che interrompe immediatamente l&#39;esecuzione dello scenario.

Vedi [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) per ulteriori informazioni sui vari tipi di errore e su come [!DNL Workfront Fusion] elabora e valuta tali processi.

### Scenario di esempio

Puoi impostare questa scena di esempio per comprendere come funzionano questi filtri per la gestione degli errori.

Utilizza un [!DNL Dropbox] per caricare un file anziché crearne uno nuovo

Se utilizzi [!UICONTROL Creare una cartella] modulo su [!DNL Dropbox] e esiste già una cartella con lo stesso nome, il modulo genera un errore di dati come mostrato di seguito:

![](assets/dropbox-350x276.png)

Lo scenario completo:

![](assets/dropbox-scenario-350x190.png)

1. La [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] il modulo contiene il nome della cartella
1. La [!UICONTROL HTTP] >[!UICONTROL Ottieni un file] il modulo recupera il file da caricare nella cartella
1. La [!UICONTROL Dropbox] >[!UICONTROL Creare una cartella] modulo genera un errore se esiste già una cartella con lo stesso nome di quella mappata nel modulo
1. La route del gestore errori (bolle trasparenti) contiene un router per filtrare gli errori
1. La prima route è per un tipo specifico di errore denominato Errore dati come già noto:

   1. Se si verifica un errore di dati e i dettagli dell’errore passano attraverso il filtro, la [!UICONTROL Dropbox] >[!UICONTROL Elencare tutti i file/sottocartelle in un modulo cartelle] elenca tutte le cartelle in [!DNL Dropbox]
   1. Il filtro successivo corrisponde ai nomi delle cartelle
   1. La [!UICONTROL Riprendi] La direttiva specifica l&#39;ID cartella e il percorso della cartella esistente e l&#39;esecuzione dello scenario riprende dalla [!UICONTROL Dropbox] >[!UICONTROL Creare una cartella] ma, invece di cercare di creare una nuova cartella, questa volta utilizza i valori del [!UICONTROL Riprendi] direttiva per passare al modulo successivo e caricare il file nella cartella esistente

1. Il secondo percorso è per tutti gli altri errori e termina con [!UICONTROL Ripristino] direttiva che comporta l&#39;arresto immediato dello scenario

Di seguito è riportata una spiegazione dettagliata della 5a dichiarazione:

Per utilizzare la cartella esistente nei moduli successivi ([!UICONTROL Caricare un file] di seguito), devi aggiungere una route del gestore errori al modulo e recuperare il percorso della cartella da mappare nel [!UICONTROL Riprendi] modulo direttiva che segue:

![](assets/add-error-handler-route-350x113.png)

Il filtro sulla prima route è impostato per gestire solo l&#39;errore specifico (Errore dati) visualizzato quando esiste già una cartella con lo stesso nome:

![](assets/condition-350x327.png)

La [!UICONTROL Dropbox] >[!UICONTROL Elencare tutti i file in una cartella] Il modulo è configurato per restituire tutte le cartelle presenti nella cartella di destinazione. Il filtro seguente passa solo a quello che stavamo cercando di creare originariamente (il nome della cartella è memorizzato in 33. Nome cartella):

![](assets/condition2-350x193.png)

Alla fine, il [!UICONTROL Riprendi] La direttiva fornisce il percorso della cartella come output per il modulo non riuscito. L&#39;ID cartella è stato lasciato vuoto poiché non è necessario per &quot;[!UICONTROL Caricare un file]Modulo &#39;:

![](assets/flow-control-350x190.png)

## Nidificazione

Indipendentemente dalla posizione di un modulo, è possibile creare e implementare percorsi del gestore errori su tutti i moduli, ad eccezione dei router. Quindi è possibile creare un percorso del gestore errori per un modulo che fa già parte di un percorso esistente del gestore errori creato per un altro modulo.

Ecco un esempio di percorso del gestore di errori nidificato:

![](assets/nested-error-handling-route-350x174.png)

In questo scenario, il secondo percorso del gestore di errori è nidificato sotto il primo percorso del gestore di errori. Quindi, se [!UICONTROL Dropbox] >[!UICONTROL Creazione di un modulo cartella] rileva un errore, l&#39;esecuzione si sposta sulla Route 1, se il [!UICONTROL Errore di dati] viene passato il filtro, il modulo successivo viene eseguito seguito da [!UICONTROL Riprendi] modulo direttiva se non si verifica un errore con [!UICONTROL Dropbox] >[!UICONTROL Elenca tutti i file/sottocartelle] in un modulo cartella.

Tuttavia, se si verifica un errore con questo [!DNL Dropbox] modulo , l&#39;esecuzione si sposta su Error Handler Route 2 e termina con [!UICONTROL Ignora] direttiva. La [!UICONTROL Riprendi direttiva] modulo non eseguito in questo caso.

Si tratta di una combinazione di gestori di filtri e nidificazione degli errori.


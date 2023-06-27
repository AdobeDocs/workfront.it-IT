---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione avanzata degli errori in [!DNL Adobe] Workfront Fusion
description: Le tecniche avanzate di gestione degli errori includono filtraggio e nidificazione.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Gestione avanzata degli errori in [!DNL Adobe Workfront Fusion]

Le tecniche avanzate di gestione degli errori includono filtraggio e nidificazione.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
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

## Filtro

Esistono due tipi di filtro che possono essere eseguiti su un percorso di gestore degli errori.

* [Aggiunta di un filtro alla route del gestore degli errori](#adding-a-filter-to-the-error-handler-route)
* [Aggiunta di un router seguito da filtri alla route del gestore errori](#adding-a-router-followed-by-filters-to-the-error-handler)

### Aggiunta di un filtro alla route del gestore degli errori

È possibile utilizzare un filtro per controllare gli errori gestiti dalla route del gestore degli errori. Questo consente di elaborare solo tipi specifici di errori. Se un errore non passa attraverso il filtro, verrà trattato come se non fosse stato definito alcun percorso del gestore degli errori per il modulo specificato.

>[!INFO]
>
>**Esempio:**
>
>![](assets/filter-error-handling-350x238.png)

### Aggiunta di un [!UICONTROL Router] seguito dai filtri al gestore degli errori

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>In questo esempio, l’errore si verifica in corrispondenza di [!UICONTROL Creare una cartella] il modulo (A), che dispone di un percorso regolare e di un percorso di gestione degli errori. Quest&#39;ultimo è seguito da un router con una route che ha un filtro che definisce un tipo specifico di errore (Data Error Takes Place), e l&#39;altra che è la route predefinita per tutti gli altri errori. Il primo percorso termina con [!UICONTROL Riprendi] direttiva contenente valori sostitutivi per lo scenario da riprendere dal modulo A ([!UICONTROL Creare una cartella]), mentre il secondo percorso termina con [!UICONTROL Rollback] direttiva che interrompe immediatamente l’esecuzione dello scenario.

Consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) per ulteriori informazioni sui vari tipi di errore e sulle modalità [!DNL Workfront Fusion] li elabora e li valuta.

### Lo scenario di esempio

Puoi impostare questa scena di esempio per comprendere come funzionano questi filtri per la gestione degli errori.

Usa un elemento esistente [!DNL Dropbox] cartella per caricare un file invece di crearne uno nuovo

Se si utilizza [!UICONTROL Creare una cartella] modulo su [!DNL Dropbox] e una cartella con lo stesso nome esiste già, il modulo genera un Errore di dati come mostrato di seguito:

![](assets/dropbox-350x276.png)

Lo scenario completo:

![](assets/dropbox-scenario-350x190.png)

1. Il [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] il modulo contiene il nome della cartella
1. Il [!UICONTROL HTTP] >[!UICONTROL Ottieni un file] Il modulo recupera il file da caricare nella cartella
1. Il [!UICONTROL Dropbox] >[!UICONTROL Creare una cartella] Il modulo genera un errore se esiste già una cartella con lo stesso nome di quella mappata nel modulo
1. La route del gestore degli errori (bolle trasparenti) contiene un router per filtrare gli errori
1. La prima route è per un tipo di errore specificato denominato Errore dati, in quanto ne sappiamo già:

   1. Se si verifica un errore di dati e i dettagli dell’errore passano attraverso il filtro, il [!UICONTROL Dropbox] >[!UICONTROL Elencare tutti i file/sottocartelle in un modulo cartella] elenca tutte le cartelle in [!DNL Dropbox]
   1. Il filtro successivo corrisponde ai nomi delle cartelle
   1. Il [!UICONTROL Riprendi] specifica l’ID cartella e il percorso della cartella esistente; l’esecuzione dello scenario riprende da [!UICONTROL Dropbox] >[!UICONTROL Creare una cartella] ma, invece di creare una nuova cartella, questa volta vengono utilizzati i valori del [!UICONTROL Riprendi] direttiva per passare al modulo successivo e caricare il file nella cartella esistente

1. La seconda route è per tutti gli altri errori e termina con [!UICONTROL Rollback] direttiva che comporta l&#39;immediata interruzione dello scenario

Di seguito una spiegazione dettagliata della quinta dichiarazione:

Per utilizzare la cartella esistente nei moduli successivi ([!UICONTROL Carica un file] di seguito), devi aggiungere al modulo una route del gestore degli errori e recuperare il percorso della cartella da mappare nel [!UICONTROL Riprendi] modulo di direttiva che segue:

![](assets/add-error-handler-route-350x113.png)

Il filtro della prima route è impostato per gestire solo l&#39;errore specifico (Errore dati) che viene visualizzato quando esiste già una cartella con lo stesso nome:

![](assets/condition-350x327.png)

Il [!UICONTROL Dropbox] >[!UICONTROL Elencare tutti i file in una cartella] è configurato per restituire tutte le cartelle nella cartella di destinazione. Il seguente filtro passa solo a quello che stavamo originariamente tentando di creare (il nome della cartella è memorizzato nel 33. Nome cartella (elemento):

![](assets/condition2-350x193.png)

Alla fine, il [!UICONTROL Riprendi] La direttiva fornisce il percorso della cartella come output per il modulo non riuscito. L’ID cartella è stato lasciato vuoto perché non è necessario in &quot;[!UICONTROL Carica un file]Modulo &#39;:

![](assets/flow-control-350x190.png)

## Nidificazione

Indipendentemente da dove si trova un modulo, è possibile creare e implementare route del gestore degli errori su tutti i moduli, ad eccezione dei router. È quindi possibile creare una route di gestore errori per un modulo che fa già parte di una route di gestore errori esistente creata per un altro modulo.

Di seguito è riportato un esempio di route del gestore degli errori nidificata:

![](assets/nested-error-handling-route-350x174.png)

In questo scenario, la seconda route del gestore errori è nidificata sotto la prima route del gestore errori. Quindi, se [!UICONTROL Dropbox] >[!UICONTROL Creare un modulo cartella] rileva un errore, l’esecuzione si sposta sulla Route 1, se [!UICONTROL Si verifica un errore di dati] viene passato, il modulo successivo viene eseguito seguito dal [!UICONTROL Riprendi] modulo direttiva se non si verifica un errore con il [!UICONTROL Dropbox] >[!UICONTROL Elenca tutti i file/sottocartelle] in un modulo cartella.

Tuttavia, se si verifica un errore con questo [!DNL Dropbox] , quindi l’esecuzione si sposta su Error Handler Route 2 e termina con [!UICONTROL Ignora] direttiva. Il [!UICONTROL Riprendi direttiva] Il modulo non viene eseguito in questo caso.

Combinazione di gestori di errori di filtro e nidificazione.


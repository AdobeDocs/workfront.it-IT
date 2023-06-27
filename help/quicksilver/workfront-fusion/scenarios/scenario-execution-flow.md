---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flusso di esecuzione dello scenario in Adobe Workfront Fusion
description: Questo articolo spiega come viene eseguito uno scenario e come i dati scorrono attraverso di esso. Vengono inoltre illustrate le aree in cui è possibile trovare informazioni sui dati elaborati e su come leggerle.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]

Questo articolo spiega come viene eseguito uno scenario e come i dati scorrono attraverso di esso. Vengono inoltre illustrate le aree in cui è possibile trovare informazioni sui dati elaborati e su come leggerle.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Flusso di esecuzione dello scenario

Dopo aver configurato correttamente e attivato uno scenario, questo viene eseguito in base alla pianificazione definita.

All’inizio dello scenario, il primo modulo risponde a un evento che è stato impostato per osservare. Se restituisce eventuali bundle (dati), questi passano al modulo successivo e lo scenario continua, passando i bundle attraverso ciascun modulo successivo, uno alla volta.

Se i bundle vengono elaborati correttamente in tutti i moduli, lo scenario viene contrassegnato come riuscito nell’area dei dettagli dello scenario, come spiegato in [Dettagli dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Per ulteriori informazioni sulla configurazione di uno scenario, consulta [Impostazioni dello scenario di base in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Per ulteriori informazioni sull’attivazione di uno scenario, consulta [Attivare o disattivare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Per ulteriori informazioni sulla pianificazione di uno scenario, consulta [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Per ulteriori informazioni sui moduli, consulta [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario che controlla le richieste in entrata in [!DNL Workfront] e quindi li converte in [!DNL Workfront] progetti, i dati scorrono come segue.
>
>Il primo passaggio dello scenario, eseguito dal primo modulo, consiste nel controllare le richieste. Ogni richiesta in entrata viene considerata un bundle. Se il modulo viene eseguito senza trovare bundle, lo scenario termina dopo il primo modulo.
>
>Se il primo modulo restituisce un bundle, il bundle passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall’ultimo modulo, che convertono la richiesta in un progetto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione e l&#39;integrazione del lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario da cui vengono scaricati i documenti [!DNL Adobe Workfront] e li invia a una cartella in [!DNL Dropbox], i dati scorrono come segue.
>
>Il primo passaggio dello scenario, eseguito dal primo modulo, consiste nel controllare i bundle (documenti). In questo esempio, il modulo controlla i bundle in [!DNL Workfront]. Se non restituisce un bundle, lo scenario termina dopo il primo modulo.
>
>Se viene restituito un bundle, questo passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall’ultimo modulo, che carica il bundle in [!DNL Dropbox] cartella.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Se il primo modulo restituisce più bundle, il primo bundle viene caricato in [!DNL Dropbox] prima del caricamento del secondo bundle. Poi viene caricato il secondo bundle, poi il terzo e così via.

## Informazioni sui bundle elaborati

Per ogni modulo, il bundle passa attraverso un processo in 4 fasi prima di passare al modulo successivo o di raggiungere la sua destinazione finale. Il processo in 4 fasi consiste in inizializzazione, operazione, commit/rollback e finalizzazione. Questa funzione è denominata elaborazione delle transazioni e aiuta a spiegare come sono stati elaborati i dati in un modulo.

Una volta completata l’esecuzione di uno scenario, ogni modulo visualizza un’icona che mostra il numero di operazioni eseguite. Puoi fare clic su questa icona per visualizzare le informazioni dettagliate sui bundle elaborati, nel formato descritto sopra. Puoi vedere quali impostazioni di moduli sono state utilizzate e quali bundle sono stati restituiti da quale modulo.

![](assets/info-processed-bundles-350x396.png)

Un modulo ha ricevuto informazioni di input quali:

* Immagine convertita
* Cartella selezionata in cui caricare l&#39;immagine
* Nome originale del [!DNL Facebook] immagine

Dopo l’elaborazione, il modulo ha restituito le seguenti informazioni di output:

* ID immagine assegnato da [!DNL Dropbox]
* Percorso completo in cui [!DNL Dropbox] [!DNL Workfront Fusion] ha caricato il file

Le informazioni di cui sopra vengono acquisite separatamente per ogni bundle, come indicato dalle caselle a discesa [!UICONTROL Operazione 1] e [!UICONTROL Operazione 2] nell&#39;immagine.

Per ulteriori informazioni sull’elaborazione delle transazioni, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Si è verificato un errore durante l’esecuzione di uno scenario

Durante l’esecuzione dello scenario potrebbe verificarsi un errore. Ad esempio, se elimini il [!DNL Dropbox] cartella impostata come cartella di destinazione nell’impostazione del modulo, lo scenario termina con un messaggio di errore. Per ulteriori informazioni su come gestire gli errori, consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

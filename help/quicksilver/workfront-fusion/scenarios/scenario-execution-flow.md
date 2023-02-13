---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flusso di esecuzione dello scenario in Adobe Workfront Fusion
description: Questo articolo spiega come viene eseguito uno scenario e come i dati scorrono al suo interno. Inoltre, spiega dove è possibile trovare informazioni sui dati elaborati e come leggerli.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]

Questo articolo spiega come viene eseguito uno scenario e come i dati scorrono al suo interno. Inoltre, spiega dove è possibile trovare informazioni sui dati elaborati e come leggerli.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Flusso di esecuzione scenario

Una volta configurato correttamente e attivato uno scenario, questo viene eseguito in base alla pianificazione definita.

All’inizio dello scenario, il primo modulo risponde a un evento per il quale è stato impostato il controllo. Se restituisce bundle (dati), passano al modulo successivo e lo scenario continua, passando i bundle attraverso ogni modulo successivo, uno per uno.

Se i bundle vengono elaborati correttamente in tutti i moduli, lo scenario viene contrassegnato come un successo nell&#39;area di dettaglio dello scenario, come spiegato in [Dettagli scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Per ulteriori informazioni sulla configurazione di uno scenario, vedi [Impostazioni di scenario di base in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Per ulteriori informazioni sull&#39;attivazione di uno scenario, vedi [Attiva o disattiva uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Per ulteriori informazioni sulla pianificazione di uno scenario, vedi [Pianifica uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Per ulteriori informazioni sui moduli, consulta [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione del lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario che controlla le richieste in arrivo in [!DNL Workfront] e poi li converte in [!DNL Workfront] I dati fluiranno come segue.
>
>Il primo passaggio dello scenario, eseguito dal primo modulo, consiste nel monitorare le richieste. Ogni richiesta che arriva in è considerata un bundle. Se il modulo viene eseguito senza trovare alcun bundle, lo scenario termina dopo il primo modulo.
>
>Se il primo modulo restituisce un bundle, il bundle passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall’ultimo modulo, che converte la richiesta in un progetto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario che scarica documenti da [!DNL Adobe Workfront] e li invia a una cartella in [!DNL Dropbox], i dati scorrono come segue.
>
>Il primo passo dello scenario, eseguito dal primo modulo, è quello di guardare i bundle (documenti). In questo esempio, il modulo controlla i bundle in [!DNL Workfront]. Se non restituisce un bundle, lo scenario termina dopo il primo modulo.
>
>Se viene restituito un bundle, il bundle passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall’ultimo modulo, che carica il bundle nel [!DNL Dropbox] cartella.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Se il primo modulo restituisce più bundle, il primo bundle viene caricato in [!DNL Dropbox] prima del caricamento del secondo bundle. Poi il secondo bundle viene caricato, poi il terzo e così via.

## Informazioni sui bundle elaborati

Per ogni modulo, il bundle passa attraverso un processo in 4 fasi prima di passare al modulo successivo o raggiungere la sua destinazione finale. Il processo in 4 fasi è l’inizializzazione, il funzionamento, il commit/rollback e la finalizzazione. Questa operazione è denominata elaborazione delle transazioni e spiega in che modo i dati sono stati elaborati in un modulo.

Una volta completata l&#39;esecuzione di uno scenario, ogni modulo visualizza un&#39;icona che indica il numero di operazioni eseguite. Fai clic su questa icona per visualizzare le informazioni dettagliate sui bundle elaborati nel formato descritto sopra. Puoi vedere quali impostazioni di moduli sono state utilizzate e quali bundle sono stati restituiti da quale modulo.

![](assets/info-processed-bundles-350x396.png)

Un modulo ha ricevuto informazioni di input quali:

* Immagine convertita
* Cartella selezionata in cui deve essere caricata l&#39;immagine
* Nome originale [!DNL Facebook] immagine

Dopo l’elaborazione, il modulo ha restituito queste informazioni di output:

* ID immagine assegnato da [!DNL Dropbox]
* Percorso completo in cui [!DNL Dropbox] [!DNL Workfront Fusion] caricato il file

Le informazioni di cui sopra vengono acquisite separatamente per ogni bundle, come indicato dalle caselle a discesa [!UICONTROL Operazione 1] e [!UICONTROL Operazione 2] nell&#39;immagine.

Per ulteriori informazioni sull&#39;elaborazione delle transazioni vedi [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Errore durante l&#39;esecuzione di uno scenario

Potrebbe verificarsi un errore durante l&#39;esecuzione dello scenario. Ad esempio, se elimini il [!DNL Dropbox] cartella impostata come cartella di destinazione nell&#39;impostazione del modulo, lo scenario termina con un messaggio di errore. Per ulteriori informazioni su come gestire gli errori, consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

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
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '799'
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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Flusso di esecuzione dello scenario

Dopo aver configurato correttamente e attivato uno scenario, questo viene eseguito in base alla pianificazione definita.

All’inizio dello scenario, il primo modulo risponde a un evento che è stato impostato per osservare. Se restituisce eventuali bundle (dati), questi passano al modulo successivo e lo scenario continua, passando i bundle attraverso ciascun modulo successivo, uno alla volta.

Se i bundle vengono elaborati correttamente in tutti i moduli, lo scenario viene contrassegnato come riuscito nell&#39;area dei dettagli dello scenario, come spiegato in [Dettagli scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Per ulteriori informazioni sulla configurazione di uno scenario, vedere [L&#39;editor dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
* Per ulteriori informazioni sull&#39;attivazione di uno scenario, vedere [Attivare o disattivare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Per ulteriori informazioni sulla pianificazione di uno scenario, vedere [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Per ulteriori informazioni sui moduli, vedere [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione del lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario che controlla le richieste in arrivo in [!DNL Workfront] e le converte in [!DNL Workfront] progetti, i dati scorrono come segue.
>
>Il primo passaggio dello scenario, eseguito dal primo modulo, consiste nel controllare le richieste. Ogni richiesta in entrata viene considerata un bundle. Se il modulo viene eseguito senza trovare bundle, lo scenario termina dopo il primo modulo.
>
>Se il primo modulo restituisce un bundle, il bundle passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall’ultimo modulo, che convertono la richiesta in un progetto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Esempio: [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione e l&#39;integrazione del lavoro]

>[!INFO]
>
>**Esempio:** In uno scenario che scarica documenti da [!DNL Adobe Workfront] e li invia a una cartella in [!DNL Dropbox], i dati scorrono come segue.
>
>Il primo passaggio dello scenario, eseguito dal primo modulo, consiste nel controllare i bundle (documenti). In questo esempio, il modulo controlla i bundle in [!DNL Workfront]. Se non restituisce un bundle, lo scenario termina dopo il primo modulo.
>
>Se viene restituito un bundle, questo passa attraverso il resto dello scenario. In questo esempio, il resto dello scenario è costituito dal secondo e dall&#39;ultimo modulo, che caricano il bundle nella cartella [!DNL Dropbox].
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Se il primo modulo restituisce più bundle, il primo viene caricato in [!DNL Dropbox] prima del secondo. Poi viene caricato il secondo bundle, poi il terzo e così via.

## Informazioni sui bundle elaborati

Per ogni modulo, il bundle passa attraverso un processo in 4 fasi prima di passare al modulo successivo o di raggiungere la sua destinazione finale. Il processo in 4 fasi consiste in inizializzazione, operazione, commit/rollback e finalizzazione. Questa funzione è denominata elaborazione delle transazioni e aiuta a spiegare come sono stati elaborati i dati in un modulo.

Una volta completata l’esecuzione di uno scenario, ogni modulo visualizza un’icona che mostra il numero di operazioni eseguite. Puoi fare clic su questa icona per visualizzare le informazioni dettagliate sui bundle elaborati, nel formato descritto sopra. Puoi vedere quali impostazioni di moduli sono state utilizzate e quali bundle sono stati restituiti da quale modulo.

![](assets/info-processed-bundles-350x396.png)

Un modulo ha ricevuto informazioni di input quali:

* Immagine convertita
* Cartella selezionata in cui caricare l&#39;immagine
* Nome originale dell&#39;immagine [!DNL Facebook]

Dopo l’elaborazione, il modulo ha restituito le seguenti informazioni di output:

* ID immagine assegnato da [!DNL Dropbox]
* Percorso completo in cui in [!DNL Dropbox] [!DNL Workfront Fusion] è stato caricato il file

Le informazioni precedenti vengono acquisite separatamente per ogni bundle, come indicato dalle caselle a discesa [!UICONTROL Operazione 1] e [!UICONTROL Operazione 2] nell&#39;immagine.

Per ulteriori informazioni sull&#39;elaborazione delle transazioni, vedere [Esecuzione dello scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Si è verificato un errore durante l’esecuzione di uno scenario

Durante l’esecuzione dello scenario potrebbe verificarsi un errore. Se ad esempio si elimina la cartella [!DNL Dropbox] impostata come cartella di destinazione nell&#39;impostazione del modulo, lo scenario termina con un messaggio di errore. Per ulteriori informazioni sulla gestione degli errori, vedere [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

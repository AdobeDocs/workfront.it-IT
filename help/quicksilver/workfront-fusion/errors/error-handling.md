---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione degli errori in [!DNL Adobe Workfront Fusion]
description: Quando si verificano errori durante l’esecuzione di uno scenario, in genere si verifica perché un servizio non è disponibile a causa di un errore, un servizio risponde con dati imprevisti o la convalida dei dati di input non riesce.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Gestione degli errori in [!DNL Adobe Workfront Fusion]

Quando si verificano errori durante l’esecuzione di uno scenario, in genere si verifica perché un servizio non è disponibile a causa di un errore, un servizio risponde con dati imprevisti o la convalida dei dati di input non riesce.

>[!NOTE]
>
>Se un modulo genera un errore durante l’esecuzione dello scenario e non è presente alcuna route di gestione degli errori collegata al modulo, viene eseguita una logica di gestione degli errori predefinita come descritto in [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Aggiungendo un percorso di gestione degli errori a un modulo, puoi sostituire la logica di gestione degli errori predefinita con la tua. [!DNL Adobe Workfront Fusion] offre 5 diverse direttive, ognuna delle quali può essere inserita alla fine dei percorsi dei gestori di errori. Per ulteriori informazioni, consulta [Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## route del gestore errori

Per aggiungere un percorso del gestore di errori a un modulo (lo chiameremo Modulo X), fai clic con il pulsante destro del mouse sul modulo e seleziona **[!UICONTROL Aggiungi handler di errori]**:

![](assets/error-handler-route.png)

Il modulo mostra un elenco di Direttive e delle app utilizzate nel tuo scenario. Se il modulo X è l&#39;ultimo modulo del percorso, è necessario scegliere una delle direttive. Oppure puoi continuare ad aggiungere uno o più moduli al tuo percorso. In questo caso, il [!UICONTROL Ignora] La direttiva è applicata per impostazione predefinita al modulo X e, in caso di errore, vengono elaborati i moduli successivi su tale rotta.

![](assets/directives-350x426.png)

Come puoi vedere di seguito, se si verifica un errore durante l’esecuzione del [!UICONTROL Creare una cartella] il modulo [!UICONTROL Ignora] La direttiva verrà applicata automaticamente e lo scenario si sposterà al modulo successivo sulla route del gestore di errori se il filtro &quot;Data Error Performing&quot; restituisce uno o più bundle.

Tuttavia, in assenza di errori, lo scenario verrà spostato nella [!UICONTROL Elencare tutti i file in un modulo cartelle] sulla rotta regolare.

![](assets/if-there-is-no-error-350x234.png)

Inoltre, per differenziare un percorso di gestione degli errori da un percorso regolare, il primo è composto da cerchi trasparenti come mostrato sopra.

## Direttive per la gestione degli errori

Le direttive sono brevemente illustrate di seguito. Per ulteriori informazioni, consulta [Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Sono disponibili in totale cinque direttive che possono essere raggruppate nelle seguenti categorie in base al fatto che l&#39;esecuzione di uno scenario debba continuare o meno:

Le seguenti direttive assicurano che l&#39;esecuzione di uno scenario continui:

* **[!UICONTROL Riprendi]** consente di specificare un output sostitutivo per il modulo con l’errore e lo stato di esecuzione dello scenario è contrassegnato come riuscito
* **[!UICONTROL Ignora]** ignora semplicemente l’errore e lo stato di esecuzione dello scenario viene contrassegnato come riuscito
* **[!UICONTROL Interruzione]** memorizza l&#39;input nella coda di esecuzioni incomplete e lo stato di esecuzione dello scenario viene contrassegnato come avviso. Per ulteriori informazioni, consulta [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

D&#39;altro canto, se l&#39;esecuzione di uno scenario deve essere interrotta, è necessario utilizzare una delle seguenti direttive:

* **[!UICONTROL Ripristino]** interrompe immediatamente l&#39;esecuzione dello scenario e ne contrassegna lo stato come errore
* **[!UICONTROL Commit]** interrompe immediatamente l’esecuzione dello scenario e ne contrassegna lo stato come completato

## Risorse aggiuntive

* [Direttive sulla gestione degli errori [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestione avanzata degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (include la configurazione del Dropbox Scenario di cui sopra)

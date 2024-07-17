---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione degli errori in [!DNL Adobe Workfront Fusion]
description: Quando si verificano errori durante l'esecuzione di uno scenario, in genere ciò è dovuto al fatto che un servizio non è disponibile a causa di un errore, che risponde con dati imprevisti o che la convalida dei dati di input non riesce.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Gestione degli errori in [!DNL Adobe Workfront Fusion]

Quando si verificano errori durante l&#39;esecuzione di uno scenario, in genere ciò è dovuto al fatto che un servizio non è disponibile a causa di un errore, che risponde con dati imprevisti o che la convalida dei dati di input non riesce.

Se un modulo genera un errore durante l&#39;esecuzione dello scenario e non vi è alcuna route di gestione degli errori associata al modulo, viene eseguita la logica di gestione degli errori predefinita, come descritto in [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Aggiungendo a un modulo una route del gestore degli errori, è possibile sostituire la logica predefinita di gestione degli errori con la propria. [!DNL Adobe Workfront Fusion] offre cinque diverse direttive che possono essere inserite alla fine dei percorsi del gestore degli errori.

Per ulteriori informazioni, vedere [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Route gestore errori

Per aggiungere una route del gestore degli errori a un modulo:

1. Fare clic con il pulsante destro del mouse sul modulo e selezionare **[!UICONTROL Aggiungi gestore errori]**:

   ![](assets/error-handler-route.png)

   Il modulo mostra un elenco di direttive e delle app utilizzate nel tuo scenario.

1. Se il modulo a cui è stato aggiunto un gestore errori è l&#39;ultimo modulo del percorso, selezionare una delle direttive.

   Oppure

   Aggiungere uno o più moduli alla route del gestore degli errori.

   Se si aggiungono altri moduli alla route, la direttiva [!UICONTROL Ignora] viene applicata per impostazione predefinita e, in caso di errore, vengono elaborati i moduli successivi della route.


>[!INFO]
>
>In questo esempio, se si verifica un errore durante l&#39;esecuzione del modulo [!UICONTROL Crea cartella], la direttiva [!UICONTROL Ignora] verrà applicata automaticamente e lo scenario verrà spostato al modulo successivo sulla route del gestore degli errori.
>
>Tuttavia, se non si verifica alcun errore, lo scenario verrà spostato in [!UICONTROL Elenca tutti i file in un modulo cartella] sulla route regolare.
>
>![](assets/if-there-is-no-error-350x234.png)

Si noti che una route del gestore degli errori è composta da cerchi trasparenti, mentre una route regolare è composta da cerchi solidi.

## Direttive sulla gestione degli errori

Le direttive sono brevemente illustrate qui di seguito. Per ulteriori informazioni, vedere [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

In totale, cinque direttive possono essere raggruppate nelle seguenti categorie in base al fatto che l’esecuzione di uno scenario debba continuare o meno.

Le seguenti direttive garantiscono la prosecuzione dell’esecuzione di uno scenario:

* **[!UICONTROL Riprendi]**: consente di specificare un output sostitutivo per il modulo con l&#39;errore. Lo stato di esecuzione dello scenario è contrassegnato come completato
* **[!UICONTROL Ignora]**: ignora l&#39;errore. Lo stato di esecuzione dello scenario è contrassegnato come completato
* **[!UICONTROL Interruzione]**: memorizza l&#39;input nella coda di esecuzioni incomplete. Lo stato di esecuzione dello scenario è contrassegnato come avviso. Per ulteriori informazioni, vedere [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Se l’esecuzione di uno scenario deve interrompersi quando si verifica un errore, utilizza una delle seguenti direttive:

* **[!UICONTROL Rollback]**: interrompe immediatamente l&#39;esecuzione dello scenario e ne contrassegna lo stato come errore
* **[!UICONTROL Commit]**: interrompe immediatamente l&#39;esecuzione dello scenario e ne contrassegna lo stato come completato

Per ulteriori informazioni sulla gestione degli errori, vedere:

* [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestione avanzata degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)
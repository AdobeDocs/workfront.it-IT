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

Se un modulo genera un errore durante l’esecuzione dello scenario e non è associato alcun percorso di gestione degli errori, viene eseguita la logica di gestione degli errori predefinita, come descritto in [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Aggiungendo a un modulo una route del gestore degli errori, è possibile sostituire la logica predefinita di gestione degli errori con la propria. [!DNL Adobe Workfront Fusion] offre cinque direttive diverse che possono essere inserite alla fine dei percorsi del gestore degli errori.

Per ulteriori informazioni, consulta [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Route gestore errori

Per aggiungere una route del gestore degli errori a un modulo:

1. Fai clic con il pulsante destro del mouse sul modulo e seleziona (Gestisci origini dati) **[!UICONTROL Aggiungi gestore errori]**:

   ![](assets/error-handler-route.png)

   Il modulo mostra un elenco di direttive e delle app utilizzate nel tuo scenario.

1. Se il modulo a cui è stato aggiunto un gestore errori è l&#39;ultimo modulo del percorso, selezionare una delle direttive.

   Oppure

   Aggiungere uno o più moduli alla route del gestore degli errori.

   Se si aggiungono altri moduli alla route, [!UICONTROL Ignora] La direttiva viene applicata per impostazione predefinita e, in caso di errore, vengono elaborati i moduli successivi su tale route.


>[!INFO]
>
>In questo esempio, se si verifica un errore durante l&#39;esecuzione di [!UICONTROL Creare una cartella] modulo, il [!UICONTROL Ignora] La direttiva verrà applicata automaticamente e lo scenario passerà al modulo successivo sulla route del gestore degli errori.
>
>Tuttavia, in assenza di errori, lo scenario passerà al [!UICONTROL Elencare tutti i file in un modulo cartella] sulla rotta regolare.
>
>![](assets/if-there-is-no-error-350x234.png)

Si noti che una route del gestore degli errori è composta da cerchi trasparenti, mentre una route regolare è composta da cerchi solidi.

## Direttive sulla gestione degli errori

Le direttive sono brevemente illustrate qui di seguito. Per ulteriori informazioni, consulta [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

In totale, cinque direttive possono essere raggruppate nelle seguenti categorie in base al fatto che l’esecuzione di uno scenario debba continuare o meno.

Le seguenti direttive garantiscono la prosecuzione dell’esecuzione di uno scenario:

* **[!UICONTROL Riprendi]**: consente di specificare un output sostitutivo per il modulo con l’errore. Lo stato di esecuzione dello scenario è contrassegnato come completato
* **[!UICONTROL Ignora]**: ignora l’errore. Lo stato di esecuzione dello scenario è contrassegnato come completato
* **[!UICONTROL Interrompi]**: memorizza l’input nella coda di esecuzioni incomplete. Lo stato di esecuzione dello scenario è contrassegnato come avviso. Per ulteriori informazioni, consulta [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Se l’esecuzione di uno scenario deve interrompersi quando si verifica un errore, utilizza una delle seguenti direttive:

* **[!UICONTROL Rollback]**: interrompe immediatamente l’esecuzione dello scenario e ne contrassegna lo stato come errore
* **[!UICONTROL Conferma]**: interrompe immediatamente l’esecuzione dello scenario e ne contrassegna lo stato come completato

Per ulteriori informazioni sulla gestione degli errori, vedere:

* [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestione avanzata degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)
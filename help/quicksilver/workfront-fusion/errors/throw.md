---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione degli errori in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Gestione degli errori in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Soluzione alternativa per configurare `throw` errore](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In alcuni casi, è possibile interrompere forzatamente l&#39;esecuzione dello scenario seguita da [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) o [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) o interrompere l&#39;elaborazione di una route e, facoltativamente, archiviarla nella coda di esecuzioni incomplete.

Attualmente le direttive di gestione degli errori non possono essere utilizzate al di fuori dell&#39;ambito di un [Route del gestore degli errori](../../workfront-fusion/errors/error-handling.md#error) e [!DNL Adobe Workfront Fusion] non offre un modulo che consentirebbe di generare facilmente errori in modo condizionale.

Per informazioni sulle esecuzioni incomplete, vedere [Visualizzare e risolvere le esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Per informazioni sulle direttive per la gestione degli errori, vedere [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Per informazioni sulle licenze [!DNL Adobe Workfront Fusion], vedere [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Soluzione alternativa per il lancio

Per generare un errore in modo condizionale, puoi configurare un modulo in modo che, durante il suo funzionamento, possa avere esito negativo intenzionalmente. Una possibilità è quella di utilizzare il modulo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] (vedi [Moduli JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurato per generare facoltativamente un errore (in questo caso BundleValidationError):

È quindi possibile allegare una delle direttive di gestione degli errori al percorso di gestione degli errori a:

* Forza l&#39;interruzione dell&#39;esecuzione dello scenario ed esegui la fase di rollback: [!UICONTROL Rollback]
* Forza l&#39;interruzione dell&#39;esecuzione dello scenario ed esegui la fase di commit: [!UICONTROL Commit]
* Interrompi l&#39;elaborazione di una route: [!UICONTROL Ignora]
* Interrompere l&#39;elaborazione di una route e archiviarla nella coda della cartella esecuzioni incomplete: [!UICONTROL Interrompi]

Nell&#39;esempio seguente viene illustrato l&#39;utilizzo della direttiva [!DNL Rollback]:

![](assets/rollback-directive-350x175.png)

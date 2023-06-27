---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestione degli errori in Adobe Workfront Fusion
description: In alcuni casi può essere utile interrompere forzatamente l’esecuzione dello scenario seguita dalla fase di rollback o commit o interrompere l’elaborazione di una route e, facoltativamente, memorizzarla nella coda di visualizzazione e risolvere le esecuzioni incomplete in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Gestione degli errori in [!DNL Adobe Workfront Fusion]

In alcuni casi, potrebbe essere utile interrompere forzatamente l’esecuzione dello scenario seguita da [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) o [Conferma](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) o per interrompere l’elaborazione di una route e, facoltativamente, memorizzarla nella coda di esecuzioni incomplete.

Attualmente le direttive di gestione degli errori non possono essere utilizzate al di fuori dell’ambito di un’ [Route gestore errori](../../workfront-fusion/errors/error-handling.md#error) e [!DNL Adobe Workfront Fusion] non offre un modulo che consentirebbe di generare (generare) errori in modo semplice e condizionale.

Per informazioni sulle esecuzioni incomplete, vedi [Visualizzare e risolvere esecuzioni incomplete in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Per informazioni sulle direttive per la gestione degli errori, consulta [Direttive per la gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Soluzione alternativa per il lancio

Per generare un errore in modo condizionale, puoi configurare un modulo in modo che, durante il suo funzionamento, possa avere esito negativo intenzionalmente. Una possibilità consiste nell&#39;utilizzare [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo (vedere [Moduli JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurato per generare facoltativamente un errore (BundleValidationError in questo caso):

È quindi possibile allegare una delle direttive di gestione degli errori al percorso di gestione degli errori a:

* Forza l’interruzione dell’esecuzione dello scenario ed esegui la fase di rollback: [!UICONTROL Rollback]
* Forza l’interruzione dell’esecuzione dello scenario ed esegui la fase di commit: [!UICONTROL Conferma]
* Interrompere l&#39;elaborazione di una route: [!UICONTROL Ignora]
* Interrompere l&#39;elaborazione di una route e archiviarla nella coda della cartella esecuzioni incomplete: [!UICONTROL Interrompi]

L’esempio seguente mostra l’utilizzo di [!DNL Rollback] direttiva:

![](assets/rollback-directive-350x175.png)

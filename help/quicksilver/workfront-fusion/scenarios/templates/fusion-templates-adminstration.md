---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Amministrazione di modelli Adobe Workfront Fusion
description: Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. È possibile eseguire queste azioni da [!UICONTROL Modelli] pagina in [!DNL Adobe Workfront Fusion Administration] area.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Amministrazione di modelli

Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. È possibile eseguire queste azioni da [!UICONTROL Modelli] pagina in [!DNL Adobe Workfront Fusion Administration] area.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront Fusion per la tua organizzazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Visualizza [!DNL Workfront Fusion] modelli come amministratore

Per visualizzare una tabella di tutti i modelli creati e dei relativi stati:

1. Clic **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Clic **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.

Sono disponibili tre colonne relative allo stato di pubblicazione dei modelli. Un segno di spunta in una colonna indica quanto segue:

* **[!UICONTROL Pubblicato]**: questi modelli sono attualmente visibili in [!UICONTROL Modelli team] nell&#39;interfaccia utente.
* **[!UICONTROL Approvazione richiesta]**: questi modelli sono in attesa della tua approvazione. Attualmente sono visibili nella sezione [!UICONTROL Modelli team] nell&#39;interfaccia utente.
* **[!UICONTROL Approvato]**: questi modelli sono stati approvati. Attualmente sono visibili nella sezione [!UICONTROL Modelli pubblici] nell’interfaccia utente standard.

>[!NOTE]
>
>Modelli con segno di spunta in entrambi [!UICONTROL Approvazione richiesta] e nella [!UICONTROL Approvato] La colonna è già stata approvata e resa pubblica, ma è disponibile una versione più recente in attesa della tua approvazione.

## Modifica [!DNL Workfront Fusion] modelli come amministratore

1. Clic **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Clic **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Clic **[!UICONTROL Dettaglio]** a destra del modello da modificare.

Ora puoi modificare il modello, in modo analogo a come si modifica un modello se sei un utente non amministratore. Tuttavia, nella [!UICONTROL Opzioni] nell’angolo in alto a destra è presente un’opzione aggiuntiva: il diagramma SVG che fornisce il codice SVG. Inoltre, il processo di pubblicazione è lo stesso del caso di un utente standard. Per ulteriori informazioni, consulta la sezione Pubblicazione e condivisione di modelli.

Per informazioni sulle opzioni specifiche del modello che è possibile modificare, consulta [Creare nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Per informazioni sulla pubblicazione dei modelli, consulta [Pubblica e condividi [!DNL Adobe Workfront Fusion] modelli](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approva o disapprova [!DNL Workfront Fusion] modelli

L’approvazione di un modello lo rende visibile nel [!UICONTROL Modelli pubblici] e disponibile per tutti gli utenti. Se si disapprova un modello, questo viene rimosso dalla [!UICONTROL Modelli pubblici] e la rende disponibile solo al team che l’ha creata.

1. Clic **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Clic **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Per approvare un modello, fai clic su **[!UICONTROL Approva]** a destra del modello.
1. Per disapprovare un modello, fare clic su **[!UICONTROL Disapprova]** a destra del modello.

>[!NOTE]
>
>Se approvi il modello precedentemente approvato e quindi modificato, la seconda approvazione sovrascriverà il modello originale.

## Clonare uno scenario come modello

In qualità di amministratore, puoi clonare uno scenario come modello.

Per istruzioni sulla clonazione di uno scenario come modello, consulta [Creare un modello da uno scenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Creare nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)

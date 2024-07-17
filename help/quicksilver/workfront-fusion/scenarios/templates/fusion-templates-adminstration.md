---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Amministrazione di modelli Adobe Workfront Fusion
description: Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. Puoi eseguire queste azioni dalla pagina [!UICONTROL Modelli] nell'area [!DNL Adobe Workfront Fusion Administration] .
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 2b67b5fb951b5ae7867144c444411ebd1c299e75
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Amministrazione di [!DNL Adobe Workfront Fusion] modelli

Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. Puoi eseguire queste azioni dalla pagina [!UICONTROL Modelli] nell&#39;area [!DNL Adobe Workfront Fusion Administration].

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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront Fusion per la tua organizzazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Visualizza [!DNL Workfront Fusion] modelli come amministratore [!DNL Workfront Fusion]

Per visualizzare una tabella di tutti i modelli creati e dei relativi stati:

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire l&#39;area [!UICONTROL Amministrazione].

   >[!NOTE]
   >
   >L&#39;area Amministrazione è visibile solo agli amministratori di Workfront Fusion.

1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.

Sono disponibili tre colonne relative allo stato di pubblicazione dei modelli. Un segno di spunta in una colonna indica quanto segue:

* **[!UICONTROL Pubblicato]**: questi modelli sono attualmente visibili nella scheda [!UICONTROL Modelli team] nell&#39;interfaccia utente.
* **[!UICONTROL Approvazione richiesta]**: questi modelli sono in attesa della tua approvazione. Sono attualmente visibili nella scheda [!UICONTROL Modelli team] nell&#39;interfaccia utente.
* **[!UICONTROL Approvati]**: questi modelli sono stati approvati. Sono attualmente visibili nella scheda [!UICONTROL Modelli pubblici] nell&#39;interfaccia utente standard.

>[!NOTE]
>
>I modelli con il segno di spunta nella colonna [!UICONTROL Approvazione richiesta] e nella colonna [!UICONTROL Approvato] sono già stati approvati e resi pubblici, ma è disponibile una versione più recente in attesa della tua approvazione.

## Modifica [!DNL Workfront Fusion] modelli come amministratore

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire l&#39;area [!UICONTROL Amministrazione].
1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Fare clic su **[!UICONTROL Dettagli]** a destra del modello che si desidera modificare.

Ora puoi modificare il modello, in modo analogo a come si modifica un modello se sei un utente non amministratore. Tuttavia, nelle [!UICONTROL Opzioni] nell&#39;angolo in alto a destra è presente un&#39;opzione aggiuntiva: il diagramma SVG che fornisce il codice SVG. Inoltre, il processo di pubblicazione è lo stesso del caso di un utente standard. Per ulteriori informazioni, consulta la sezione Pubblicazione e condivisione di modelli.

Per informazioni sulle opzioni specifiche del modello modificabili, vedere [Creare nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Per informazioni sulla pubblicazione di modelli, vedere [Publish e condividere [!DNL Adobe Workfront Fusion] modelli](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approva o disapprova [!DNL Workfront Fusion] modelli

L&#39;approvazione di un modello lo rende visibile nella scheda [!UICONTROL Modelli pubblici] e disponibile a tutti gli utenti. Se si disapprova un modello, questo viene rimosso dalla scheda [!UICONTROL Modelli pubblici] e reso disponibile solo al team che lo ha creato.

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire l&#39;area [!UICONTROL Amministrazione].
1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Per approvare un modello, fare clic su **[!UICONTROL Approva]** a destra del modello.
1. Per disapprovare un modello, fare clic su **[!UICONTROL Disapprova]** a destra del modello.

>[!NOTE]
>
>Se approvi il modello precedentemente approvato e quindi modificato, la seconda approvazione sovrascriverà il modello originale.

## Clonare uno scenario come modello

In qualità di amministratore, puoi clonare uno scenario come modello.

Per istruzioni sulla clonazione di uno scenario come modello, vedere [Creare un modello da uno scenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Creare nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)

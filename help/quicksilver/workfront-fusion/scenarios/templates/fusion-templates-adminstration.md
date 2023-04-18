---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Amministrazione di modelli Adobe Workfront Fusion
description: Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. Puoi eseguire queste azioni dalla [!UICONTROL Modelli] nella pagina [!DNL Adobe Workfront Fusion Administration] area.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Amministrazione dei modelli

Gli amministratori dispongono delle autorizzazioni necessarie per visualizzare, modificare, rinominare, pubblicare, approvare ed eliminare i modelli creati da altri utenti. Puoi eseguire queste azioni dalla [!UICONTROL Modelli] nella pagina [!DNL Adobe Workfront Fusion Administration] area.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario essere un amministratore di Workfront Fusion per la propria organizzazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Visualizza [!DNL Workfront Fusion] modelli come amministratore

Per visualizzare una tabella di tutti i modelli creati e dei relativi stati:

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.

Lo stato di pubblicazione dei modelli è correlato a tre colonne. Un segno di spunta in una colonna indica quanto segue:

* **[!UICONTROL Pubblicato]**: Questi modelli sono attualmente visibili nella [!UICONTROL Modelli team] nell’interfaccia utente di .
* **[!UICONTROL Approvazione richiesta]**: Questi modelli sono in attesa dell’approvazione. Sono attualmente visibili nella [!UICONTROL Modelli team] nell’interfaccia utente di .
* **[!UICONTROL Approvato]**: Questi modelli sono stati approvati. Sono attualmente visibili nella [!UICONTROL Modelli pubblici] nell’interfaccia utente standard.

>[!NOTE]
>
>Modelli con segno di spunta in entrambi i modelli [!UICONTROL Approvazione richiesta] e nella colonna [!UICONTROL Approvato] La colonna è già stata approvata e resa pubblica, ma è disponibile una versione più recente in attesa della tua approvazione.

## Modifica [!DNL Workfront Fusion] modelli come amministratore

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Fai clic su **[!UICONTROL Dettaglio]** a destra del modello da modificare.

Ora puoi modificare il modello, in modo analogo a come modificarlo come utente non amministratore. Tuttavia, nella [!UICONTROL Opzioni] nell’angolo in alto a destra è disponibile un’opzione aggiuntiva, il diagramma di SVG, che fornisce il codice di SVG. Inoltre, il processo di pubblicazione è lo stesso del caso di un utente standard. Per ulteriori informazioni, consulta la sezione Pubblicazione e condivisione di modelli .

Per informazioni sulle opzioni di modello specifiche che è possibile modificare, consulta [Crea nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Per informazioni sulla pubblicazione dei modelli, consulta [Pubblicare e condividere [!DNL Adobe Workfront Fusion] modelli](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approvare o disapprovare [!DNL Workfront Fusion] modelli

L’approvazione di un modello lo rende visibile nella [!UICONTROL Modelli pubblici] e disponibile per tutti gli utenti. La disapprovazione di un modello lo rimuove dalla [!UICONTROL Modelli pubblici] e lo rende disponibile solo al team che lo ha creato.

1. Fai clic su **[!UICONTROL Amministrazione]** nel pannello di navigazione a sinistra per aprire [!UICONTROL Amministrazione] area.
1. Fai clic su **[!UICONTROL Modelli]** nel pannello di navigazione a sinistra.
1. Se desideri approvare un modello, fai clic su **[!UICONTROL Approva]** a destra del modello.
1. Se desideri disapprovare un modello, fai clic su **[!UICONTROL Disapprovare]** a destra del modello.

>[!NOTE]
>
>Se approvi il modello approvato in precedenza e modificato, la seconda approvazione sovrascrive il modello originale.

## Clonare uno scenario come modello

In qualità di amministratore, puoi clonare uno scenario come modello.

Per istruzioni sulla clonazione di uno scenario come modello, vedi [Creare un modello da uno scenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Crea nuovi modelli in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)

---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Aggiungere un filtro a uno scenario in [!DNL Adobe] Workfront Fusion
description: In alcuni scenari, devi lavorare solo con bundle che soddisfano criteri specifici. I filtri ti consentono di selezionare tali bundle.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]

In alcuni scenari, devi lavorare solo con bundle che soddisfano criteri specifici. I filtri ti consentono di selezionare tali bundle.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Puoi aggiungere un filtro tra due moduli e verificare se i bundle ricevuti dai moduli precedenti soddisfano specifiche condizioni del filtro:

* In caso affermativo, i bundle passano al modulo successivo nello scenario.
* In caso contrario, l’elaborazione dei bundle termina.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>    </tr> 
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

## Prerequisiti

È necessario aggiungere entrambi i moduli a uno scenario prima di poter aggiungere un filtro tra di essi.

## Aggiungi un filtro tra due moduli:

1. Clic **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra, seleziona lo scenario per aprirlo.
1. Nell&#39;angolo superiore destro della finestra fare clic su **[!UICONTROL Modifica]**.
1. Fare clic sulla linea di connessione tra i moduli.
1. Nella casella visualizzata, digita **[!UICONTROL Etichetta]** per il filtro.
1. Definire un filtro **[!UICONTROL Condizione]**.

   Potete immettere uno o due operandi nelle due caselle. Se si immettono operandi in entrambe le caselle, è possibile selezionare un operatore nel menu a discesa tra di essi per specificare la relazione tra di essi.

   >[!TIP]
   >
   >Nei campi dell&#39;operando, è possibile immettere i valori nello stesso modo in cui vengono mappati, come descritto in [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Ad esempio, se desideri che il filtro trovi i file [!DNL Adobe Workfront] terminando con XML e trasmettendoli a [!DNL Dropbox], si immette **[!UICONTROL Nome file]** nella prima casella e .**[!UICONTROL xml]** nella seconda casella. Nel menu a discesa tra di essi, puoi selezionare **[!UICONTROL Termina con (senza distinzione maiuscole/minuscole)]**. Questo filtro si applica ai bundle in arrivo dal primo modulo (Workfront). Solo i bundle contenenti file XML vengono trasmessi al modulo successivo ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Clic **[!DNL OK]**.

## Copiare un filtro

Attualmente, l’editor di scenari non include una funzione per copiare un filtro.

>[!NOTE]
>
>Se copi i moduli su entrambi i lati del filtro, viene copiato anche il filtro.
>
>Per ulteriori informazioni sulla copia dei moduli, consulta [Copiare moduli o scenari in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Per copiare un filtro senza copiare i moduli, puoi utilizzare [!DNL Google] Chrome per la seguente soluzione alternativa:

1. Installare [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] estensione.
1. In entrata [!DNL Workfront Fusion], apri lo scenario.
1. Fai clic sul menu a tre punti di Chrome, quindi fai clic su **[!UICONTROL Altri strumenti*]* > **[!UICONTROL Strumenti per sviluppatori]**.

1. In [!UICONTROL Strumenti per sviluppatori] nella barra dei menu nella parte superiore, fare clic sul pulsante [!UICONTROL Workfront Fusion] scheda.

   ![](assets/copy-a-filter-350x174.png)

1. Fai clic su **[!UICONTROL Strumenti]** icona ![](assets/devtools-tools-icon.png) nella barra laterale sinistra.

1. Clic **[!UICONTROL Copia filtro]**, quindi configura il **[!UICONTROL Copia filtro]** strumento nel pannello laterale destro:

   1. Imposta il **[!UICONTROL Modulo sorgente]** come modulo subito dopo il filtro che desideri copiare.
   1. Imposta il **[!UICONTROL Modulo di destinazione]** come modulo immediatamente prima del filtro che desideri copiare.

1. Clic **[!UICONTROL Esegui]**.

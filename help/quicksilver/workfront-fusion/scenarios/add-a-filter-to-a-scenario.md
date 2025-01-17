---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Aggiungere un filtro a uno scenario in [!DNL Adobe] Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Aggiungere un filtro a uno scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-filter-to-a-scenario.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>    </tr> 
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

## Prerequisiti

È necessario aggiungere entrambi i moduli a uno scenario prima di poter aggiungere un filtro tra di essi.

## Aggiungi un filtro tra due moduli:

1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra, quindi seleziona lo scenario per aprirlo.
1. Nell&#39;angolo superiore destro della finestra fare clic su **[!UICONTROL Modifica]**.
1. Fare clic sulla linea di connessione tra i moduli.
1. Nella casella visualizzata digitare un **[!UICONTROL Etichetta]** per il filtro.
1. Definisci una **[!UICONTROL Condizione]** filtro.

   Potete immettere uno o due operandi nelle due caselle. Se si immettono operandi in entrambe le caselle, è possibile selezionare un operatore nel menu a discesa tra di essi per specificare la relazione tra di essi.

   >[!TIP]
   >
   >Nei campi dell&#39;operando è possibile immettere i valori nello stesso modo in cui vengono mappati, come descritto in [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Ad esempio, se si desidera che il filtro trovi i file in [!DNL Adobe Workfront] che terminano con XML e li trasmetta a [!DNL Dropbox], immettere **[!UICONTROL Nome file]** nella prima casella e .**[!UICONTROL xml]** nella seconda casella. Nel menu a discesa tra di essi, selezionare **[!UICONTROL Termina con (senza distinzione maiuscole/minuscole)]**. Questo filtro si applica ai bundle in arrivo dal primo modulo (Workfront). Solo i bundle contenenti file XML passeranno al modulo successivo ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Fare clic su **[!DNL OK]**.

## Copiare un filtro

Attualmente, l’editor di scenari non include una funzione per copiare un filtro.

>[!NOTE]
>
>Se copi i moduli su entrambi i lati del filtro, viene copiato anche il filtro.
>
>Per ulteriori informazioni sulla copia dei moduli, vedere [Copiare moduli o scenari in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Per copiare un filtro senza copiare moduli, è possibile utilizzare [!DNL Google] Chrome per la seguente soluzione alternativa:

1. Installare l&#39;estensione [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome].
1. In [!DNL Workfront Fusion] aprire lo scenario.
1. Fai clic sul menu a tre punti di Chrome, quindi fai clic su **[!UICONTROL Altri strumenti*]* > **[!UICONTROL Strumenti per sviluppatori]**.

1. Nel pannello [!UICONTROL Strumenti per sviluppatori] visualizzato, nella barra dei menu nella parte superiore, fare clic sulla scheda [!UICONTROL Workfront Fusion].

   ![](assets/copy-a-filter-350x174.png)

1. Fai clic sull&#39;icona ![](assets/devtools-tools-icon.png) di **[!UICONTROL Strumenti]** nella barra laterale sinistra.

1. Fai clic su **[!UICONTROL Copia filtro]**, quindi configura lo strumento **[!UICONTROL Copia filtro]** nel pannello a destra:

   1. Imposta il **[!UICONTROL modulo Source]** come modulo subito dopo il filtro che desideri copiare.
   1. Imposta il **[!UICONTROL modulo di destinazione]** come modulo immediatamente prima del filtro da copiare.

1. Fare clic su **[!UICONTROL Esegui]**.

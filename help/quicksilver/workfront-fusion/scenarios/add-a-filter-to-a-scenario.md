---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Aggiungi un filtro a uno scenario in [!DNL Adobe] Workfront Fusion
description: In alcuni scenari, devi lavorare solo con bundle che soddisfano criteri specifici. I filtri ti consentono di selezionare tali bundle.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Aggiungi un filtro a uno scenario in [!DNL Adobe Workfront Fusion]

In alcuni scenari, devi lavorare solo con bundle che soddisfano criteri specifici. I filtri ti consentono di selezionare tali bundle.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Puoi aggiungere un filtro tra due moduli e verificare se i bundle ricevuti dai moduli precedenti soddisfano condizioni di filtro specifiche:

* In caso affermativo, i bundle passano al modulo successivo nello scenario .
* In caso contrario, l&#39;elaborazione dei bundle termina.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

È necessario aggiungere entrambi i moduli a uno scenario prima di poter aggiungere un filtro tra di essi.

## Aggiungi un filtro tra due moduli:

1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra, seleziona lo scenario da aprire.
1. Nell&#39;angolo superiore destro della finestra, fai clic su **[!UICONTROL Modifica]**.
1. Fare clic sulla linea di connessione tra i moduli.
1. Nella casella visualizzata, digita un **[!UICONTROL Etichetta]** per il filtro.
1. Definire un filtro **[!UICONTROL Condizione]**.

   È possibile immettere uno o due operandi nelle due caselle. Se si immettono operandi in entrambe le caselle, è possibile selezionare un operatore nel menu a discesa tra di essi per specificare la relazione tra di essi.

   >[!TIP]
   >
   >Nei campi dell&#39;operando è possibile immettere i valori nello stesso modo in cui li si esegue la mappatura, come descritto in [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Ad esempio, se desideri che il filtro trovi i file in [!DNL Adobe Workfront] terminazione con XML e trasmetterle a [!DNL Dropbox], inserisci **[!UICONTROL Nome file]** nella prima casella e .**[!UICONTROL xml]** nella seconda casella. Nel menu a discesa tra di essi, seleziona **[!UICONTROL Termina con (senza distinzione maiuscole/minuscole)]**. Questo filtro verrebbe applicato ai bundle in ingresso dal primo modulo (Workfront). Solo i bundle contenenti file XML passerebbero al modulo successivo ([!DNL Dropbox]).

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

1. Installa il [!UICONTROL [!DNL Adobe Workfront Fusion] Chrome DevTool] estensione.
1. In [!DNL Workfront Fusion], apri lo scenario .
1. Fai clic sul menu a tre punti di Chrome, quindi fai clic su **[!UICONTROL Altri strumenti*]* > **[!UICONTROL Strumenti per sviluppatori]**.

1. In [!UICONTROL Strumenti per sviluppatori] pannello visualizzato, nella barra dei menu nella parte superiore, fai clic sul pulsante [!UICONTROL Workfront Fusion] scheda .

   ![](assets/copy-a-filter-350x174.png)

1. Fai clic sul pulsante **[!UICONTROL Strumenti]** icona ![](assets/devtools-tools-icon.png) nella barra laterale sinistra.

1. Fai clic su **[!UICONTROL Filtro Copia]**, quindi configura il **[!UICONTROL Filtro Copia]** nel pannello laterale destro:

   1. Imposta la **[!UICONTROL Modulo di origine]** come modulo subito dopo il filtro da copiare.
   1. Imposta la **[!UICONTROL Modulo di destinazione]** come modulo immediatamente prima del filtro da copiare.

1. Fai clic su **[!UICONTROL Esegui]**.

---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copia moduli o scenari in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Copia moduli o scenari in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Copia moduli o scenari](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/copy-modules-or-scenarios.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

È possibile copiare moduli, gruppi di moduli o interi scenari in [!DNL Adobe Workfront Fusion]. Questa funzionalità consente di riutilizzare scenari o parti di scenari senza doverli ricreare

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

Per poterli copiare, è necessario aggiungere moduli a uno scenario.

## Copiare un modulo o un gruppo di moduli

Quando si copia un modulo, la copia mantiene tutti i valori e le impostazioni dei campi del modulo originale.

Puoi incollare il modulo o i moduli in un’altra area dello stesso scenario o in uno scenario diverso.

Quando si incollano moduli in uno scenario diverso, considera quanto segue.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Qualsiasi valore di campo che richiami informazioni da un altro modulo non copiato non può più accedere a tali informazioni. Devi impostare questi campi per estrarre informazioni dal nuovo scenario.
* Se si incollano i moduli in uno scenario di proprietà di un altro team o organizzazione, tutte le connessioni devono essere aggiornate alle connessioni di proprietà del gruppo o dell&#39;organizzazione proprietaria del nuovo scenario.

### Copia moduli

La copia di un gruppo di moduli è simile alla copia di un singolo modulo.

1. Fai clic con il pulsante destro del mouse sul modulo che desideri copiare.

   >[!NOTE]
   >
   >Per selezionare più moduli, tieni premuto [!UICONTROL shift] e fai clic sui moduli da copiare. Copiando un gruppo di moduli vengono copiate anche le linee di connessione, i filtri o la logica di routing tra di essi.

1. Seleziona **[!UICONTROL Copia modulo]**.
1. Spostare il cursore nell&#39;area dello scenario in cui si desidera copiare lo scenario.
1. Fare clic con il pulsante destro del mouse e selezionare **[!UICONTROL Incolla]**.
1. Connetti i moduli incollati allo scenario trascinandoli nella posizione appropriata nello scenario.

   È inoltre possibile utilizzare i tasti di scelta rapida per copiare e incollare.

## Copiare uno scenario tramite clonazione

La clonazione di uno scenario ne crea una copia, che potrai quindi modificare.

1. Apri la pagina dei dettagli dello scenario:

   1. Fai clic sulla scheda **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic su uno scenario su cui desideri visualizzare i dettagli.

      Oppure

      Se si sta lavorando sullo scenario in [Editor scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), fare clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Fai clic con il pulsante destro del mouse su **[!UICONTROL Opzioni]** in alto a destra della pagina.
1. Selezionare **[!UICONTROL Clone]**.
1. (Facoltativo) Immetti un nome per il nuovo scenario.
1. (Facoltativo) Abilita **[!UICONTROL Mantenere gli stati dei nuovi moduli uguali a quelli dei moduli duplicati]** per garantire che lo scenario copiato includa anche informazioni sui record più recenti elaborati dallo scenario originale.
1. Fai clic su **[!UICONTROL Salva]** per creare lo scenario.

## Copiare uno scenario utilizzando blueprint

I blueprint dello scenario rappresentano i valori di disposizione, mappatura e campi di uno scenario specifico in un determinato momento. Puoi esportare una blueprint di scenario in un file JSON sul computer, quindi importarla durante la creazione di un nuovo scenario. È possibile modificare gli scenari importati da una blueprint di scenario.

Una blueprint di scenario rappresenta l’intero scenario. Se desideri copiare solo determinati moduli da uno scenario, consulta [Copiare un modulo o un gruppo di moduli](#copy-a-module-or-a-group-of-modules) in questo articolo.

>[!NOTE]
>
>Per informazioni sui blueprint nel contesto di [!DNL Adobe Workfront], consulta [Panoramica sui blueprint](../../administration-and-setup/blueprints/blueprints-overview.md).

### Esportare una blueprint di scenario

1. Nello scenario, fai clic sul menu **[!UICONTROL Altro]** nell&#39;area delle impostazioni dello scenario.
1. Fai clic su **[!UICONTROL Esporta blueprint]**.

   Viene creato un file JSON che viene scaricato sul computer. È possibile individuare questo file nella cartella [!DNL Downloads].

### Importare una blueprint

>[!IMPORTANT]
>
>Se importi una blueprint in uno scenario esistente, la blueprint dello scenario sostituisce quello esistente. Non puoi aggiungere una blueprint a uno scenario esistente.

1. Inizia a creare un nuovo scenario.
1. Nello scenario, fai clic sul menu **[!UICONTROL Altro]** nell&#39;area delle impostazioni dello scenario.
1. Fai clic su **[!UICONTROL Importa blueprint]**.
1. Nella finestra di dialogo visualizzata, fai clic su **[!UICONTROL Sfoglia]**
1. Passare alla blueprint da importare e fare clic su **[!UICONTROL Apri]**.
1. Fai clic su **[!UICONTROL Salva]**.

   Viene creato un file JSON che viene scaricato sul computer. Puoi individuare questo file nella cartella [!UICONTROL Download].

## Copiare e riutilizzare gli scenari utilizzando i modelli

È possibile creare modelli come punto di partenza per gli scenari [!DNL Workfront Fusion]. Quando crei uno scenario da un modello, puoi modificarlo senza modificarlo. I valori dei campi non vengono salvati nei modelli.

Per ulteriori informazioni sulla creazione e l&#39;utilizzo dei modelli, vedere [Modelli di scenario](../../workfront-fusion/scenarios/templates/fusion-templates.md).

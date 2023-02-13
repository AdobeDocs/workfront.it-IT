---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copiare moduli o scenari in [!DNL Adobe Workfront Fusion]
description: Copiare moduli o scenari in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Copiare moduli o scenari in [!DNL Adobe Workfront Fusion]

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

È necessario aggiungere moduli a uno scenario prima di poterli copiare.

## Copiare un modulo o un gruppo di moduli

Quando si copia un modulo, la copia conserva tutti i valori e le impostazioni del campo del modulo originale.

È possibile incollare il modulo o i moduli in un&#39;altra area dello stesso scenario o in uno scenario diverso.

Quando si incollano moduli in uno scenario diverso, tenere presente quanto segue.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* I valori di campo che estraggono informazioni da un altro modulo non copiato non possono più accedere a tali informazioni. È necessario impostare questi campi per estrarre le informazioni dal nuovo scenario.
* Se si incollano i moduli in uno scenario di proprietà di un altro team o organizzazione, tutte le connessioni devono essere aggiornate alle connessioni di proprietà del gruppo o dell&#39;organizzazione proprietaria del nuovo scenario.

### Copiare i moduli

La copia di un gruppo di moduli è simile alla copia di un singolo modulo.

1. Fare clic con il pulsante destro del mouse sul modulo che si desidera copiare.

   >[!NOTE]
   >
   >È possibile selezionare più moduli tenendo premuto [!UICONTROL shift] e facendo clic sui moduli da copiare. Copiare un gruppo di moduli consente inoltre di copiare tra loro le linee di connessione, i filtri o la logica di routing.

1. Seleziona **[!UICONTROL Modulo copia]**.
1. Spostare il cursore nell’area dello scenario in cui si desidera copiare lo scenario.
1. Fai clic con il pulsante destro del mouse e seleziona **[!UICONTROL Incolla]**.
1. Collega i moduli incollati allo scenario trascinandoli nella posizione appropriata nello scenario.

   È inoltre possibile utilizzare le scelte rapide da tastiera per copiare e incollare.

## Copiare uno scenario tramite clonazione

Clonazione di uno scenario crea una copia dello scenario, che puoi quindi modificare.

1. Apri la pagina dei dettagli dello scenario:

   1. Fai clic sul pulsante **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic su uno scenario su cui desideri visualizzare i dettagli.

      Oppure

      Se si sta lavorando sullo scenario nel [Editor di scenari in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), fai clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Clic destro **[!UICONTROL Opzioni]** in alto a destra della pagina.
1. Seleziona **[!UICONTROL Clona]**.
1. (Facoltativo) Immetti un nome per il nuovo scenario.
1. (Facoltativo) Abilita **[!UICONTROL Mantenere gli stati di tutti i nuovi moduli uguali a quelli duplicati]** per garantire che lo scenario copiato includa anche informazioni sui record più recenti elaborati dallo scenario originale.
1. Fai clic su **[!UICONTROL Salva]** per creare lo scenario.

## Copiare uno scenario utilizzando le blueprint

I progetti scenario rappresentano la disposizione, la mappatura e i valori di campo di un dato scenario in un determinato momento. È possibile esportare una blueprint dello scenario in un file JSON sul computer, quindi importarla durante la creazione di un nuovo scenario. È possibile modificare gli scenari importati da una blueprint dello scenario.

Un modello di scenario rappresenta l&#39;intero scenario. Se desideri copiare solo alcuni moduli da uno scenario, consulta [Copiare un modulo o un gruppo di moduli](#copy-a-module-or-a-group-of-modules) in questo articolo.

>[!NOTE]
>
>Per informazioni sui progetti nel contesto di [!DNL Adobe Workfront], vedi [Panoramica delle blueprint](../../administration-and-setup/blueprints/blueprints-overview.md).

### Esportare una blueprint dello scenario

1. Nello scenario, fai clic su **[!UICONTROL Altro]** nell&#39;area delle impostazioni dello scenario.
1. Fai clic su **[!UICONTROL Esporta blueprint]**.

   Viene creato un file JSON da scaricare sul computer. Puoi individuare questo file nel tuo [!DNL Downloads] cartella.

### Importare una blueprint

>[!IMPORTANT]
>
>Se importi una blueprint in uno scenario esistente, la blueprint dello scenario sostituisce lo scenario esistente. Non è possibile aggiungere una blueprint a uno scenario esistente.

1. Inizia a creare un nuovo scenario.
1. Nello scenario, fai clic su **[!UICONTROL Altro]** nell&#39;area delle impostazioni dello scenario.
1. Fai clic su **[!UICONTROL Importa blueprint]**.
1. Nella finestra di dialogo visualizzata, fai clic su **[!UICONTROL Sfoglia]**
1. Passa alla blueprint da importare e fai clic su **[!UICONTROL Apri]**.
1. Fai clic su **[!UICONTROL Salva]**.

   Viene creato un file JSON da scaricare sul computer. Puoi individuare questo file nel tuo [!UICONTROL Download] cartella.

## Copiare e riutilizzare gli scenari utilizzando i modelli

Puoi creare modelli come punto di partenza per le [!DNL Workfront Fusion] scenari. Quando crei uno scenario da un modello, puoi modificarlo senza modificarlo. I valori dei campi non vengono salvati nei modelli.

Per ulteriori informazioni sulla creazione e l’utilizzo dei modelli, consulta [Modelli di scenario](../../workfront-fusion/scenarios/templates/fusion-templates.md).

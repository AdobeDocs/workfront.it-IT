---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Crea nuovi modelli in [!DNL Adobe Workfront Fusion]
description: È possibile creare nuovi modelli di scenario in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Crea nuovi modelli in [!DNL Adobe Workfront Fusion]

È possibile creare nuovi modelli di scenario in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Prima di creare un nuovo modello, puoi controllare la [!UICONTROL Modelli pubblici] per assicurarti che il modello che desideri creare non sia già disponibile.

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creare un nuovo modello

1. Fai clic su **[!UICONTROL Modelli]** ![](assets/fusion-template-icon.png) nel pannello di navigazione a sinistra.
1. Fai clic su **[!UICONTROL Creare un nuovo modello]** nell&#39;angolo in alto a destra.
1. (Facoltativo) Rinomina il modello sostituendo il modello predefinito **[!UICONTROL Nome nuovo modello]** nell&#39;angolo in alto a sinistra.
1. (Facoltativo) Per modificare la lingua del modello, fai clic su **[!UICONTROL Imposta un modello]** ![](assets/fusion-scenario-settings-icon.png) e seleziona la lingua dal menu a discesa Lingua .

   >[!IMPORTANT]
   >
   >La selezione Lingue corrisponde alle lingue disponibili nelle impostazioni del sistema e riguarda solo il nome del modello pubblico e la relativa descrizione. Non è possibile modificare una lingua del modello una volta salvato il modello.

1. (Facoltativo) Per inserire una descrizione del modello, fai clic su **[!UICONTROL Imposta un modello]** ![](assets/fusion-scenario-settings-icon.png) e immetti la descrizione.
1. Aggiungi app, moduli e strumenti nello stesso modo che faresti per creare uno scenario standard.

   Per aggiungere aiuto contestuale ai moduli, consulta [Configurazione [!UICONTROL Creazione guidata] funzionalità](#set-up-wizard-functionality) in questo articolo.

   Per ulteriori informazioni sulla creazione di uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se il modello include moduli che richiedono l’aggiunta della connessione, delle credenziali o di altre informazioni riservate, queste informazioni non vengono condivise con gli utenti del modello.

1. (Facoltativo) Fai clic su **[!UICONTROL Esegui una volta]** per testare il modello.
1. Fai clic sul pulsante **[!UICONTROL Salva]** icona ![](assets/save-icon.png).

>[!NOTE]
>
>Salvando il modello lo rendi visibile per tutti i membri del team. Se desideri che il modello sia accessibile al di fuori del team, devi pubblicarlo e quindi utilizzare un collegamento condiviso, oppure chiedere all’amministratore di approvare e pubblicare il modello.

## Configurazione [!UICONTROL Creazione guidata] funzionalità {#set-up-wizard-functionality}

La [!DNL Workfront Fusion template] [!UICONTROL Creazione guidata] consente di fornire agli utenti futuri del modello istruzioni o informazioni relative ai campi specifici utilizzati nei moduli.

1. Fai clic sul modulo aggiunto al modello per visualizzare i campi del modulo.
1. Individua il campo in cui desideri aggiungere [!UICONTROL Creazione guidata] informazioni e **[!UICONTROL Usa nella procedura guidata]** per quel campo.
1. Immetti le informazioni che desideri rendere visibili agli utenti nel [!UICONTROL Aiuto] campo .
1. (Facoltativo) Per consentire agli utenti di visualizzare questo testo quando utilizzano il modello, abilita **[!UICONTROL Usa come valore predefinito]**.
1. Ripetere i passaggi da 2 a 4 per ogni campo per il quale si desidera fornire informazioni.
1. Fai clic su **[!UICONTROL OK]** per salvare le modifiche e chiudere il modulo.

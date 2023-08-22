---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Creare nuovi modelli in [!DNL Adobe Workfront Fusion]
description: Puoi creare nuovi modelli di scenario in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Creare nuovi modelli in [!DNL Adobe Workfront Fusion]

Puoi creare nuovi modelli di scenario in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Prima di creare un nuovo modello, è possibile controllare [!UICONTROL Modelli pubblici] per accertarsi che il modello da creare non sia già disponibile.

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Crea un nuovo modello

È possibile creare un modello in un processo simile alla creazione di uno scenario. Gli amministratori di Fusion possono anche creare modelli da scenari esistenti.

* [Creare un modello](#build-a-template)
* [Creare un modello da uno scenario](#create-a-template-from-a-scenario)

### Creare un modello

1. Clic **[!UICONTROL Modelli]** ![](assets/fusion-template-icon.png) nel pannello di navigazione a sinistra.
1. Clic **[!UICONTROL Crea un nuovo modello]** nell’angolo superiore destro.
1. (Facoltativo) Rinomina il modello sostituendo il modello predefinito **[!UICONTROL Nome nuovo modello]** nell&#39;angolo superiore sinistro.
1. (Facoltativo) Per modificare la lingua del modello, fai clic su **[!UICONTROL Configurare un modello]** ![](assets/fusion-scenario-settings-icon.png) e seleziona la lingua dal menu a discesa Lingua.

   >[!IMPORTANT]
   >
   >La selezione Lingue corrisponde alle lingue disponibili nelle impostazioni di sistema e riguarda solo il nome del modello pubblico e la relativa descrizione. Una volta salvato il modello, non è possibile modificare il linguaggio del modello.

1. (Facoltativo) Per immettere una descrizione del modello, fare clic su **[!UICONTROL Configurare un modello]** ![](assets/fusion-scenario-settings-icon.png) e inserisci la descrizione.
1. Puoi aggiungere app, moduli e strumenti nello stesso modo in cui lo faresti quando crei uno scenario standard.

   Per aggiungere assistenza contestuale ai moduli, consulta [Configurazione [!UICONTROL Procedura guidata] funzionalità](#set-up-wizard-functionality) in questo articolo.

   Per ulteriori informazioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se il modello include moduli che richiedono l’aggiunta di connessione, credenziali o altre informazioni riservate, queste informazioni non vengono condivise con gli utenti del modello.

1. (Facoltativo) Fai clic su **[!UICONTROL Esegui una volta]** per testare il modello.
1. Fai clic su **[!UICONTROL Salva]** icona ![](assets/save-icon.png).

>[!NOTE]
>
>Salvando il modello sarà possibile renderlo visibile a tutti i membri del team. Se desideri che il modello sia accessibile all’esterno del team, devi inviare una richiesta per far sì che sia approvato e pubblicato. La richiesta viene inviata ad Adobe Workfront per l’approvazione e, una volta approvato, il modello è accessibile ad altri utenti esterni al team.
>
>Per informazioni sulla pubblicazione dei modelli, consulta [Pubblica e condividi [!DNL Adobe Workfront Fusion] modelli](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Creare un modello da uno scenario

>[!NOTE]
>
>Per creare un modello da uno scenario, è necessario essere un amministratore di Fusion.

1. Aprire la pagina dei dettagli dello scenario da cui si desidera creare uno scenario.
1. Fai clic su **Amministratore** menu a discesa vicino all’angolo superiore destro della pagina.
1. Seleziona **Clona come modello**.

   Lo scenario viene copiato in una pagina Nuovo modello.
1. (Facoltativo) Rinomina il modello sostituendo il modello predefinito **[!UICONTROL Nome nuovo modello]** nell&#39;angolo superiore sinistro.
1. (Facoltativo) Per modificare la lingua del modello, fai clic su **[!UICONTROL Configurare un modello]** ![](assets/fusion-scenario-settings-icon.png) e seleziona la lingua dal menu a discesa Lingua.

   >[!IMPORTANT]
   >
   >La selezione Lingue corrisponde alle lingue disponibili nelle impostazioni di sistema e riguarda solo il nome del modello pubblico e la relativa descrizione. Una volta salvato il modello, non è possibile modificare il linguaggio del modello.

1. (Facoltativo) Per immettere una descrizione del modello, fare clic su **[!UICONTROL Configurare un modello]** ![](assets/fusion-scenario-settings-icon.png) e inserisci la descrizione.
1. Modifica app, moduli e strumenti nello stesso modo in cui effettui la modifica di uno scenario standard.

   Per aggiungere assistenza contestuale ai moduli, consulta [Configurazione [!UICONTROL Procedura guidata] funzionalità](#set-up-wizard-functionality) in questo articolo.

   >[!NOTE]
   >
   >Se il modello include moduli che richiedono l’aggiunta di connessione, credenziali o altre informazioni riservate, queste informazioni non vengono condivise con gli utenti del modello.

1. (Facoltativo) Fai clic su **[!UICONTROL Esegui una volta]** per testare il modello.
1. Fai clic su **[!UICONTROL Salva]** icona ![](assets/save-icon.png).

## Configurazione [!UICONTROL Procedura guidata] funzionalità {#set-up-wizard-functionality}

Il [!DNL Workfront Fusion template] [!UICONTROL Procedura guidata] consente di fornire agli utenti futuri del modello istruzioni o informazioni relative ai campi specifici utilizzati nei moduli.

1. Fai clic sul modulo aggiunto al modello per visualizzare i campi del modulo.
1. Individua il campo in cui desideri aggiungere [!UICONTROL Procedura guidata] e abilitare **[!UICONTROL Uso in procedura guidata]** per quel campo.
1. Immettere le informazioni che si desidera rendere visibili agli utenti nel [!UICONTROL Aiuto] campo.
1. (Facoltativo) Per consentire agli utenti di visualizzare questo testo quando utilizzano il modello, abilita **[!UICONTROL Usa come valore predefinito]**.
1. Ripetere i passaggi da 2 a 4 per ogni campo per il quale si desidera fornire informazioni.
1. Clic **[!UICONTROL OK]** per salvare le modifiche e chiudere il modulo.

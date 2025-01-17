---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Crea nuovi modelli in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Crea nuovi modelli in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Crea nuovi modelli](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-and-manage-templates/create-new-fusion-templates.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

È possibile creare nuovi modelli di scenario in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Prima di creare un nuovo modello, è possibile controllare la scheda [!UICONTROL Modelli pubblici] per assicurarsi che il modello che si desidera creare non sia già disponibile.

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

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Crea un nuovo modello

È possibile creare un modello in un processo simile alla creazione di uno scenario. Gli amministratori di Fusion possono anche creare modelli da scenari esistenti.

* [Creare un modello](#build-a-template)
* [Creare un modello da uno scenario](#create-a-template-from-a-scenario)

### Creare un modello

1. Fai clic su **[!UICONTROL Modelli]** ![](assets/fusion-template-icon.png) nel pannello di navigazione a sinistra.
1. Fai clic su **[!UICONTROL Crea un nuovo modello]** nell&#39;angolo superiore destro.
1. (Facoltativo) Rinominare il modello sostituendo il **[!UICONTROL Nome nuovo modello]** predefinito nell&#39;angolo superiore sinistro.
1. (Facoltativo) Per modificare la lingua del modello, fare clic su **[!UICONTROL Configura un modello]** ![](assets/fusion-scenario-settings-icon.png) e selezionare la lingua dal menu a discesa Lingua.

   >[!IMPORTANT]
   >
   >La selezione Lingue corrisponde alle lingue disponibili nelle impostazioni di sistema e riguarda solo il nome del modello pubblico e la relativa descrizione. Una volta salvato il modello, non è possibile modificare il linguaggio del modello.

1. (Facoltativo) Per immettere una descrizione del modello, fare clic su **[!UICONTROL Configura un modello]** ![](assets/fusion-scenario-settings-icon.png) e immettere la descrizione.
1. Puoi aggiungere app, moduli e strumenti nello stesso modo in cui lo faresti quando crei uno scenario standard.

   Per aggiungere informazioni contestuali ai moduli, vedere [Configurare la funzionalità [!UICONTROL Wizard]](#set-up-wizard-functionality) in questo articolo.

   Per ulteriori informazioni sulla creazione di uno scenario, vedere [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se il modello include moduli che richiedono l’aggiunta di connessione, credenziali o altre informazioni riservate, queste informazioni non vengono condivise con gli utenti del modello.

1. (Facoltativo) Fai clic su **[!UICONTROL Esegui una volta]** per verificare il modello.
1. Fai clic sull&#39;icona **[!UICONTROL Salva]** ![](assets/save-icon.png).

>[!NOTE]
>
>Salvando il modello sarà possibile renderlo visibile a tutti i membri del team. Se desideri che il modello sia accessibile all’esterno del team, devi inviare una richiesta per far sì che sia approvato e pubblicato. La richiesta viene inviata ad Adobe Workfront per l’approvazione e, una volta approvato, il modello è accessibile ad altri utenti esterni al team.
>
>Per informazioni sulla pubblicazione di modelli, vedere [Publish e condividere [!DNL Adobe Workfront Fusion] modelli](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Creare un modello da uno scenario

>[!NOTE]
>
>Per creare un modello da uno scenario, è necessario essere un amministratore di Fusion.

1. Aprire la pagina dei dettagli dello scenario da cui si desidera creare uno scenario.
1. Fai clic sul menu a discesa **Amministratore** nell&#39;angolo superiore destro della pagina.
1. Seleziona **Clona come modello**.

   Lo scenario viene copiato in una pagina Nuovo modello.
1. (Facoltativo) Rinominare il modello sostituendo il **[!UICONTROL Nome nuovo modello]** predefinito nell&#39;angolo superiore sinistro.
1. (Facoltativo) Per modificare la lingua del modello, fare clic su **[!UICONTROL Configura un modello]** ![](assets/fusion-scenario-settings-icon.png) e selezionare la lingua dal menu a discesa Lingua.

   >[!IMPORTANT]
   >
   >La selezione Lingue corrisponde alle lingue disponibili nelle impostazioni di sistema e riguarda solo il nome del modello pubblico e la relativa descrizione. Una volta salvato il modello, non è possibile modificare il linguaggio del modello.

1. (Facoltativo) Per immettere una descrizione del modello, fare clic su **[!UICONTROL Configura un modello]** ![](assets/fusion-scenario-settings-icon.png) e immettere la descrizione.
1. Modifica app, moduli e strumenti nello stesso modo in cui effettui la modifica di uno scenario standard.

   Per aggiungere informazioni contestuali ai moduli, vedere [Configurare la funzionalità [!UICONTROL Wizard]](#set-up-wizard-functionality) in questo articolo.

   >[!NOTE]
   >
   >Se il modello include moduli che richiedono l’aggiunta di connessione, credenziali o altre informazioni riservate, queste informazioni non vengono condivise con gli utenti del modello.

1. (Facoltativo) Fai clic su **[!UICONTROL Esegui una volta]** per verificare il modello.
1. Fai clic sull&#39;icona **[!UICONTROL Salva]** ![](assets/save-icon.png).

## Configura funzionalità [!UICONTROL Wizard] {#set-up-wizard-functionality}

La [!DNL Workfront Fusion template] [!UICONTROL procedura guidata] consente di fornire agli utenti futuri del modello istruzioni o informazioni relative ai campi specifici utilizzati nei moduli.

1. Fai clic sul modulo aggiunto al modello per visualizzare i campi del modulo.
1. Individuare il campo in cui si desidera aggiungere le informazioni della [!UICONTROL Procedura guidata] e abilitare **[!UICONTROL Utilizza nella procedura guidata]** per tale campo.
1. Immettere le informazioni da rendere visibili agli utenti nel campo [!UICONTROL Guida].
1. (Facoltativo) Per consentire agli utenti di visualizzare questo testo quando utilizzano il modello, abilitare **[!UICONTROL Usa come valore predefinito]**.
1. Ripetere i passaggi da 2 a 4 per ogni campo per il quale si desidera fornire informazioni.
1. Fare clic su **[!UICONTROL OK]** per salvare le modifiche e chiudere il modulo.

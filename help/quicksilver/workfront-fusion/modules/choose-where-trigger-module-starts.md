---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Scegli dove inizia un modulo trigger in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# Scegli dove inizia un modulo trigger in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Scegli dove inizia un modulo trigger](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/choose-where-trigger-module-starts.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Alcuni moduli di attivazione ti consentono di selezionare il primo bundle da cui desideri avviare il recupero dei bundle.

Puoi anche specificare se recuperare tutti i bundle o solo i bundle da dopo una data specifica.

Per ulteriori informazioni sui moduli trigger, vedere la sezione [Moduli trigger](../../workfront-fusion/modules/module-types.md#triggers) nell&#39;articolo [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
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
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Scegli dove inizia un modulo trigger

1. Salva un modulo trigger.

   Oppure

   Modificare le impostazioni del modulo trigger come descritto in [Configurare le impostazioni di un modulo in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Oppure

   Fare clic con il pulsante destro del mouse sull&#39;icona del modulo trigger nell&#39;[!UICONTROL Editor scenari], come descritto in [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Selezionare un&#39;opzione nella casella **[!UICONTROL Scegli da dove iniziare]** visualizzata.

   ![](assets/choose-where-to-start-350x346.jpg)

   Le opzioni visualizzate dipendono dalle possibilità di un determinato servizio. Esse possono comprendere quanto segue:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Da ora in avanti] (impostazione predefinita)</td>
            <td>Recupera tutti i bundle aggiunti o aggiornati (a seconda delle impostazioni) da ora in poi</td>
        </tr>
        <tr>
            <td>[!UICONTROL Da dopo una data specifica]</td>
            <td>Recupera tutti i bundle aggiunti o aggiornati (a seconda delle impostazioni) dopo una data/ora specificata</td>
        </tr>
        <tr>
            <td>[!UICONTROL Con ID maggiore o uguale a un valore specifico]</td>
            <td>Recupera tutti i bundle con un ID maggiore o uguale a un ID specificato</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Tutti i bundle]</td>
            <td>Recupera tutti i bundle disponibili</td>
        </tr>
        <tr>
            <td>[!UICONTROL Seleziona il primo bundle]</td>
            <td>Consente di selezionare il primo bundle dal quale deve iniziare il recupero dei bundle</td>
        </tr>
   </table>

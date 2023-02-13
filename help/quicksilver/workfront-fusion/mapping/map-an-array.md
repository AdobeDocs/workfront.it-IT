---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappare un array in [!DNL Adobe] Workfront Fusion
description: È possibile mappare un array a un campo modulo in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Mappare un array in [!DNL Adobe Workfront Fusion]

Un array è un tipo speciale di elemento che può contenere quanto segue:

* Uno o più valori di testo (matrice semplice)
* Una o più raccolte dello stesso tipo (array complesso)

>[!INFO]
>
>**Esempio:** La [!UICONTROL Guarda le e-mail] modulo restituisce un array di allegati per ogni e-mail. Ogni allegato rappresenta una raccolta che può contenere un nome, un contenuto, una dimensione e così via.

Per ulteriori informazioni, consulta [Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappare un array

1. Fai clic sul pulsante situato nel campo di destinazione.

   >[!INFO]
   >
   >  **Esempio:** Per l’esempio precedente, fai clic sul pulsante [!UICONTROL Aggiungere un allegato] per un messaggio e-mail.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Nella casella visualizzata, immettere l&#39;elemento.

   Il pannello ti consente di mappare i campi nello stesso modo di qualsiasi altro tipo di elemento. Se non si desidera compilare ciascun elemento separatamente, ma si desidera mappare un altro array nel campo di destinazione, utilizzare il [!UICONTROL Mappa] pulsante . In questo caso, assicurarsi che entrambi gli array (l&#39;array di origine e l&#39;array di destinazione) abbiano la stessa struttura.

   È possibile aggiungere qualsiasi numero di elementi a una matrice.

È possibile dividere un array in singoli bundle utilizzando un iteratore. Per ulteriori informazioni, consulta [[!UICONTROL Iteratore] modulo in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

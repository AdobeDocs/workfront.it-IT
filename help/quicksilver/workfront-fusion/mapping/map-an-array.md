---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappare un array in [!DNL Adobe] Workfront Fusion
description: È possibile mappare un array su un campo modulo in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Mappa un array in [!DNL Adobe Workfront Fusion]

Un array è un tipo speciale di elemento che può contenere i seguenti elementi:

* Uno o più valori di testo (array semplice)
* Una o più raccolte dello stesso tipo (array complesso)

>[!INFO]
>
>**Esempio:** Il modulo [!UICONTROL Controlla e-mail] restituisce un array di allegati per ogni e-mail. Ogni allegato rappresenta una raccolta che può contenere un nome, contenuto, dimensioni e così via.

Per ulteriori informazioni, vedere [Tipi di dati elemento in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mappare un array

1. Fai clic sul pulsante che si trova nel campo di destinazione.

   >[!INFO]
   >
   >  **Esempio:** Per l&#39;esempio precedente, fare clic sul pulsante [!UICONTROL Aggiungi un allegato] per un&#39;e-mail.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Nella casella visualizzata immettere l&#39;elemento.

   Il pannello consente di mappare i campi allo stesso modo di qualsiasi altro tipo di elemento. Se non desideri compilare ogni elemento separatamente, ma vuoi mappare un altro array nel campo di destinazione, utilizza il pulsante [!UICONTROL Mappa]. In questo caso, assicurarsi che entrambe le matrici (l&#39;array di origine e l&#39;array di destinazione) abbiano la stessa struttura.

   È possibile aggiungere un numero qualsiasi di elementi a un array.

Potete dividere una matrice in singoli bundle utilizzando un iteratore. Per ulteriori informazioni, vedere il modulo [[!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

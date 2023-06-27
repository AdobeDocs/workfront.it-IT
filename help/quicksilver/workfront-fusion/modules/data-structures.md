---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Strutture di dati in [!DNL Adobe Workfront Fusion]
description: Una struttura di dati è un documento che descrive in dettaglio il formato dei dati trasferiti ad Adobe Workfront Fusion. In base a questo documento, l’editor di scenari è in grado di capire quale modulo restituisce o riceve quale tipo di dati. I documenti della struttura dati vengono utilizzati in genere per la serializzazione/analisi dei formati di dati come JSON, XML, CSV e altri.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Strutture di dati in [!DNL Adobe Workfront Fusion]

Una struttura di dati è un documento che descrive in dettaglio il formato dei dati trasferiti a [!DNL Adobe Workfront Fusion]. In base a questo documento, l’editor di scenari è in grado di capire quale modulo restituisce o riceve quale tipo di dati. I documenti della struttura dati vengono utilizzati in genere per la serializzazione/analisi dei formati di dati come JSON, XML, CSV e altri.

Per creare una struttura di dati, fai clic su [!UICONTROL Creare una nuova struttura dati] pulsante in [!UICONTROL Panoramica sulla struttura dei dati] o nelle impostazioni del modulo che richiedono le specifiche della struttura dati.

I tipi di dati supportati sono descritti nel [[!UICONTROL Tipi di moduli]](../../workfront-fusion/modules/module-types.md) articolo.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Generatore struttura dati

Non è sempre necessario creare strutture di dati. Puoi semplificarlo utilizzando un modello del nostro generatore incorporato. Fornendo un esempio di dati, il generatore crea automaticamente una struttura di dati in base al campione di dati immesso. La struttura dati creata può quindi essere modificata manualmente.

![](assets/data-structure-generator-350x341.jpg)

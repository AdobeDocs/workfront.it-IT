---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Ricevere un webhook da un servizio Web
description: Se un servizio Web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l'invio di webhook, è possibile aggiungerlo a uno scenario utilizzando il modulo Web hook personalizzato come trigger immediato.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Ricevere un webhook da un servizio Web

Se un servizio Web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l&#39;invio di webhook, è possibile aggiungerlo a uno scenario utilizzando il modulo Web hook personalizzato come trigger immediato.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
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

## Ricevi un webhook

1. Aggiungi il modulo **[!UICONTROL Webhook] >[!UICONTROL Webhook personalizzato]** allo scenario.
1. Fai clic su **[!UICONTROL Aggiungi]**, digita un **[!UICONTROL nome webhook]** nella casella visualizzata, quindi fai clic su **[!UICONTROL Salva]**.

1. Fai clic su **[!UICONTROL Copia indirizzo negli Appunti]**, quindi fai clic su **[!UICONTROL OK]**.

1. Accedi al servizio web ed effettua le seguenti operazioni:

   1. Creare un webhook nell&#39;area [!UICONTROL Impostazioni] del servizio Web.
   1. Incolla l&#39;indirizzo copiato negli Appunti al punto 3.
   1. Seleziona l’evento che attiverà il webhook.

1. Nello scenario [!DNL Workfront Fusion], specificare l&#39;evento o gli eventi che si desidera attivare il modulo [!UICONTROL Webhook personalizzato].
1. Esegui lo scenario.

   Quando si verificano l&#39;evento o gli eventi, il modulo [!UICONTROL Webhook personalizzato] viene attivato e lo scenario viene eseguito.

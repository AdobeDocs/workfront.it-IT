---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Ricevere un webhook da un servizio Web
description: Se un servizio web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l’invio di webhook, puoi aggiungere il servizio a uno scenario utilizzando il modulo Webhook personalizzato come attivatore immediato.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Ricevere un webhook da un servizio Web

Se un servizio web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l’invio di webhook, puoi aggiungere il servizio a uno scenario utilizzando il modulo Webhook personalizzato come attivatore immediato.

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

## Ricevi un webhook

1. Aggiungi il **[!UICONTROL Webhook] >[!UICONTROL Webhook personalizzato]** al tuo scenario.
1. Clic **[!UICONTROL Aggiungi]**, digitare a **[!UICONTROL Nome webhook]** nella casella visualizzata, fai clic su **[!UICONTROL Salva]**.

1. Clic **[!UICONTROL Copia indirizzo negli Appunti]**, quindi fai clic su **[!UICONTROL OK]**.

1. Accedi al servizio web ed effettua le seguenti operazioni:

   1. In [!UICONTROL Impostazioni] per il servizio web, crea un webhook.
   1. Incolla l&#39;indirizzo copiato negli Appunti al punto 3.
   1. Seleziona l’evento che attiverà il webhook.

1. In [!DNL Workfront Fusion] , specificare l&#39;evento o gli eventi che si desidera attivare [!UICONTROL Webhook personalizzato] modulo.
1. Esegui lo scenario.

   Quando si verificano l&#39;evento o gli eventi, [!UICONTROL Webhook personalizzato] e lo scenario viene eseguito.

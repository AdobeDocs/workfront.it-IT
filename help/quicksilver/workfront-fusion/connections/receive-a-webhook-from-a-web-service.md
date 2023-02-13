---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Ricevere un webhook da un servizio Web
description: Se un servizio Web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l’invio di webhook, puoi aggiungere il servizio a uno scenario utilizzando il modulo webhook personalizzato come attivatore immediato.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Ricevere un webhook da un servizio Web

Se un servizio Web non è attualmente implementato come app in [!DNL Adobe Workfront Fusion], ma supporta l’invio di webhook, puoi aggiungere il servizio a uno scenario utilizzando il modulo webhook personalizzato come attivatore immediato.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ricevere un webhook

1. Aggiungi il **[!UICONTROL Webhook] >[!UICONTROL Webhook personalizzato]** al tuo scenario.
1. Fai clic su **[!UICONTROL Aggiungi]**, digitare a **[!UICONTROL Nome Webhook]** nella casella visualizzata, quindi fai clic su **[!UICONTROL Salva]**.

1. Fai clic su **[!UICONTROL Copia indirizzo negli Appunti]**, quindi fai clic su **[!UICONTROL OK]**.

1. Accedi al servizio Web ed effettua le seguenti operazioni:

   1. In [!UICONTROL Impostazioni] area per il servizio Web, creare un webhook.
   1. Incolla l’indirizzo copiato negli Appunti al passaggio 3 .
   1. Seleziona l&#39;evento che attiverà il webhook.

1. In [!DNL Workfront Fusion] specificare l&#39;evento o gli eventi che si desidera attivare [!UICONTROL Webhook personalizzato] modulo .
1. Esegui lo scenario.

   Quando si verifica l&#39;evento o gli eventi, la [!UICONTROL Webhook personalizzato] Viene attivato il modulo e lo scenario viene eseguito.

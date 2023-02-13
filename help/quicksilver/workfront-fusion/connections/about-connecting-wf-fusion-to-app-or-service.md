---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un'app o a un servizio
description: Per la maggior parte delle app, è necessario creare una connessione, attraverso la quale [!DNL Adobe Workfront Fusion] può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un&#39;app o a un servizio

Per la maggior parte delle app, è necessario creare una connessione, attraverso la quale [!DNL Adobe Workfront Fusion] può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.

Ad esempio, se desideri creare uno scenario che recuperi informazioni da [!DNL Workfront], devi concedere l’autorizzazione di accesso per [!DNL Workfront Fusion] per accedere al [!DNL Workfront] conto.

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

## Diritti di accesso

Per ogni connessione, [!DNL Workfront Fusion] richiede solo i diritti di accesso necessari per completare con successo un dato scenario. Ad esempio, se si crea uno scenario per elencare i documenti da [!DNL Google Docs], [!DNL Workfront Fusion] non richiede l&#39;autorizzazione per ottenere il contenuto dei documenti.

Sfortunatamente, non tutti i servizi ti consentono di limitare l’accesso a attività specifiche. Pertanto, [!DNL Workfront Fusion] devono richiedere pieni diritti di accesso. Per ulteriori informazioni su come limitare [!DNL Workfront Fusion] accedere al tuo account registrato a tali servizi, consulta la documentazione specifica dell’applicazione.

## Informazioni sull’amministrazione delle connessioni

Puoi amministrare tutte le connessioni dal [!UICONTROL Connessioni] area. Qui puoi:

* Vedi quali autorizzazioni sono state assegnate a [!DNL Workfront Fusion] per ogni connessione
* Rinomina connessioni
* Autorizzare nuovamente le connessioni esistenti
* Elimina connessioni esistenti
* Verificare che la connessione al servizio sia stata stabilita correttamente

Per aprire [!UICONTROL Connessioni] area, fai clic su <b>[!UICONTROL Connessioni]</b> nella navigazione a sinistra.

## Rinnovare una connessione

[!DNL Workfront Fusion] di solito ottiene diritti di accesso a un determinato servizio per un periodo di tempo illimitato. Tuttavia, non è sempre così. Per alcuni servizi, l&#39;autorizzazione di accesso deve essere rinnovata dopo un certo periodo di tempo. In questi casi, [!DNL Workfront Fusion] ti informa via e-mail poco prima della scadenza dei suoi diritti di accesso.

Per rinnovare una connessione:

1. Fai clic sul pulsante **[!UICONTROL Riautorizzare]** nel **[!UICONTROL Connessioni]** area.

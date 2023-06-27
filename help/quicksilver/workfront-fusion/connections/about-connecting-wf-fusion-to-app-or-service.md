---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un’app o a un servizio
description: Per la maggior parte delle app, è necessario creare una connessione, attraverso la quale [!DNL Adobe Workfront Fusion] può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un’app o a un servizio

Per la maggior parte delle app, è necessario creare una connessione, attraverso la quale [!DNL Adobe Workfront Fusion] può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.

Ad esempio, se desideri creare uno scenario da cui recuperare informazioni [!DNL Workfront], devi concedere l’autorizzazione di accesso per [!DNL Workfront Fusion] per accedere al [!DNL Workfront] account.

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

## Diritti di accesso

Per ogni connessione, [!DNL Workfront Fusion] richiede solo i diritti di accesso necessari per completare correttamente uno scenario specifico. Ad esempio, se si crea uno scenario da cui elencare i documenti [!DNL Google Docs], [!DNL Workfront Fusion] non richiede l’autorizzazione per ottenere il contenuto dei documenti.

Sfortunatamente, non tutti i servizi consentono di limitare l’accesso ad attività specifiche. Pertanto, [!DNL Workfront Fusion] deve richiedere diritti di accesso completi. Per ulteriori informazioni su come limitare [!DNL Workfront Fusion] accedere all’account registrato per tali servizi, consulta la documentazione specifica per l’applicazione.

## Informazioni sull&#39;amministrazione delle connessioni

È possibile amministrare tutte le connessioni da [!UICONTROL Connessioni] area. Qui è possibile:

* Scopri a quali autorizzazioni sono state assegnate [!DNL Workfront Fusion] per ogni connessione
* Rinominare le connessioni
* Riautorizza connessioni esistenti
* Elimina connessioni esistenti
* Verificare che la connessione al servizio sia stata stabilita correttamente

Per aprire [!UICONTROL Connessioni] , fare clic su <b>[!UICONTROL Connessioni]</b> nel menu di navigazione a sinistra.

## Rinnovare una connessione

[!DNL Workfront Fusion] di solito ottiene i diritti di accesso a un determinato servizio per un periodo di tempo illimitato. Tuttavia, non sempre è così. Con alcuni servizi, l’autorizzazione di accesso deve essere rinnovata dopo un determinato periodo di tempo. In questi casi, [!DNL Workfront Fusion] invia una notifica via e-mail poco prima della scadenza dei diritti di accesso.

Per rinnovare una connessione:

1. Fai clic su **[!UICONTROL Riautorizza]** pulsante in **[!UICONTROL Connessioni]** area.

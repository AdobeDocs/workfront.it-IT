---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Panoramica delle connessioni
description: Per la maggior parte delle app, è necessario creare una connessione, attraverso la quale [!DNL Adobe Workfront Fusion] può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Panoramica delle connessioni

<!-- Audited: 3/2024-->

Per la maggior parte delle app, [!DNL Workfront Fusion] richiede una connessione, attraverso la quale può comunicare con il servizio di terze parti specificato in base alle impostazioni dello scenario specifico.

Ad esempio, se desideri creare uno scenario da cui recuperare informazioni [!DNL Workfront], devi concedere l’autorizzazione di accesso per [!DNL Workfront Fusion] per accedere al [!DNL Workfront] account.

Una connessione rappresenta l&#39;autorizzazione e le autorizzazioni utilizzate da Fusion per accedere all&#39;applicazione. È possibile creare una o più connessioni per ogni applicazione e utilizzare la stessa connessione in più moduli o scenari.

La maggior parte delle connessioni viene utilizzata solo per una singola applicazione. Ad esempio, un [!DNL Workfront] connessione non può essere utilizzata in un [!UICONTROL Salesforce] modulo. Alcuni [!DNL Adobe] Le applicazioni possono condividere le connessioni. Per ulteriori informazioni, vedere gli articoli relativi alle applicazioni elencate in [App e relativi moduli](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Le connessioni vengono gestite a livello di team. Tutti i membri di un team hanno accesso alle connessioni del team e gli utenti all&#39;esterno di un team non hanno accesso alle connessioni del team.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Legacy: qualsiasi </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Nuovo:</p> <ul><li>[!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront] Piano: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Piano: [!DNL Workfront Fusion] è incluso.</li></ul>
   <p>Oppure</p>
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Diritti di accesso

Per ogni connessione, [!DNL Workfront Fusion] richiede solo i diritti di accesso necessari per completare correttamente uno scenario specifico. Ad esempio, se si crea uno scenario da cui elencare i documenti [!DNL Google Docs], [!DNL Workfront Fusion] non richiede l’autorizzazione per ottenere il contenuto dei documenti. In seguito, se si scopre che è necessario accedere al contenuto dei documenti, è possibile aggiornare la connessione o crearne una nuova che possa accedere a tale contenuto.

Non tutti i servizi consentono di limitare l’accesso ad attività specifiche. In questi casi, [!DNL Workfront Fusion] deve richiedere diritti di accesso completi. Per ulteriori informazioni su come limitare [!DNL Workfront Fusion] accedere all’account registrato per tali servizi, consulta la documentazione specifica per l’applicazione elencata in [App e relativi moduli](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Gestire le connessioni

Puoi gestire tutte le connessioni da [!UICONTROL Connessioni] area.

>[!NOTE]
>
>Le connessioni sono di proprietà dei team. Se non riesci a trovare la connessione che stai cercando, controlla che tu stia visualizzando il team corretto.
>
>Per selezionare un nuovo team:
>
>* Fai clic sul nome del team nella barra di navigazione a sinistra e seleziona un nuovo team.
>
>    Oppure
>
>* Fai clic su Panoramica team nel menu di navigazione a sinistra, quindi fai clic sulla freccia a discesa accanto al nome del team nella parte superiore della pagina. Selezionare un nuovo team.

1. Per aprire [!UICONTROL Connessioni] , fare clic su <b>[!UICONTROL Connessioni]</b> nel menu di navigazione a sinistra.
1. (Facoltativo) Indica l’ambiente e il tipo di connessione facendo clic sul menu a discesa Ambiente e tipo e selezionando un’opzione.
1. (Facoltativo) Per visualizzare quali autorizzazioni sono state concesse a [!DNL Workfront Fusion] per una connessione, fai clic sull’icona Visualizza ![Visualizza autorizzazioni di connessione](assets/view-connection-permissions.png) per quella connessione.
1. (Facoltativo) Per rinominare una connessione, evidenziarne il nome e digitare il nuovo nome.
1. (Facoltativo) Per autorizzare nuovamente una connessione, fai clic su **Riautorizza** per quella connessione.
1. (Facoltativo) Per eliminare una connessione, fai clic su **Elimina** per quella connessione.
1. (Facoltativo) Per verificare che la connessione al servizio sia stata stabilita correttamente, fai clic su **Verifica** per la connessione.



## Rinnovare una connessione

[!DNL Workfront Fusion] di solito ottiene i diritti di accesso a un determinato servizio per un periodo di tempo illimitato. Alcune applicazioni richiedono il rinnovo dell’autorizzazione di accesso dopo un determinato periodo di tempo. In questi casi, [!DNL Workfront Fusion] invia una notifica via e-mail poco prima della scadenza dei diritti di accesso.

Per rinnovare una connessione:

1. Fai clic su **[!UICONTROL Riautorizza]** pulsante in **[!UICONTROL Connessioni]** area.

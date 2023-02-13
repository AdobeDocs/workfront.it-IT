---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: connections-annd-webhooks
title: Crea connessioni in [!DNL Adobe Workfront Fusion]
description: Una connessione deve rispettare i requisiti impostati dall’API dell’app o del servizio Web a cui si connette. Per questo motivo, le istruzioni per l'impostazione di una connessione variano in base all'app o al servizio Web. Questo articolo può aiutarti a identificare e individuare le istruzioni per la connessione [!DNL Adobe Workfront Fusion] all'app o al servizio Web scelto.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Crea connessioni in [!DNL Adobe Workfront Fusion]

Una connessione deve rispettare i requisiti impostati dall’API dell’app o del servizio Web a cui si connette. Per questo motivo, le istruzioni per l&#39;impostazione di una connessione variano in base all&#39;app o al servizio Web. Questo articolo può aiutarti a identificare e individuare le istruzioni per la connessione [!DNL Adobe Workfront Fusion] all&#39;app o al servizio Web scelto.

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

</tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connetti [!DNL Adobe Workfront] a [!DNL Workfront Fusion]

Workfront e [!DNL Workfront Fusion] sono progettati per funzionare insieme. La connessione creata determina l&#39;account che [!DNL Workfront Fusion] utilizza per eseguire azioni in Workfront.

Per istruzioni, consulta [Connetti [!DNL Workfront] a [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] moduli](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## Connettersi a un&#39;app o a un servizio Web che non richiede la configurazione

Nella maggior parte dei casi, è possibile utilizzare il modulo per creare una connessione con poche o nessuna informazione aggiuntiva. [!DNL Workfront Fusion] gestisce automaticamente l&#39;autenticazione.

Per istruzioni su come creare una connessione senza considerazioni speciali, consulta [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Connessione a un [!DNL Microsoft] app o servizio Web

La maggior parte dei [!DNL Microsoft] app in [!DNL Workfront Fusion] consente di creare una connessione senza ulteriori informazioni.

Le seguenti circostanze richiedono passaggi aggiuntivi per la creazione di una connessione:

* Utilizzo [!DNL Microsoft Dynamics 365] moduli.

   Per istruzioni, consulta [[!DNL Microsoft Dynamics 365] moduli](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Collegamento al [!DNL Microsoft Graph API] utilizzando [!UICONTROL HTTP] modulo

   Per istruzioni, consulta [Chiama il [!DNL MS Graph REST API] tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Connessione a un [!DNL Google] app o servizio Web

Il processo di connessione a [!DNL Google] le app possono variare a seconda del tipo di [!DNL Google] account in uso. Inoltre, [!DNL Google] le misure di sicurezza possono richiedere una configurazione aggiuntiva quando ci si connette a [!DNL Workfront Fusion].

Per ulteriori informazioni, consulta:

* [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con misure di sicurezza aggiornate](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Altre app che richiedono una configurazione aggiuntiva

Le seguenti app non seguono la configurazione di base per [!DNL Workfront Fusion] connessioni. Puoi trovare le istruzioni per la connessione di queste app nell&#39;articolo per quell&#39;app.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App / Servizio Web</th> 
   <th>Informazioni aggiuntive sulle connessioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Connetti [!DNL Adobe Workfront] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] moduli</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] moduli</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Connetti [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Connetti [!DNL Datadog] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-mail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Collega l’e-mail a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">Moduli di [!UICONTROL Email]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Connetti [!DNL Gmail] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Intacct]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md#connecti" class="MCXref xref">Connetti [!DNL Intacct] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md" class="MCXref xref">[!DNL Intacct] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Connetti [!DNL Jira Cloud] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Connetti [!DNL Jira Server] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Connetti [!DNL MariaDB] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Collegamento [!DNL Qualtrics] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Connetti [!DNL ServiceNow] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Connetti SFTP a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">Moduli [!UICONTROL SFTP]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Connetti [!DNL Split.io] a [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] moduli</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estendi</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] moduli</a></td> 
  </tr> 
 </tbody> 
</table>

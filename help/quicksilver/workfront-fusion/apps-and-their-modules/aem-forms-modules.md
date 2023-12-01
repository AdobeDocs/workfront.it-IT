---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Experience Manager Forms
description: Con il [!DNL Adobe Experience Manager Forms] connettore per [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] creare, caricare e aggiornare le risorse, nonché copiare o spostare cartelle e risorse.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c4e068729d8de4bef4b2018868e3fa020ca61a06
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] moduli

Con il [!DNL Adobe Experience Manager Forms] connettore per [!DNL Adobe Workfront Fusion], puoi avviare uno scenario basato sugli eventi nel tuo [!DNL Adobe Experience Manager Forms] creando un webhook.

È possibile configurare un modulo in [!DNL Adobe Experience Manager Forms] per inviare gli invii di moduli a questo webhook.

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

## Prerequisiti

* Devi avere un [!DNL Adobe Experience Manager Forms] per utilizzare questo modulo.

## Creare una connessione ad Adobe Experience Manager Forms

Per creare una connessione per [!DNL Adobe Experience Manager Forms] moduli:

1. Clic **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nome connessione]</td>
        <td>
          <p>Immettere un nome per la connessione.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Seleziona se questa connessione si connette a un ambiente di produzione o non di produzione.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>
          <p>Specificare se l'account è un account di servizio o un account personale.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL istanza senza una barra finale]</td>
        <td>
          <p>Immetti l’URL da utilizzare per accedere all’account, senza la barra finale.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL IMS endpoint]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti il [!DNL Adobe] ID client. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il [!DNL Adobe] Segreto client. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID organizzazione]</td>
        <td>Immetti il [!DNL Adobe] ID organizzazione. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Immetti il [!DNL Adobe] ID account tecnico. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Ambiti]</td>
        <td>Inserisci i meta-ambiti appropriati       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Immetti la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
          <p>Per estrarre la chiave privata o il certificato:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selezionare il tipo di file da estrarre.</p>
            </li>
            <li value="3">
              <p>Seleziona il file che contiene la chiave privata o il certificato.</p>
            </li>
            <li value="4">
              <p>Immettere la password per il file.</p>
            </li>
            <li value="5">
              <p>Clic <b>[!UICONTROL Salva]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## Modulo Adobe Experience Manager Forms e relativi campi

Attualmente, nel connettore Adobe Experience Manager Forms è presente un solo modulo.

### Osserva eventi modulo

Questo trigger immediato (webhook) consente di avviare uno scenario quando si verifica un&#39;azione Invia in un Adobe Experience Manager Form.

>[!IMPORTANT]
>
>Questo modulo richiede anche la configurazione in Adobe Experience Manager. Dopo aver configurato il webhook, è necessario aprire Adobe Experience Manager e configurare il modulo per inviare gli invii al webhook.
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook]</td> 
   <td> <p>Immetti un nome per il webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Creare una connessione a [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

Il modulo crea un webhook e ne fornisce l’indirizzo, che puoi immettere nella finestra di dialogo per l’invio del modulo in [!DNL Adobe Experience Manager Forms].












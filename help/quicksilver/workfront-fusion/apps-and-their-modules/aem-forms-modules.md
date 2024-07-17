---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Experience Manager Forms
description: Con il connettore  [!DNL Adobe Experience Manager Forms]  per l'account  [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] , crea, carica e aggiorna le risorse e copia o sposta cartelle e risorse.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 107d81f7-ca41-4d76-a6dd-e579886dc2ad
source-git-commit: 6c7d22bea669586c56acfc23d328d7cc815b04be
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] moduli

Con il connettore [!DNL Adobe Experience Manager Forms] per [!DNL Adobe Workfront Fusion], puoi avviare uno scenario basato sugli eventi nel tuo account [!DNL Adobe Experience Manager Forms] creando un webhook.

È possibile configurare un modulo all&#39;interno di [!DNL Adobe Experience Manager Forms] per inviare invii di moduli a questo webhook.

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

## Prerequisiti

* Per utilizzare questo modulo è necessario disporre di un account [!DNL Adobe Experience Manager Forms].

## Creare una connessione ad Adobe Experience Manager Forms

Per creare una connessione per i moduli [!DNL Adobe Experience Manager Forms]:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

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
        <td>Immetti l'ID client [!DNL Adobe]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il segreto client [!DNL Adobe]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID organizzazione]</td>
        <td>Immetti l'ID organizzazione [!DNL Adobe]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Immetti l'ID account tecnico [!DNL Adobe]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Ambiti]</td>
        <td>Inserisci i meta-ambiti appropriati       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Immettere la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
          <p>Per estrarre la chiave privata o il certificato:</p>
          <ol>
            <li value="1">
              <p>Fare clic su <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Fare clic su <b>[!UICONTROL Salva]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Adobe Experience Manager] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Creare una connessione a [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

Il modulo crea un webhook e fornisce l&#39;indirizzo del webhook, che è possibile immettere nella finestra di dialogo di invio del modulo in [!DNL Adobe Experience Manager Forms].

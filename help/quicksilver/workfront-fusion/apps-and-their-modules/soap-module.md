---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Modulo SOAP
description: È possibile utilizzare il modulo SOAP per connettersi alle API SOAP in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: b820fb8d597205da9f2d0e5e6f5aec1056ec9a45
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# [!UICONTROL SOAP] modulo

È possibile utilizzare [!UICONTROL SOAP] modulo a cui connettersi [!UICONTROL SOAP] API in [!UICONTROL Adobe Workfront Fusion].

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

## Limitazioni del [!UICONTROL SOAP] modulo

>[!NOTE]
>
>I reindirizzamenti sono disattivati durante il caricamento WDSL. Si tratta di una funzione di sicurezza, ma potrebbe significare che i reindirizzamenti non verificati vengono bloccati durante l’esecuzione del modulo.

Il [!UICONTROL SOAP] Il modulo è attualmente in versione beta e non supporta:

* Ridefinire gli elementi
* Limitazioni per cifre frazionarie
* Limitazioni per le cifre totali
* Limitazioni dello spazio vuoto
* Più parti nei messaggi di input e di output. Sono supportati solo i messaggi in una sola parte
* Elementi schema XML personalizzati definiti con l&#39;aiuto di [[!UICONTROL SOAP] Codifica](https://schemas.xmlsoap.org) schemi ed elementi.

>[!INFO]
>
>**Esempio:**
>  
>I seguenti elementi non verrebbero riconosciuti correttamente da [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```
>
>Questo esempio include `soapenc:Array`, `soapenc:arrayType` e `wsdl:arrayType` riferimenti, non ancora supportati in [!UICONTROL Workfront Fusion].

## Soluzione alternativa

Se il [!UICONTROL SOAP] Il modulo rifiuta di elaborare il file WSDL o genera vari errori nella configurazione del modulo. **[!UICONTROL HTTP] > [!UICONTROL Fai una richiesta]** invece del modulo:

1. In entrata [!DNL Workfront Fusion], crea un nuovo scenario.
1. Inserisci il **[!UICONTROL HTTP] > [!UICONTROL Fai una richiesta]** nello scenario.
1. Apri la configurazione del modulo e compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Tipo di corpo]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di contenuto]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Analizza risposta]</td> 
      <td>[!UICONTROL abilitato]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Aprire una nuova finestra o scheda del browser Web.
1. Incollare l&#39;URL WSDL nella barra degli indirizzi del browser Web e recuperare il file XML.

   L’URL WSDL in genere termina con `?wsdl`, ma non necessariamente, ad esempio `http://voip.ms/api/v1/server.wsdl`.

1. Se il file WSDL non viene visualizzato direttamente nel browser Web, aprire il file scaricato in un editor di testo.
1. Cerca `<service>` o `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Una volta individuato, copia l’URL da `location` attributo.
1. In entrata [!DNL Workfront Fusion], incolla l’URL nel campo URL del modulo HTTP.
1. Apri [Online [!UICONTROL SOAP] Client](https://wsdlbrowser.com/) in una nuova finestra/scheda del browser web.
1. Incollare l&#39;URL WSDL nel campo URL WSDL.
1. Clic **[!UICONTROL Sfoglia]**.
1. Scegli dall’elenco delle funzioni a sinistra, ad esempio `getLanguages`.
1. Copia il contenuto del [!UICONTROL Richiedi XML] area di testo.
1. In entrata [!UICONTROL Workfront Fusion], incolla il contenuto copiato nel campo URL del modulo.
1. Fornire i valori per i parametri selezionati sostituendo i punti interrogativi con i valori effettivi:

   ![](assets/request-xml-350x172.png)

1. Chiudi la configurazione del modulo facendo clic su **[!UICONTROL OK]**.
1. Esegui lo scenario o il modulo.

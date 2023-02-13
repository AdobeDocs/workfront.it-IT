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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '418'
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

## Utilizzo della [!UICONTROL SOAP] modulo

La [!UICONTROL SOAP] Il modulo è attualmente in versione beta e non supporta:

* Ridefinire gli elementi
* Restrizioni relative alle cifre della frazione
* Restrizioni a cifre totali
* Restrizioni dello spazio bianco
* Più parti nei messaggi di input e output. Sono supportati solo i messaggi con una sola parte
* Elementi di schema XML personalizzati definiti con l&#39;aiuto di [[!UICONTROL SOAP] Codifica](http://schemas.xmlsoap.org) schemi ed elementi.

>[!INFO]
>
>**Esempio:**
>  
>I seguenti elementi non vengono riconosciuti correttamente da [!UICONTROL Workfront Fusion]:
>
>
```
><complexType name="ArrayOfFloat">
>
>   
  <complexContent>
>
>      
     <restriction base="soapenc:Array">
>
>         
        <attribute ref="soapenc:arrayType"
>
>            
           wsdl:arrayType="xsd:integer[]"/>
>
>      
     </restriction>
>
>   
  </complexContent>
>
>
</complexType>
>```

Include `soapenc:Array`, `soapenc:arrayType` e `wsdl:arrayType` riferimenti, non ancora supportati in [!UICONTROL Workfront Fusion].

## Soluzione alternativa

Se la [!UICONTROL SOAP] Il modulo rifiuta di elaborare il file WSDL o genera vari errori nella configurazione del modulo. È possibile provare a utilizzare il **[!UICONTROL HTTP] > [!UICONTROL Fai una richiesta]** invece:

1. In [!DNL Workfront Fusion], crea un nuovo scenario.
1. Inserisci **[!UICONTROL HTTP] > [!UICONTROL Fai una richiesta]** nello scenario.
1. Apri la configurazione del modulo e compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL, Metodo]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di contenuto]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL abilitato]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Apri una nuova finestra o scheda del browser Web.
1. Incolla l’URL WSDL nella barra degli indirizzi del browser Web e recupera il file XML.

   L’URL WSDL di solito termina con `?wsdl`, ma non necessariamente, per esempio `http://voip.ms/api/v1/server.wsdl`.

1. Se il file WSDL non viene visualizzato direttamente nel browser Web, aprire il file scaricato in un editor di testo.
1. Cerca il `<service>` o `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Una volta individuato, copia l’URL dal `location` attributo.
1. In [!DNL Workfront Fusion], incolla l’URL nel campo URL del modulo HTTP.
1. Apri [Online [!UICONTROL SOAP] Client](https://wsdlbrowser.com/) in una nuova finestra/scheda del browser Web.
1. Incolla l’URL WSDL nel campo URL WSDL.
1. Fai clic su **[!UICONTROL Sfoglia]**.
1. Scegli dall&#39;elenco delle funzioni a sinistra, ad esempio `getLanguages`.
1. Copia il contenuto del [!UICONTROL Richiedi XML] area di testo.
1. In [!UICONTROL Workfront Fusion], incolla il contenuto copiato nel campo URL del modulo.
1. Fornisci valori per i parametri selezionati sostituendo i punti interrogativi con i valori effettivi:

   ![](assets/request-xml-350x172.png)

1. Chiudi la configurazione del modulo facendo clic su **[!UICONTROL OK]**.
1. Esegui lo scenario o il modulo.

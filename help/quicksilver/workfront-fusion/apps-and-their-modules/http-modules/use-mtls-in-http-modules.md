---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: http-modules
title: Utilizzare Mutual TLS nei moduli HTTP in Adobe Workfront Fusion
description: Puoi utilizzare Mutual TLS nei moduli HTTP di Adobe Workfront Fusion, consentendo a entrambi i lati della transazione delle informazioni di verificare l’identità dell’altro.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 595d6e3e0a7d87240644bf20efd425917f4d953d
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Utilizzare Mutual TLS nei moduli HTTP in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza Adobe Workfront.

## Panoramica reciproca su TLS

Quando invii dati tramite Internet, è importante assicurarsi che questi vengano o vengano dalla posizione corretta e che solo il destinatario previsto possa leggerli. Con TLS abilitato, il client (computer che richiede informazioni) utilizza certificati per verificare l’identità del server (computer che fornisce informazioni). Ciò rende sicure le connessioni HTTP.

Mutual TLS consente a questa conferma dell&#39;identità di andare in entrambi i modi. Quando il server invia il certificato per verificare la propria identità al client, richiede anche il certificato del client. In questo modo, il server non invia informazioni a un sito o a un utente che le utilizzerebbe in modo improprio.

>[!INFO]
>
>**Esempio:**
>
>* **TLS**: Quando una persona digita &quot;MyGreatBank.com&quot; in un browser, vuole essere sicuro che stanno andando alla My Great Bank, non un sito web che potrebbe abusare o vendere le loro informazioni bancarie. Vogliono anche essere sicuri che le informazioni sul loro conto bancario siano crittografate.
   >
   >   Quando il browser (il client) si connette a MyGreatBank.com (il server), TLS richiede un certificato da MyGreatBank.com per verificare la sua identità. Il certificato è fornito da un’autorità di certificazione come [!DNL DigiCert] o [!DNL Thawte]. Poiché il browser considera attendibile l’autorità di certificazione, consente la connessione.
>
>* **TLS reciproco**: MySoftware.com è un client software che necessita di informazioni dall&#39;API MyGreatBank.com. MyGreatBank consente solo ai client affidabili di connettersi ai propri server. Quindi, oltre al regolare TLS che verifica l&#39;identità di MyGreatBank.com, il processo di autorizzazione TLS/certificate verifica anche la richiesta di MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Fornisci il tuo [!DNL Workfront Fusion] certificato pubblico


Quando ci si connette a un servizio Web con una richiesta HTTP, in genere il servizio Web richiede un [!DNL Workfront Fusion] certificato pubblico per la verifica. Questo consente al servizio Web di confrontare il certificato presentato nella richiesta HTTP con quello presente nel file, in modo da garantire che il certificato sia sull’inserire nell&#39;elenco Consentiti del servizio Web.

Per istruzioni su come caricare i [!DNL Adobe Workfront Fusion] certificato pubblico per un servizio Web, consulta la documentazione del servizio Web.

>[!NOTE]
>
>Potrebbe essere necessario fornire altre informazioni oltre al certificato. Per informazioni sulle esigenze di un servizio Web, consulta la documentazione API del servizio Web.

È possibile utilizzare i seguenti collegamenti per scaricare i certificati pubblici di Workfront Fusion:

### Certificati per il 14 novembre 2022 - 15 luglio 2023

>[!IMPORTANT]
>
>Tali [!DNL Workfront Fusion] i certificati pubblici scadono il 15 luglio 2023. Dopo la scadenza, dovrai caricare un nuovo certificato sul servizio Web. Ti consigliamo di:
>
>* Prendi nota della data di scadenza e imposta un promemoria per te stesso sul caricamento del certificato nel tuo servizio Web.
>* Aggiungi ai segnalibri questa pagina per trovare facilmente i nuovi certificati.
>


* [Scarica [!DNL Workfront Fusion] Certificato 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Scarica [!DNL Workfront Fusion] Certificato UE 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   Da utilizzare nell&#39;UE

<!--

Previous US cert

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app_workfrontfusion_com-jul-15-2023.cer)

### Certificates for November 17, 2021 - November 14, 2022

>[!IMPORTANT]
>
>These certificates expire on November 14, 2022. Upload the new certificates to the web service as soon as possible.

* [Download Workfront Fusion Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
* [Download Workfront Fusion EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt)

  For use in the EU

  -->

## Abilitazione di TLS reciproco in [!DNL Workfront Fusion] Moduli HTTP

Tutto [!DNL Workfront Fusion] [!UICONTROL HTTP] i moduli di richiesta possono abilitare Mutual TLS.

Per abilitare Mutual TLS in un [!UICONTROL HTTP] modulo di richiesta:

1. Aggiungi un [!UICONTROL HTTP] richiedere il modulo allo scenario.
1. Inizia a configurare il modulo.

   Per istruzioni su come configurare un [!UICONTROL HTTP] modulo di richiesta, vedi l&#39;articolo appropriato in [[!UICONTROL HTTP] moduli](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Abilita **[!UICONTROL Mostra impostazioni avanzate]** vicino alla parte inferiore del modulo.
1. Abilita **[!UICONTROL Usa TLS reciproco]**.

---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: http-modules
title: Utilizzo di Mutual TLS nei moduli HTTP in Adobe Workfront Fusion
description: Puoi utilizzare Mutual TLS nei moduli HTTP di Adobe Workfront Fusion, consentendo a entrambi i lati della transazione di informazioni di verificare l’identità dell’altro.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 790f5da3af32ffdfcbb596f467f882a7408e3f28
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Utilizzare Mutual TLS nei moduli HTTP in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza di Adobe Workfront.

## Panoramica di Mutual TLS

Quando invii dati tramite Internet, è importante assicurarsi che arrivino o provengano dalla posizione corretta e che solo il destinatario previsto possa leggerli. Con TLS abilitato, il client (computer che richiede informazioni) utilizza i certificati per verificare l&#39;identità del server (computer che fornisce informazioni). Questo rende sicure le connessioni HTTP.

Il TLS reciproco consente di confermare l’identità in entrambi i modi. Quando il server invia il proprio certificato per verificarne l’identità al client, richiede anche il certificato del client. In questo modo il server non invia informazioni a un sito o a un utente che potrebbero utilizzarle in modo improprio.

>[!INFO]
>
>**Esempio:**
>
>* **TLS**: quando una persona digita &quot;MyGreatBank.com&quot; in un browser, vuole essere sicura di andare su My Great Bank, non su un sito web che potrebbe abusare o vendere le proprie informazioni bancarie. Vogliono anche essere sicuri che le informazioni del loro conto bancario siano crittografate.
   >
   >   Quando il browser (il client) si connette a MyGreatBank.com (il server), TLS richiede un certificato da MyGreatBank.com per verificarne l’identità. Il certificato viene fornito da un’autorità di certificazione come [!DNL DigiCert] o [!DNL Thawte]. Poiché il browser considera attendibile l&#39;autorità di certificazione, consente la connessione.
>
>* **TLS reciproco**: MySoftware.com è un client software che richiede informazioni dall’API MyGreatBank.com. MyGreatBank consente solo ai client attendibili di connettersi ai propri server. Quindi, oltre alla verifica TLS regolare dell’identità di MyGreatBank.com, il processo TLS/autorità di certificazione verifica anche la richiesta da MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion per l'automazione e l'integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Fornire [!DNL Workfront Fusion] certificato pubblico


Quando ti connetti a un servizio web con una richiesta HTTP, in genere il servizio web richiede un [!DNL Workfront Fusion] certificato pubblico di verifica. Questo consente al servizio web di confrontare il certificato presentato nella richiesta HTTP con quello presente nel file, in modo da garantire che il certificato si trovi nel inserisco nell&#39;elenco Consentiti di del servizio web.

Per istruzioni sul caricamento di [!DNL Adobe Workfront Fusion] certificato pubblico a un servizio web, consulta la documentazione del servizio web.

>[!NOTE]
>
>In aggiunta al certificato, potrebbe essere necessario fornire altre informazioni. Per informazioni sulle esigenze di un servizio web, consulta la documentazione API del servizio web.

È possibile utilizzare i seguenti collegamenti per scaricare i certificati pubblici di Workfront Fusion:

### Certificati per il 25 maggio 2023 - 9 giugno 2024

>[!IMPORTANT]
>
>* Questi [!DNL Workfront Fusion] i certificati pubblici scadono il 9 giugno 2024. Dopo la scadenza, dovrai caricare un nuovo certificato nel servizio web. Si consiglia di:
   >
   >   * Prendi nota della data di scadenza e imposta un promemoria per te stesso per caricare il certificato nel servizio web.
   >   * Aggiungi ai segnalibri questa pagina per trovare facilmente i nuovi certificati.
>
>* Si tratta di certificati mTLS non jolly.


* [Scarica [!DNL Workfront Fusion] Certificato 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)
* [Scarica [!DNL Workfront Fusion] Certificato UE 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   Per l&#39;uso nell&#39;UE

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## Abilitazione della connessione TLS reciproca in [!DNL Workfront Fusion] Moduli HTTP

Tutti [!DNL Workfront Fusion] [!UICONTROL HTTP] I moduli di richiesta hanno l’opzione per abilitare Mutual TLS.

Per abilitare Mutual TLS in un [!UICONTROL HTTP] modulo di richiesta:

1. Aggiungi un [!UICONTROL HTTP] richiedere il modulo allo scenario.
1. Inizia la configurazione del modulo.

   Per istruzioni sulla configurazione di un [!UICONTROL HTTP] modulo di richiesta, consulta l’articolo appropriato in [[!UICONTROL HTTP] moduli](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Abilita **[!UICONTROL Mostra impostazioni avanzate]** nella parte inferiore del modulo.
1. Abilita **[!UICONTROL Usa TLS reciproco]**.

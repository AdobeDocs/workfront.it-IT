---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: HTTP &gt; Altri moduli
description: La [!DNL Adobe Workfront Fusion] L’app HTTP fornisce vari moduli di comunicazione basati sul protocollo HTTP (Hypertext Transfer Protocol). HTTP è la base della comunicazione di dati per il World Wide Web. Puoi utilizzare i moduli per scaricare pagine web e file, chiamare webhook e endpoint API e così via.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > Altri moduli

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] richiede un [!UICONTROL Adobe Workfront Fusion] oltre a una licenza [!UICONTROL Adobe Workfront] licenza.

La [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] app fornisce vari moduli per la comunicazione basata sul protocollo HTTP (Hypertext Transfer Protocol). HTTP è la base della comunicazione di dati per il World Wide Web. Puoi utilizzare i moduli per scaricare pagine web e file, chiamare webhook e endpoint API e così via.

La scelta corretta del modulo dipende dal meccanismo di autenticazione/autorizzazione della risorsa a cui desideri accedere dipende dai dipendenti. Di seguito sono riportati alcuni esempi di moduli

* Esegui una richiesta:modulo universale destinato principalmente alle risorse che non utilizzano alcun tipo di autenticazione/autorizzazione
* Esegui una richiesta di autenticazione di base:per le risorse che utilizzano [!DNL HTTP] Autenticazione di base (BA)
* Effettua una richiesta OAuth 2.0: per le risorse che utilizzano il protocollo di autorizzazione OAuth 2.0
* Effettua una richiesta di autenticazione certificato client: per le risorse che utilizzano il protocollo di autorizzazione che richiede un certificato lato client.
* Effettua una richiesta di autorizzazione della chiave API: per le risorse che utilizzano le chiavi API per l&#39;autorizzazione.

## Moduli di richiesta

Per istruzioni specifiche sul modulo di richiesta, consulta i seguenti articoli:

* [[!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] modulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta di autorizzazione di base] modulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta di autorizzazione certificato client] modulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta di autorizzazione della chiave API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Altri moduli d&#39;azione

* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Risolvere un URL di destinazione]](#resolve-a-target-url)

### [!UICONTROL Ottieni un file]

Questo modulo di azione scarica un file dall’URL specificato. Una volta scaricato il file, è possibile elaborare ulteriormente il file (mappare i dati del file) utilizzando altri moduli nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Immetti o mappa l’URL del file da scaricare. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Risolvere un URL di destinazione]

Questo modulo di azione risolve una catena di reindirizzamenti HTTP e restituisce un URL di destinazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Immetti o mappa l’URL da risolvere, ad esempio un [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo] </td> 
   <td> <p>Seleziona se desideri utilizzare il metodo [!UICONTROL HEAD] o il metodo [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Moduli iteratori

### [!UICONTROL Recupera intestazioni]

Questo modulo restituisce ogni intestazione (nome e valore) dal modulo HTTP specificato in un bundle separato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Selezionare il modulo da cui si desidera recuperare le intestazioni.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generazione di token web JSON (JWT)

È possibile generare un token JWT con l’aiuto di funzioni integrate:

Intestazione:

![](assets/jwt-header-350x19.png)

Codice per copia&amp;incolla:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Payload:

![](assets/jwt-payload-350x17.png)

Codice per copia&amp;incolla:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Codice per copia&amp;incolla:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

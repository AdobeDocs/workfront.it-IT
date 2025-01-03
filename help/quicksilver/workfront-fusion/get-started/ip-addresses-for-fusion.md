---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Indirizzi IP per l'accesso ad Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 800cf889ff2729fca0c9d75d0ace0ecc1ee53a79
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Indirizzi IP per accedere a [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede una licenza [!DNL Adobe Workfront Fusion] oltre a [!DNL Adobe Workfront license].

Se il firewall o il server di posta è configurato per consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti per consentire la comunicazione aperta tra l&#39;ambiente e [!DNL Adobe Workfront Fusion].

È possibile aggiungere tutti gli indirizzi IP e i domini di Fusion al inserisco nell&#39;elenco Consentiti di oppure individuare il cluster di Fusion e aggiungere solo gli indirizzi IP e i domini per tale cluster.

## Aggiungere tutti gli indirizzi IP e i domini di Fusion

Aggiungi i seguenti indirizzi IP al tuo inserisco nell&#39;elenco Consentiti di:

* 52.30.133.50
* 54 220 93 204
* 34 254 76 122
* 54 244 142 219
* 52.39.217.230
* 44 241 82 96
* 100.20.126.137
* 34 223 32,4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

Inoltre, se l’organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al inserisco nell&#39;elenco Consentiti per consentire al sistema di accedere a Workfront Fusion. Questi vengono utilizzati per i webhook.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Aggiungere indirizzi IP e domini Fusion solo per il cluster

### Identificare il datacenter

Gli indirizzi IP variano in base alla posizione in cui vengono memorizzati i dati.

Se accedi a Fusion tramite un URL, puoi esaminarlo per individuare il tuo datacenter.

| URL | Datacenter |
| --- | --- |
| `https://app.workfrontfusion.com/` | Datacenter USA |
| `https://app-eu.workfrontfusion.com/` | Datacenter UE |
| `https://app-az.workfrontfusion.com/` | Datacenter di Azure |

Se accedi a Fusion tramite experience.adobe.com, puoi controllare la scheda di rete nel browser per identificare il datacenter.

| URL | Datacenter |
| --- | --- |
| Chiamate a `https://fusion.adobe.com` | Datacenter USA |
| Chiamate a `https://eu.fusion.adobe.com` | Datacenter UE |
| Chiamate a `https://az.fusion.adobe.com` | Datacenter di Azure |

### Aggiungere indirizzi IP e domini per il centro dati

Aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di accesso al sistema per consentire a [!DNL Workfront Fusion] di accedere al sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Datacenter UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Datacenter USA</p> </td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li>
     <li>100.20.126.137</li>
     <li>34 223 32,4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] nel cluster di Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Inoltre, se l’organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al inserisco nell&#39;elenco Consentiti per consentire al sistema di accedere a Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Datacenter UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Datacenter USA</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] nel cluster di Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Il filtro di rete in uscita non è comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare il inserisco nell&#39;elenco Consentiti di gestione della rete per adattarlo a tale scopo.

Per ulteriori informazioni sull&#39;impostazione del inserisco nell&#39;elenco Consentiti di configurazione del dell&#39;organizzazione, vedere [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

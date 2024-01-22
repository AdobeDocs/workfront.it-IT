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
source-git-commit: adb324323330f53108532cc7a7e68466fdb84273
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] licenza oltre a un [!DNL Adobe Workfront license].

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di per consentire la comunicazione aperta tra l&#39;ambiente e [!DNL Adobe Workfront Fusion].

Aggiungi i seguenti indirizzi IP al tuo inserisco nell&#39;elenco Consentiti di abilitazione per l’accesso a tutti i servizi di gestione dell’accesso ai dati () [!DNL Workfront Fusion] per accedere al sistema.

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

Inoltre, se l’organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al tuo elenco Consentiti di accesso a Workfront Fusion per consentire l’accesso al sistema.

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
>Il filtro di rete in uscita non è comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare il inserisco nell&#39;elenco Consentiti di accesso a un&#39;istanza di accesso a un&#39;istanza di rete.

Per ulteriori informazioni sulla configurazione del inserisco nell&#39;elenco Consentiti di dell’organizzazione, consulta [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

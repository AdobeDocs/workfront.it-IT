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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# Indirizzi IP per l&#39;accesso [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza [!DNL Adobe Workfront license].

Se il firewall o il server di posta elettronica è configurato per consentire l’accesso solo a determinati fornitori, è necessario aggiungere alcuni indirizzi IP al relativo inserire nell&#39;elenco Consentiti al fine di consentire la comunicazione aperta tra l’ambiente e [!DNL Adobe Workfront Fusion].

Aggiungi i seguenti indirizzi IP al tuo inserire nell&#39;elenco Consentiti per abilitare [!DNL Workfront Fusion] per accedere al sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro dati UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Datacenter USA</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Inoltre, se l&#39;organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al tuo inserire nell&#39;elenco Consentiti per consentire al sistema di accedere a Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro dati UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Datacenter USA</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Filtro di rete in uscita non comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare l&#39;inserire nell&#39;elenco Consentiti per adattarlo.

Per ulteriori informazioni sull&#39;impostazione dell&#39;inserire nell&#39;elenco Consentiti dell&#39;organizzazione, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

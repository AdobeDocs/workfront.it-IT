---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare l’inserire nell'elenco Consentiti del firewall
description: Se il firewall o il server di posta elettronica è configurato per consentire l’accesso solo a determinati fornitori, è necessario aggiungere alcuni indirizzi IP al relativo inserire nell'elenco Consentiti. Questo apre la comunicazione tra l'ambiente e i server Adobe Workfront e consente agli utenti di inviare messaggi da Workfront e di utilizzare SSO con Active Directory o LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 13%

---

# Configurare l’inserire nell&#39;elenco Consentiti del firewall

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per configurare il tuo inserire nell&#39;elenco Consentiti se l&#39;organizzazione è stata caricata in Adobe Admin Console, vedi [Domini consentiti per Adobi app e servizi](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Se il firewall o il server di posta elettronica è configurato per consentire l’accesso solo a determinati fornitori, è necessario aggiungere alcuni indirizzi IP al relativo inserire nell&#39;elenco Consentiti. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront e consente i seguenti processi:

* Invio di messaggi dall’applicazione Workfront

   >[!NOTE]
   >
   >Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

* Utilizzo dei webhook di documenti durante la configurazione di integrazioni di documenti personalizzate
* Utilizzo degli abbonamenti agli eventi di Workfront

   Per ulteriori informazioni, consulta [API iscrizione agli eventi](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

È inoltre necessario aprire alcune porte affinché i messaggi e-mail vengano crittografati al momento della consegna.

## Workfront inseriti nell&#39;elenco Consentiti utilizzabili

Se la tua organizzazione dispone del piano Enterprise, puoi anche configurare due inserire nell&#39;elenco Consentiti Workfront:

* **inserire nell&#39;elenco Consentiti e-mail**: Consente di controllare dove gli utenti possono inviare i dati e-mail archiviati in Workfront. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti e-mail](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **inserire nell&#39;elenco Consentiti IP**: Limita l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati, fornendo un ulteriore livello di sicurezza per l’applicazione Workfront. Per ulteriori informazioni, consulta [Limitare l’accesso ad Adobe Workfront per indirizzo IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Indirizzi IP da aggiungere all’inserire nell&#39;elenco Consentiti

Gli indirizzi IP che devi aggiungere al tuo inserire nell&#39;elenco Consentiti sul firewall dipendono dal cluster in cui viene eseguito l’ambiente di produzione. Per scoprire quale cluster si trova, vedi Configurazione > Sistema > Informazioni personalizzate. Per ulteriori informazioni, consulta la sezione . [Configurare le informazioni di base](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) nell&#39;articolo [Configurare le informazioni di base per il sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>Alcune integrazioni Workfront non funzionano quando l&#39;inserire nell&#39;elenco Consentiti è abilitato perché non possono essere configurate con un indirizzo IP statico. Per utilizzare le seguenti integrazioni, devi disattivare l&#39;inserire nell&#39;elenco Consentiti.
>
>* Workfront per G Suite
>* Workfront per Outlook
>* Workfront per Salesforce


* [Indirizzi IP consentiti per i cluster 1, 2, 3, 5, 7, 8 e 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Indirizzi IP per consentire il cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Indirizzi IP per consentire il cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Indirizzi IP per consentire un&#39;unità di prova](#IP%20Addre2)
* [Indirizzi IP da consentire durante l’implementazione degli abbonamenti agli eventi](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Indirizzi IP per consentire un’autenticazione avanzata](#ip-addresses-to-allow-for-enhanced-authentication)
* [Indirizzi IP da aggiungere per accedere a Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Indirizzi IP da aggiungere per l’utilizzo di Workfront per Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Indirizzi IP da aggiungere per l’utilizzo di Workfront Ascent](#ip-addresses-to-add-for-using-workfront-ascent)
* [URL da aggiungere per tutti i cluster Workfront](#urls-to-add-for-all-clusters-workfront)

### Indirizzi IP consentiti per i cluster 1, 2, 3, 5, 7, 8 e 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Se l&#39;ambiente di produzione si trova nel cluster 1, 2, 3, 5 o 7, è necessario consentire i seguenti indirizzi IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per SSO, documentazione Web hook o altre funzionalità</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall’applicazione Workfront</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>Per informazioni sui seguenti indirizzi IP, vedi <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">Nuovi indirizzi IP per le e-mail di Adobe Workfront con la versione 21.1</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire il cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Se l&#39;ambiente di produzione è nel cluster 4, aggiungi i seguenti indirizzi IP per SSO, documenta le integrazioni webhook e per ricevere e-mail dall&#39;applicazione Workfront:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122

Per informazioni sui seguenti indirizzi IP, vedi [Nuovi indirizzi IP per le e-mail di Adobe Workfront con la versione 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### Indirizzi IP per consentire il cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Se l&#39;ambiente di produzione si trova nel cluster 6, aggiungi i seguenti indirizzi IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall’applicazione Workfront</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per utilizzare il servizio e-mail AWS</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire un&#39;unità di prova

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall’applicazione Workfront quando si utilizza un’unità di test</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per l'SSO e documentare le integrazioni webhook quando si utilizza un'unità di prova</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Questo indirizzo deve anche essere aggiunto al tuo inserire nell'elenco Consentiti affinché i tuoi utenti ricevano e-mail da Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP da consentire durante l’implementazione degli abbonamenti agli eventi  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Per tutti gli ambienti, aggiungi i seguenti indirizzi IP per ricevere payload dagli abbonamenti agli eventi di Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Per i clienti in Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per i clienti in località diverse dall'Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire un’autenticazione avanzata {#ip-addresses-to-allow-for-enhanced-authentication}

Aggiungi i seguenti indirizzi IP per utilizzare l’autenticazione avanzata per Anteprima o Produzione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se l'ambiente è nel cluster 1, 2, 3, 5, 7, 8 o 9</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se l'ambiente è nel cluster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP da aggiungere per accedere a Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Aggiungi i seguenti indirizzi IP al tuo inserire nell&#39;elenco Consentiti per consentire ad Workfront Fusion di accedere al tuo sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro dati Adobe Workfront EU</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centro dati Adobe Workfront US</p> </td> 
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
   <td role="rowheader">Centro dati Adobe Workfront EU</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centro dati Adobe Workfront US</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Filtro di rete in uscita non comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare l&#39;inserire nell&#39;elenco Consentiti per adattarlo.

### Indirizzi IP da aggiungere per l’utilizzo di Workfront per Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Aggiungi i seguenti indirizzi IP al tuo inserire nell&#39;elenco Consentiti per utilizzare Workfront per l’integrazione Jira.

Anche il dominio jira.workfront.com deve essere accessibile dai server aziendali. Questo dominio è necessario perché funge da middleware tra Workfront e Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Per i clienti in Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per i clienti in località diverse dall'Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP da aggiungere per l’utilizzo di Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per accedere alle risorse di formazione Workfront tramite Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per ricevere notifiche e-mail da Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domini da aggiungere per l’accesso a Workfront

Se la tua organizzazione utilizza il filtro di rete in uscita, aggiungi i seguenti domini al tuo inserire nell&#39;elenco Consentiti per consentire al sistema di accedere a Workfront.

>[!NOTE]
>
>Filtro di rete in uscita non comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare l&#39;inserire nell&#39;elenco Consentiti per adattarlo.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## URL da aggiungere per tutti i cluster Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per consentire la visualizzazione dei contenuti dell’Aiuto nell’ambiente Workfront</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per consentire a Workfront Proof di accedere a Workfront su qualsiasi cluster, aggiungili a tutti gli ambienti</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Richiesto per visualizzare le bozze in Workfront</li> 
     <li>*.proofhq.com - Richiesto per visualizzare le bozze in Workfront Proof</li> 
     <li>*.proofhq.eu - Richiesto per visualizzare le bozze in Workfront Proof</li> 
    </ul> <p><b>NOTA</b>:  <p>Non è supportata l’aggiunta di indirizzi IP al tuo inserire nell'elenco Consentiti per Workfront Proof. Sono state dinamiche dopo il passaggio di Workfront ad AWS. È invece consigliabile consentire solo i domini di prova Workfront.</p> <p>Se si verifica un problema con l’aggiunta di questi domini al tuo inserire nell'elenco Consentiti e hai bisogno invece di un indirizzo IP, contatta l’Assistenza clienti Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Indirizzi IP e URL da aggiungere per l’accesso a Workfront Proof

Per utilizzare varie funzioni, devi aggiungere i seguenti indirizzi IP al tuo inserire nell&#39;elenco Consentiti.

* [Per callback e bozze di acquisizione web](#for-callbacks-and-webcapture-proofs)
* [Per e-mail in uscita](#for-outgoing-email)

### Per callback e bozze di acquisizione web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (cluster 1, 2, 3, 5 e 7)</td> 
   <td> 
    <ul> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>NOTA</b>: Le opzioni del server DNS non sono più supportate.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Per e-mail in uscita {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (cluster 1, 2, 3, 5 e 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Porte da aprire per le migliori prestazioni di Workfront Proof

Apri le seguenti porte se si verificano problemi con il caricamento o il funzionamento delle bozze in Workfront Proof:

* 5671
* 5672
* 15671

## Porte da aprire per e-mail crittografate

Le e-mail provenienti dall’applicazione Workfront vengono inviate crittografate utilizzando le porte 465 e 587. Se il server di posta elettronica non supporta le e-mail crittografate, queste vengono recapitate non crittografate utilizzando la porta 25.

## Notifiche e-mail dal supporto Workfront

Se non ricevi e-mail dal supporto Workfront, assicurati di aggiungere gli indirizzi IP e i domini di Salesforce di cui hai bisogno. Per ulteriori informazioni, consulta l’articolo della guida Salesforce sugli indirizzi IP e i domini di Salesforce da consentire.

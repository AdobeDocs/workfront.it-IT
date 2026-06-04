---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare il Inserisco nell'elenco Consentiti di configurazione del firewall per l'installazione di un sistema di protezione in linea con il sistema di protezione in uso. Configurare il  di protezione del firewall
description: Se il firewall o il server di posta è configurato in modo da consentire l'accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell'elenco Consentiti di. In questo modo si apre la comunicazione tra l'ambiente e i server Adobe Workfront e si consente agli utenti di inviare messaggi da Workfront e di utilizzare l'SSO con Active Directory o LDAP.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
TQID: https://experienceleague.adobe.com/voAiMROhu9NJkN-WLjPWcpDu-x8YYgtlZNeNWk8dFjA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: ec8965fc-2f75-47f6-a9bb-730e8c2725f3
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1456
ht-degree: 6%

---

# Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo

<!-- Audited: 12/2023 -->

<!--Follow up October 2026-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in Admin Console. Poiché tutte le organizzazioni sono ora state integrate in Adobe Admin Console, è necessario eseguire questa azione tramite Adobe Admin Console.
>
>Per configurare il elenco Consentiti di dopo l&#39;onboarding dell&#39;organizzazione in Adobe Admin Console, vedere [Domini per le app e i servizi Adobe](https://helpx.adobe.com/it/enterprise/kb/network-endpoints.html).
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, vedi [Differenze di amministrazione tra Adobe Workfront e Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Il modo in cui un’organizzazione configura il proprio inserisco nell&#39;elenco Consentiti di è univoco per ogni organizzazione. Collabora con il tuo team IT per identificare la procedura aziendale e implementare queste aggiunte.

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront e consente i seguenti processi:

* Utilizzo dei webhook dei documenti durante la configurazione di integrazioni di documenti personalizzate
* Utilizzo delle sottoscrizioni agli eventi di Workfront

  Per ulteriori informazioni, vedere [API sottoscrizione eventi](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

È inoltre necessario aprire alcune porte per crittografare i messaggi e-mail al momento della consegna.

## Workfront utilizzabili

Se la tua organizzazione dispone del piano Enterprise, puoi anche configurare due Workfront di inserire nell&#39;elenco Consentiti:

* **inserisco nell&#39;elenco Consentiti di invio di posta elettronica per l&#39;**: consente di controllare la posizione in cui gli utenti possono inviare i dati archiviati in Workfront. Per ulteriori informazioni, consulta [Configurare il tuo inserisco nell&#39;elenco Consentiti di e-mail](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **inserisco nell&#39;elenco Consentiti di IP**: limita l&#39;accesso a Workfront a 75 indirizzi IP o intervalli di indirizzi IP specificati, fornendo un ulteriore livello di sicurezza per l&#39;applicazione Workfront. Per ulteriori informazioni, vedere [Limitare l&#39;accesso ad Adobe Workfront per indirizzo IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Individuare il cluster Workfront

Gli indirizzi IP da aggiungere al elenco Consentiti di sul firewall dipendono dal cluster in cui viene eseguito l’ambiente di produzione.

Per individuare il cluster dell&#39;organizzazione:

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Sistema**, quindi seleziona **Informazioni cliente**.
1. Individua il campo **Cluster Setup** nell&#39;angolo superiore destro della pagina. Il cluster della tua organizzazione è elencato qui.

   CL01 fa riferimento al cluster 1, CL02 al cluster 2 e così via.

Per ulteriori informazioni, vedere la sezione [Visualizzare il cluster e il piano Workfront dell&#39;organizzazione](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) nell&#39;articolo [Panoramica del firewall](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Indirizzi IP da aggiungere al inserisco nell&#39;elenco Consentiti di

* [Indirizzi IP per consentire i cluster 1, 2, 3, 5, 7, 8 e 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Indirizzi IP da consentire per il cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Indirizzi IP da consentire per il cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Indirizzi IP per consentire il cluster 10](#ip-addresses-to-allow-for-cluster-10)
* [Indirizzi IP da consentire per un&#39;unità di prova](#IP%20Addre2)
* [Indirizzi IP da consentire durante l&#39;implementazione di sottoscrizioni eventi](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Indirizzi IP da aggiungere per accedere a Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Indirizzi IP da aggiungere per l&#39;utilizzo di Workfront per Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL da aggiungere per tutti i cluster Workfront](#urls-to-add-for-all-clusters-workfront)

### Per ricevere e-mail dall’applicazione Workfront

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di ricezione dei messaggi di posta elettronica dell&#39;applicazione Workfront.

#### Aree geografiche USA: cluster 1, 2, 3, 5, 6, 7, 8, 9 e 10

* 206.55.149.211
* 206.55.149.212
* 206.55.149.213
* 206.55.149.214
* 206.55.149.215
* 23.251.237.106
* 23.251.237.107
* 23.251.237.108
* 23.251.237.109
* 54.240.119.54
* 54.240.119.55
* 54.240.60.174
* 54.240.60.175
* 54.240.61.222
* 54.240.61.223

#### Regioni UE: cluster 4, 11, 12 e 13

* 23.251.239.98
* 23.251.239.99
* 24.110.76.223
* 24.110.76.224
* 69.169.230.231
* 69.169.230.232


### SSO, integrazioni di webhook di documenti e altre funzionalità

#### Aree geografiche USA: cluster 1, 2, 3, 5, 6, 7, 8, 9 e 10

**Cluster 1, 2, 3, 5, 6, 7, 8, 9**


* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4
* 34.211.224.9
* 54.218.48.56
* 52.36.154.34
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 54.203.255.135/32
* 35.155.2.51/32
* 52.34.192.77/32

**Cluster 10**

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

#### Regioni UE: cluster 4 e 11


**Custer 4**

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
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
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32


### Indirizzi IP per consentire un&#39;unità di test

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall'applicazione Workfront quando si utilizza un'unità di test</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per le integrazioni SSO e documenta webhook quando si utilizza un’unità di test</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Per consentire agli utenti di ricevere e-mail da Workfront, questo indirizzo deve essere aggiunto anche al tuo elenco Consentiti di.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP da consentire durante l’implementazione delle sottoscrizioni di eventi  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Per tutti gli ambienti, aggiungi i seguenti indirizzi IP per ricevere i payload dagli abbonamenti agli eventi di Workfront.

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
   <td role="rowheader">Per clienti in paesi diversi dall'Europa</td> 
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

### Indirizzi IP da aggiungere per accedere a Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di accesso di Workfront Fusion al proprio sistema di.

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
   <td role="rowheader"> <p>Centro dati Adobe Workfront USA</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] nel cluster Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Inoltre, se l’organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al tuo elenco Consentiti di accesso a Workfront Fusion per consentire l’accesso al sistema. Questi URL vengono utilizzati per i webhook in Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro dati Adobe Workfront EU</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centro dati Adobe Workfront USA</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] nel cluster Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Il filtro di rete in uscita non è comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare il inserisco nell&#39;elenco Consentiti di accesso a un&#39;istanza di accesso a un&#39;istanza di rete.

### Indirizzi IP da aggiungere per l’utilizzo di Workfront per Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Aggiungi i seguenti indirizzi IP al tuo inserisco nell&#39;elenco Consentiti di per utilizzare l’integrazione di Workfront for Jira.

Il dominio jira.workfront.com deve essere accessibile anche dai server aziendali. Questo dominio è necessario perché funge da middleware tra Workfront e Jira.

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
   <td role="rowheader">Per clienti in paesi diversi dall'Europa</td> 
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

## Domini da aggiungere per accedere a Workfront

Se l’organizzazione utilizza il filtro di rete in uscita, aggiungi i seguenti domini al inserisco nell&#39;elenco Consentiti di accesso a Workfront per abilitare il sistema.

>[!NOTE]
>
>Il filtro di rete in uscita non è comune. Rivolgersi all&#39;amministratore di rete per verificare se è necessario aggiornare il inserisco nell&#39;elenco Consentiti di accesso a un&#39;istanza di accesso a un&#39;istanza di rete.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Si tratta di un dominio statico che include tutti i seguenti domini. Puoi aggiungere i singoli domini se preferisci:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Poiché la tua organizzazione si trova nell’esperienza unificata di Adobe, utilizza i seguenti domini. Questi domini sono coperti in `*.adobe.com`, ma possono essere aggiunti se si desidera.

* &lt;dominio>.my.workfront.adobe.com
* &lt;dominio>.preview.workfront.adobe.com
* &lt;dominio>.sb01.workfront.adobe.com
* &lt;dominio>.sb02.workfront.adobe.com


Per Workfront Fusion, aggiungi i seguenti domini:

<!--Remove me October 2026-->

* Per l’organizzazione non inclusa nell’esperienza unificata di Adobe:
   * app.workfrontfusion.com (US AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* Per l’organizzazione sull’esperienza unificata di Adobe
Questi domini sono coperti in `*.adobe.com`, ma possono essere aggiunti se lo si desidera.

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## URL da aggiungere per tutti i cluster Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per consentire la visualizzazione del contenuto dell'Aiuto nell'ambiente Workfront</td> 
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
     <li>*.workfront.com - Necessario per visualizzare le bozze in Workfront</li> 
     <li>*.proofhq.com - Necessario per visualizzare le bozze in Workfront Proof</li> 
     <li>*.proof.eu - Necessario per visualizzare le bozze in Workfront Proof</li> 
    </ul> <p><b>NOTA</b>:  <p>Non è supportata l’aggiunta di indirizzi IP al tuo elenco Consentiti di per Workfront Proof. Sono diventati dinamici dopo il passaggio di Workfront ad AWS. È invece consigliabile consentire solo i domini Workfront Proof.</p> <p>Se si verifica un problema durante l’aggiunta di questi domini al tuo inserisco nell'elenco Consentiti di e hai bisogno di un indirizzo IP, contatta l’Assistenza clienti Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Indirizzi IP e URL da aggiungere per accedere a Workfront Proof

Per utilizzare varie funzioni, è necessario aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di.

* [Per callback e bozze di webcapture](#for-callbacks-and-webcapture-proofs)
* [Per e-mail in uscita](#for-outgoing-email)

### Per callback e bozze di acquisizione Web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (cluster 1, 2, 3, 5 e 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
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
    <li>34.255.252.190</li>
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
    </ul> <p><b>NOTA</b>: le opzioni del server DNS non sono più supportate.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Per e-mail in uscita {#for-outgoing-email}

Consulta la sezione [Per ricevere e-mail dall&#39;applicazione Workfront](#to-receive-email-from-the-workfront-application) precedente.


## Porte aperte per prestazioni Workfront Proof ottimali

Se riscontri problemi con il caricamento delle bozze o se non lavori in Workfront Proof, apri le seguenti porte:

* 5671
* 5672
* 15671

## Porte da aprire per le e-mail crittografate

Le e-mail provenienti dall’applicazione Workfront vengono inviate crittografate utilizzando le porte 465 e 587. Se il server di posta non supporta i messaggi e-mail crittografati, i messaggi e-mail vengono consegnati non crittografati utilizzando la porta 25.

## Notifiche e-mail dal supporto Workfront

Se non ricevi e-mail dal Supporto Workfront, accertati di aggiungere gli indirizzi IP e i domini Salesforce necessari. Per ulteriori informazioni, consulta l’articolo della guida di Salesforce sugli indirizzi IP e i domini Salesforce da consentire.

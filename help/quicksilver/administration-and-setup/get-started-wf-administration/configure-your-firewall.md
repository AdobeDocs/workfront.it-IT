---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare il inserisco nell'elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo
description: Se il firewall o il server di posta è configurato in modo da consentire l'accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell'elenco Consentiti di. In questo modo si apre la comunicazione tra l'ambiente e i server Adobe Workfront e si consente agli utenti di inviare messaggi da Workfront e di utilizzare l'SSO con Active Directory o LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 8a8a36732800d0f48026b616cc16e4ff30e0ad41
workflow-type: tm+mt
source-wordcount: '1598'
ht-degree: 0%

---

# Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per configurare il inserisco nell&#39;elenco Consentiti di accesso a Adobe Admin Console, se la tua organizzazione è stata integrata, consulta [Domini da consentire per app e servizi di Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Il modo in cui un’organizzazione configura il proprio inserisco nell&#39;elenco Consentiti di è univoco per ogni organizzazione. Collabora con il tuo team IT per identificare la procedura aziendale e implementare queste aggiunte.

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a determinati fornitori, è necessario aggiungere determinati indirizzi IP al relativo inserisco nell&#39;elenco Consentiti di. Questo apre la comunicazione tra l’ambiente e i server Adobe Workfront e consente i seguenti processi:

* Invio di messaggi dall’applicazione Workfront

  >[!NOTE]
  >
  >Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

* Utilizzo dei webhook dei documenti durante la configurazione di integrazioni di documenti personalizzate
* Utilizzo delle sottoscrizioni agli eventi di Workfront

  Per ulteriori informazioni, consulta [API di abbonamento agli eventi](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

È inoltre necessario aprire alcune porte per crittografare i messaggi e-mail al momento della consegna.

## Workfront inserire nell&#39;elenco Consentiti utilizzabili

Se la tua organizzazione dispone del piano Enterprise, puoi anche configurare due Workfront di inserire nell&#39;elenco Consentiti:

* **Inserire nell&#39;elenco Consentiti E-mail**: consente di controllare dove gli utenti possono inviare i dati e-mail memorizzati in Workfront. Per ulteriori informazioni, consulta [Configurare il inserisco nell&#39;elenco Consentiti di e-mail per l e-mail](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **INSERIRE NELL&#39;ELENCO CONSENTITI IP**: limita l’accesso a Workfront a 45 indirizzi IP o intervalli di indirizzi IP specificati dall’utente, fornendo un ulteriore livello di sicurezza per l’applicazione Workfront. Per ulteriori informazioni, consulta [Limita l’accesso ad Adobe Workfront per indirizzo IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Individuare il cluster Workfront

Gli indirizzi IP da aggiungere al elenco Consentiti di sul firewall dipendono dal cluster in cui viene eseguito l’ambiente di produzione.

Per individuare il cluster dell&#39;organizzazione:

1. In qualità di amministratore di Workfront, fai clic su **Menu principale** icona ![Menu principale](assets/main-menu-icon.png), quindi fai clic su **Configurazione**.
1. Nel menu di navigazione a sinistra, fai clic su **Sistema**, quindi seleziona **Informazioni Cliente**.
1. Individua il **Cluster Setup** nell&#39;angolo superiore destro della pagina. Il cluster della tua organizzazione è elencato qui.

   CL01 fa riferimento al cluster 1, CL02 al cluster 2 e così via.

Per ulteriori informazioni, consulta la sezione [Visualizza il piano Workfront e il cluster della tua organizzazione](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) nell’articolo [Panoramica del firewall](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Indirizzi IP da aggiungere al inserisco nell&#39;elenco Consentiti di

>[!IMPORTANT]
>
>Alcune integrazioni Workfront non funzionano quando il inserisco nell&#39;elenco Consentiti di è abilitato perché non possono essere configurate con un indirizzo IP statico. Per utilizzare le seguenti integrazioni, devi disabilitare il inserisco nell&#39;elenco Consentiti di.
>
>* Workfront per G Suite
>* Workfront per Outlook
>* Workfront per Salesforce

* [Indirizzi IP per consentire i cluster 1, 2, 3, 5, 7, 8 e 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Indirizzi IP per consentire il cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Indirizzi IP per consentire il cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Indirizzi IP per consentire un&#39;unità di test](#IP%20Addre2)
* [Indirizzi IP da consentire durante l’implementazione delle sottoscrizioni di eventi](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Indirizzi IP per consentire l’autenticazione avanzata](#ip-addresses-to-allow-for-enhanced-authentication)
* [Indirizzi IP da aggiungere per accedere a Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Indirizzi IP da aggiungere per l’utilizzo di Workfront per Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL da aggiungere per tutti i cluster Workfront](#urls-to-add-for-all-clusters-workfront)

### Indirizzi IP per consentire i cluster 1, 2, 3, 5, 7, 8 e 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Se l&#39;ambiente di produzione si trova nel cluster 1, 2, 3, 5 o 7, è necessario consentire i seguenti indirizzi IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per SSO, webhook di documenti o altre funzionalità</td> 
   <td> 
    <ul> 
     <li>35 160 0 242</li> 
     <li>34 213 36 118</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52.36.154.34</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall’applicazione Workfront</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13 58 86 183</li> 
     <li>34 209 181 84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54 71 252 65</li> 
    </ul> <p>Per informazioni sui seguenti indirizzi IP, vedi <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Nuovi indirizzi IP per l’e-mail di Adobe Workfront con la versione 21.1</a></p> 
    <ul> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>23 251 237 109</li> 
     <li>23 251 237 106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire il cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Se l’ambiente di produzione si trova nel cluster 4, aggiungi i seguenti indirizzi IP per l’SSO, documenta le integrazioni dei webhook e per ricevere e-mail dall’applicazione Workfront:

* 52 31 132 175
* 52.19.188.226
* 52 28 49 94
* 52 29 41 175
* 52.29.197.69
* 52 48 124 108
* 69 169 230 231
* 69,169. 230,232
* 3 121 91 129
* 3 122 11 35
* 34 246 27 40
* 52 208 123 166
* 52 208 159 124
* 52.17.130.201
* 34 252 250 191
* 52.30.133.50
* 54 220 93 204
* 34 254 76 122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

Per informazioni sui seguenti indirizzi IP, vedi [Nuovi indirizzi IP per l’e-mail di Adobe Workfront con la versione 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23 251 239 98
* 23 251 239 99

### Indirizzi IP per consentire il cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Se l&#39;ambiente di produzione si trova nel cluster 6, aggiungere i seguenti indirizzi IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall’applicazione Workfront</td> 
   <td> 
    <ul> 
     <li>34 94 227 64</li> 
     <li>34 94 227 65</li> 
     <li>34 94 227 66</li> 
     <li>34 94 227 67</li> 
     <li>34 66 82 64</li> 
     <li>34 66 82 65</li> 
     <li>34 66 82 66</li> 
     <li>34 66 82 67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per utilizzare il servizio e-mail di AWS</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13 58 86 183</li> 
     <li>34 209 181 84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54 71 252 65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire un&#39;unità di test

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Per ricevere e-mail dall'applicazione Workfront quando si utilizza un'unità di test</td> 
   <td> 
    <ul> 
     <li>69 42 126 188 </li> 
     <li>66 119 37 185</li> 
     <li>66 119 37 186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per le integrazioni SSO e documenta webhook quando si utilizza un’unità di test</td> 
   <td> 
    <ul> 
     <li> <p>69 42 126 188:</p> <p>Per consentire agli utenti di ricevere e-mail da Workfront, questo indirizzo deve essere aggiunto anche al tuo elenco Consentiti di.</p> </li> 
     <li>66 119 37 186</li> 
     <li>66 119 37 167</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
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
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>52.17.130.201</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per clienti in paesi diversi dall'Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52.36.154.34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Indirizzi IP per consentire l’autenticazione avanzata {#ip-addresses-to-allow-for-enhanced-authentication}

Aggiungi i seguenti indirizzi IP per utilizzare l’autenticazione avanzata per l’anteprima o la produzione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se l'ambiente si trova nel cluster 1, 2, 3, 5, 7, 8 o 9</td> 
   <td> 
    <ul> 
     <li>35 167 74 121</li> 
     <li>35 166 202 113</li> 
     <li>35 160 3 103</li> 
     <li>54 183 64 135</li> 
     <li>54 67 77 38</li> 
     <li>54 67 15 170</li> 
     <li>54 183 204 205</li> 
     <li>35 171 156 124</li> 
     <li>18 233 90 226</li> 
     <li>3 211 189 167</li> 
     <li>18 232 225 224</li> 
     <li>34 233 19 82</li> 
     <li>52 204 128 250</li> 
     <li>3 132 201 78</li> 
     <li>3.19.44.88</li> 
     <li>3 20 244 231</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se l'ambiente si trova nel cluster 4</td> 
   <td> 
    <ul> 
     <li>52 28 56 226</li> 
     <li>52 28 45 240</li> 
     <li>52 16 224 164</li> 
     <li>52.16.193,66</li> 
     <li>34 253 4 94</li> 
     <li>52 50 106 250</li> 
     <li>52 211 56 181</li> 
     <li>52 213 38 246</li> 
     <li>52 213 74 69</li> 
     <li>52 213 216 142</li> 
     <li>35 156 51 163</li> 
     <li>35 157 221 52</li> 
     <li>52 28 184 187</li> 
     <li>52 28 212 16</li> 
     <li>52 29 176 99</li> 
     <li>52 57 230 214</li> 
     <li>54 76 184 103</li> 
     <li>52 210 122 50</li> 
     <li>52 208 95 174</li> 
     <li>52.30.133.50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
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
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centro dati Adobe Workfront USA</p> </td> 
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

Inoltre, se l’organizzazione utilizza il filtro di rete in uscita, aggiungi il seguente dominio al tuo elenco Consentiti di accesso a Workfront Fusion per consentire l’accesso al sistema.

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
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] nel cluster di Microsoft Azure</p> </td> 
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
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>52.17.130.201</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
     <li>35 162 128 73</li> 
     <li>52 42 25 64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li> <p>3 209 27 146</p> </li> 
     <li> <p>18 205 251,4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Per clienti in paesi diversi dall'Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52.36.154.34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52.39.217.230</li> 
     <li>35 162 128 73</li> 
     <li>52 42 25 64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
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
* https://app.pendo.io/
* https://cdn.pendo.io/

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
    </ul> <p><b>NOTA</b>:  <p>Non è supportata l’aggiunta di indirizzi IP al inserisco nell'elenco Consentiti di per Workfront Proof. Sono diventati dinamici dopo il passaggio di Workfront ad AWS. È invece consigliabile consentire solo i domini Workfront Proof.</p> <p>Se si verifica un problema durante l’aggiunta di questi domini al tuo inserisco nell'elenco Consentiti di e hai bisogno di un indirizzo IP, contatta l’Assistenza clienti Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Indirizzi IP e URL da aggiungere per accedere a Workfront Proof

Per utilizzare varie funzioni, è necessario aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di.

* [Per callback e bozze di acquisizione Web](#for-callbacks-and-webcapture-proofs)
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
     <li>34 213 36 118</li> 
     <li>35 160 0 242</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>35 165 152 202</li> 
     <li>54 184 151 122</li> 
     <li>35 84 40 190</li> 
     <li>54 218 48 56</li> 
     <li>34 211 224,9</li> 
     <li>52.36.154.34</li> 
     <li>34 232 138 38</li> 
     <li>54 237 6 156</li> 
     <li>54 237 12 32</li> 
     <li>44 241 82 96</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>52 207 47 153</li> 
     <li>50.16.118.214</li> 
     <li>52 54 180 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>34 246 27 40</li> 
     <li>52 208 123 166</li> 
     <li>3 121 91 129</li> 
     <li>3 122 11 35</li> 
     <li>34 241 103 51</li> 
     <li>46 51 203 201</li> 
     <li>54 247 174 227</li> 
     <li>52 208 159 124</li> 
     <li>52.17.130.201</li> 
     <li>34 252 250 191</li> 
     <li>52.30.133.50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> <p><b>NOTA</b>: le opzioni del server DNS non sono più supportate.</p> </td> 
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
     <li> 23 251 237 106</li> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>23 251 239 98</li> 
     <li>69 169 230 231</li> 
     <li>69 169 230 232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Porte aperte per ottenere prestazioni ottimali con Workfront Proof

Se riscontri problemi durante il caricamento delle bozze o se non lavori in Workfront Proof, apri le seguenti porte:

* 5671
* 5672
* 15671

## Porte da aprire per le e-mail crittografate

Le e-mail provenienti dall’applicazione Workfront vengono inviate crittografate utilizzando le porte 465 e 587. Se il server di posta non supporta i messaggi e-mail crittografati, i messaggi e-mail vengono consegnati non crittografati utilizzando la porta 25.

## Notifiche e-mail dal supporto Workfront

Se non ricevi le e-mail dal Supporto Workfront, accertati di aggiungere gli indirizzi IP e i domini Salesforce necessari. Per ulteriori informazioni, consulta l’articolo della guida di Salesforce relativo agli indirizzi IP e ai domini di Salesforce da consentire.

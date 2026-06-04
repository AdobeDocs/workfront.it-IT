---
content-type: reference
navigation-topic: announcements
title: La clientela dei cluster 1, 2 e 3 deve aggiornare eventuali blocchi IP nell’elenco Consentiti per impedire il blocco dei servizi Adobe Workfront
description: Per migliorare la nostra infrastruttura di base, presto i clienti Adobe Workfront nei cluster 01, 02 e 03 verranno migrati al cloud pubblico AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
TQID: https://experienceleague.adobe.com/I6EiM5bD37m-gC5wyB3DBaOscSTMX-18BpjogM1LcgU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 14%

---

# La clientela dei cluster 1, 2 e 3 deve aggiornare eventuali blocchi IP nell’elenco Consentiti per impedire il blocco dei servizi Adobe Workfront

Per migliorare la nostra infrastruttura di base, presto i clienti Adobe Workfront nei cluster 01, 02 e 03 verranno migrati al cloud pubblico AWS.

Come parte di questa modifica, per evitare il blocco dei servizi Workfront è necessario aggiungere i seguenti IP all’:

Per SSO e POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

Per e-mail:

* 54.240.60.174
* 54.240.60.175

Assicurati che i blocchi IP di inserisco nell&#39;elenco Consentiti di siano aggiornati entro il 13 maggio 2019. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Vi ringraziamo per il vostro continuo supporto su Workfront per aiutarci a creare un&#39;esperienza più affidabile e solida per i nostri clienti.

Per ulteriori domande, contatta il nostro team di supporto visitando il sito experience.workfront.com o chiamando il numero verde 844.306.4357 (US) o il numero +44.1256.274200 (EMEA).

## Domande frequenti

### Perché Workfront sta apportando questo cambiamento?

Nel tentativo di offrire ai clienti il miglior servizio possibile, Workfront cerca costantemente di migliorare l&#39;esperienza di utilizzo. Questo cambiamento fa uso di nuove tecnologie che ci permettono di fornire la migliore esperienza possibile e migliorare il nostro già robusto modello di sicurezza.

### Quali azioni sono necessarie in qualità di amministratore di Workfront?

Contatta il reparto di IT o di sicurezza interno per assistenza durante la revisione dei blocchi IP del inserisco nell&#39;elenco Consentiti di e nell’aggiunta degli IP elencati sopra.

### Cosa può aspettarsi la mia organizzazione se non apportiamo questa modifica?

Non potrai accedere ai servizi di Workfront durante la migrazione dei servizi ai nuovi IP.

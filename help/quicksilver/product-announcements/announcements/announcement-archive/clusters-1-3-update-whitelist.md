---
content-type: reference
navigation-topic: announcements
title: I clienti che usano i cluster 1, 2 e 3 devono aggiornare eventuali blocchi IP inserire nell'elenco Consentiti per evitare il blocco dei servizi Adobe Workfront
description: Per migliorare e migliorare l’infrastruttura di base, presto i clienti Adobe Workfront verranno migrati nel cloud pubblico di AWS in base ai cluster 01, 02 e 03.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# I clienti che usano i cluster 1, 2 e 3 devono aggiornare eventuali blocchi IP inserire nell&#39;elenco Consentiti per evitare il blocco dei servizi Adobe Workfront

Per migliorare e migliorare l’infrastruttura di base, presto i clienti Adobe Workfront verranno migrati nel cloud pubblico di AWS in base ai cluster 01, 02 e 03.

Per evitare il blocco dei servizi Workfront, è necessario aggiungere i seguenti IP ai blocchi IP inserire nell&#39;elenco Consentiti:

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

Assicurati che i blocchi IP inserire nell&#39;elenco Consentiti siano aggiornati entro il 13 maggio 2019. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Grazie per il supporto continuo di Workfront, che ci ha permesso di creare un&#39;esperienza più affidabile e solida per i nostri clienti.

Per ulteriori domande, contatta il nostro team di assistenza visitando experience.workfront.com o chiamando il numero 844.306.4357 (US) o il numero +44.1256.274200 (EMEA).

## Domande frequenti

### Perché Workfront sta apportando questo cambiamento?

Nel tentativo di fornire costantemente ai nostri clienti il miglior servizio possibile, Workfront cerca costantemente modi per migliorare l&#39;esperienza utente. Questo cambiamento fa uso di nuove tecnologie che ci permettono di fornire la migliore esperienza possibile e migliorare il nostro modello di sicurezza già robusto.

### Quali azioni sono necessarie da me in qualità di amministratore Workfront?

Contatta il reparto IT o di sicurezza interno per assistenza nella revisione dei blocchi IP inserire nell&#39;elenco Consentiti e nell’aggiunta degli IP elencati sopra.

### Cosa posso aspettarmi dalla mia organizzazione se non apporteremo questa modifica?

Non potrai accedere ai servizi Workfront durante la migrazione dei servizi ai nuovi IP.

---
content-type: reference
navigation-topic: announcements
title: I clienti dei cluster 1, 2 e 3 devono aggiornare eventuali blocchi IP di inserisco nell'elenco Consentiti per impedire il blocco dei servizi Adobe Workfront
description: Per migliorare la nostra infrastruttura di base, presto i clienti Adobe Workfront nei cluster 01, 02 e 03 verranno migrati al cloud pubblico AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# I clienti dei cluster 1, 2 e 3 devono aggiornare eventuali blocchi IP di inserisco nell&#39;elenco Consentiti per impedire il blocco dei servizi Adobe Workfront

Per migliorare la nostra infrastruttura di base, presto i clienti Adobe Workfront nei cluster 01, 02 e 03 verranno migrati al cloud pubblico AWS.

Inserire nell&#39;elenco Consentiti Per evitare il blocco dei servizi Workfront, come parte di questa modifica, è necessario aggiungere i seguenti IP al di blocchi IP:

Per SSO e POP:

* 34 215 145 168
* 54 69 155 48
* 35 160 44 226
* 34 213 96 218
* 3.16.210.22.
* 3 16 229 153
* 18 224 117 99
* 3 18 123 153
* 3 211 159 196
* 3 85 255 45
* 3 210 78 197
* 3 211 23 183

Per e-mail:

* 54 240 60 174
* 54 240 60 175

Assicurati che i blocchi IP di inserisco nell&#39;elenco Consentiti del tuo siano aggiornati entro il 13 maggio 2019. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di protezione del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Vi ringraziamo per il vostro continuo supporto su Workfront per aiutarci a creare un&#39;esperienza più affidabile e solida per i nostri clienti.

Per ulteriori domande, contatta il nostro team di supporto visitando il sito experience.workfront.com o chiamando il numero verde 844.306.4357 (US) o il numero +44.1256.274200 (EMEA).

## Domande frequenti

### Perché Workfront sta apportando questo cambiamento?

Nel tentativo di offrire ai clienti il miglior servizio possibile, Workfront cerca costantemente di migliorare l&#39;esperienza di utilizzo. Questo cambiamento fa uso di nuove tecnologie che ci permettono di fornire la migliore esperienza possibile e migliorare il nostro già robusto modello di sicurezza.

### Quali azioni sono necessarie in qualità di amministratore di Workfront?

Contatta il reparto IT o di sicurezza interno per assistenza durante la revisione dei blocchi IP del elenco Consentiti e l’aggiunta degli IP elencati sopra.

### Cosa può aspettarsi la mia organizzazione se non apportiamo questa modifica?

Non potrai accedere ai servizi di Workfront durante la migrazione dei servizi ai nuovi IP.

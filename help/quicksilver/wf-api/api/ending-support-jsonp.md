---
content-type: api
navigation-topic: api-navigation-topic
title: Fine del supporto di JSONP
description: Fine del supporto di JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Fine del supporto di JSONP

Poiché JSONP (JavaScript con spaziatura) è un vecchio standard con vulnerabilità di sicurezza note, Adobe Workfront non supporterà più JSONP da novembre 2018. Questa decisione sostiene la nostra più ampia iniziativa di modernizzazione della piattaforma Workfront.

JSONP è uno standard tramite il quale è possibile eseguire richieste cross-origin o cross-site. Molti clienti e partner di Workfront utilizzano JSONP per accedere a Workfront da un sistema sul proprio dominio come parte di un’integrazione. JSONP consente l’elaborazione delle richieste da domini non Workfront da parte dell’applicazione Workfront.

Se utilizzi JSONP come parte di una qualsiasi delle integrazioni Workfront, devi aggiornare l’integrazione per utilizzare lo standard CORS (Cross-Origin Resource Sharing). Questo aggiornamento richiede le seguenti operazioni:

1. Invia una richiesta al team di supporto Workfront affinché disponga dei domini utilizzati per effettuare richieste cross-origin al nostro inserisco nell&#39;elenco Consentiti di.

   Per aggiungere i domini al inserisco nell&#39;elenco Consentiti di CORS, contatta l’Assistenza clienti Workfront al numero 844-306-HELP(4357) o inviando un ticket di supporto online.

   >[!NOTE]
   >
   >L’aggiunta di domini al inserisco nell&#39;elenco Consentiti di per CORS è supportata solo per i clienti che utilizzavano JSONP prima del 1° agosto 2018.


1. Per utilizzare CORS, modifica il codice di integrazione.

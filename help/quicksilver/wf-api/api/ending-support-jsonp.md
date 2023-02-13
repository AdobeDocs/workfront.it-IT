---
content-type: api
navigation-topic: api-navigation-topic
title: Terminazione del supporto per JSONP
description: Terminazione del supporto per JSONP
author: John
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Terminazione del supporto per JSONP

Poiché JSONP (JavaScript con spaziatura interna) è un vecchio standard con vulnerabilità di sicurezza note, Adobe Workfront non supporterà più JSONP a partire da novembre 2018. Questa decisione sostiene la nostra più ampia iniziativa per modernizzare la piattaforma Workfront.

JSONP è uno standard in base al quale è possibile eseguire richieste cross-origin o cross-site. Molti clienti e partner Workfront utilizzano JSONP per accedere a Workfront da un sistema sul proprio dominio come parte di un’integrazione. JSONP consente l’elaborazione delle richieste da domini non Workfront da parte dell’applicazione Workfront.

Se utilizzi JSONP come parte di una delle integrazioni Workfront, devi aggiornare l’integrazione per utilizzare lo standard CORS (Cross-Origin Resource Sharing, CORS). Questo aggiornamento richiede di effettuare le seguenti operazioni:

1. Invia una richiesta al team di supporto Workfront per avere tutti i domini utilizzati per effettuare richieste tra origini diverse al nostro inserire nell&#39;elenco Consentiti.

   Per aggiungere i tuoi domini all&#39;inserire nell&#39;elenco Consentiti di CORS, contatta il Servizio Clienti Workfront all&#39;indirizzo 844-306-HELP(4357) o inviando un ticket di supporto online.

   >[!NOTE]
   >
   >L’aggiunta di domini all’inserire nell&#39;elenco Consentiti di CORS è supportata solo per i clienti che utilizzavano JSONP prima del 1° agosto 2018.


1. Apporta modifiche al codice di integrazione per utilizzare CORS.

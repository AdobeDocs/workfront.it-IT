---
product-area: workfront-integrations
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacy e autorizzazioni in Workfront per Google Workspace
description: Privacy e autorizzazioni in Workfront per Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Privacy e autorizzazioni in Workfront per Google Workspace

Poiché la privacy dei clienti è importante, Adobe Workfront non memorizza né raccoglie dati identificativi dei clienti derivanti dall’autorizzazione di terze parti di un’app plug-in di Google. L&#39;utilizzo di Workfront per Google Workspace e il trasferimento delle informazioni ricevute dalle API Google a qualsiasi altra app rispetteranno i [Criteri dei dati utente dei servizi API Google](https://developers.google.com/terms/api-services-user-data-policy), inclusi i requisiti per l&#39;utilizzo limitato.

Sono necessarie le seguenti autorizzazioni affinché il plug-in Workfront for Google Workspace possa fornire il valore massimo:

* **Visualizza i messaggi di posta elettronica quando il componente aggiuntivo è in esecuzione**: il plug-in Workfront for Google Workspace consente agli utenti di risparmiare innumerevoli ore di lavoro duplicato convertendo le e-mail in nuove attività in Workfront e popolando automaticamente il titolo e la descrizione dell&#39;attività con l&#39;oggetto e il corpo dell&#39;e-mail. Il plug-in consente inoltre di pubblicare le e-mail in Workfront come nuovi commenti. Per ottenere questo valore, il plug-in deve visualizzare i messaggi e-mail quando il componente aggiuntivo è in esecuzione.
* **Esegui come componente aggiuntivo Gmail/non sensibile**: sono necessarie autorizzazioni affinché il componente aggiuntivo Workfront for Google Workspace funzioni nell&#39;ambiente Gmail. Il plug-in richiede un ambiente Gmail per funzionare, quindi richiede l&#39;autorizzazione `Run as a Gmail add-on / non-sensitive`.
* **Visualizza i metadati del messaggio di posta elettronica quando il componente aggiuntivo è in esecuzione**: per migliorare i flussi di lavoro, il plug-in Workfront for Google Workspace conferma se un&#39;e-mail è una notifica di Workfront e identifica il tipo di notifica di Workfront (nuova richiesta di lavoro, richiesta di approvazione, nuovo commento, ecc.). Il plug-in richiede l&#39;autorizzazione `View your email message metadata when the add-on is running` per fornire questo valore.
* **Il plug-in deve essere eseguito come componente aggiuntivo del calendario o non sensibile**: il plug-in di Workfront for Google Workspace si connette al calendario dell&#39;utente per consentirgli di visualizzare l&#39;impatto delle attività sulle pianificazioni. Il plug-in richiede l&#39;autorizzazione `Run as a Calendar add-on / non-sensitive` per eseguire questa operazione.
* **Connetti a un&#39;autorizzazione del servizio esterno:** In ultima analisi, il plug-in deve connettersi all&#39;API Workfront, che è la spina dorsale del valore del plug-in. L&#39;API Workfront è un servizio esterno a Google, pertanto il plug-in richiede `Connect to an external service permission` per funzionare.

Per ulteriori informazioni sull&#39;impegno di Adobe Workfront per la privacy dei clienti, consulta [Informativa sulla privacy di Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Per ulteriori informazioni, vedere [Criteri dei dati utente dei servizi API di Google](https://developers.google.com/terms/api-services-user-data-policy).

---
product-area: workfront-integrations
keywords: google,doc,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacy e autorizzazioni in Workfront per G Suite
description: Privacy e autorizzazioni in Workfront per G Suite
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: bd9fb14b99886f4a514c4d37ad9d93be7a051858
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Privacy e autorizzazioni in Workfront per G Suite

Poiché la privacy del cliente è importante, Adobe Workfront non archivia o raccoglie dati identificativi del cliente risultanti dall&#39;autorizzazione di terze parti di un&#39;app plug-in Google. Workfront per l’utilizzo e il trasferimento delle informazioni ricevute dalle API Google a qualsiasi altra app da parte di G Suite si attiene alla [Criteri utente dei servizi API Google](https://developers.google.com/terms/api-services-user-data-policy), compresi i requisiti per l&#39;uso limitato.

È necessario disporre delle seguenti autorizzazioni in modo che il plug-in Workfront for G Suite possa fornire il suo valore massimo:

* **Visualizza i messaggi e-mail quando il componente aggiuntivo è in esecuzione**: Il plug-in Workfront for G Suite consente di risparmiare agli utenti innumerevoli ore di lavoro duplicato convertendo le e-mail in nuove attività in Workfront e compilando automaticamente il titolo e la descrizione dell’attività con l’oggetto e il corpo dell’e-mail. Il plug-in consente inoltre di inviare e-mail a Workfront come nuovi commenti. Per fornire questo valore, il plug-in deve visualizzare i messaggi e-mail quando il componente aggiuntivo è in esecuzione.
* **Esegui come componente aggiuntivo Gmail / non sensibile**: Per il funzionamento del componente aggiuntivo Workfront for G Suite nell’ambiente Gmail sono necessarie le autorizzazioni. Il plug-in richiede il funzionamento di un ambiente Gmail, quindi richiede il `Run as a Gmail add-on / non-sensitive` autorizzazione.
* **Visualizza i metadati del messaggio e-mail quando il componente aggiuntivo è in esecuzione**: Per migliorare i flussi di lavoro, il plug-in Workfront for G Suite conferma se un’e-mail è una notifica Workfront e identifica il tipo di notifica Workfront (nuova richiesta di lavoro, richiesta di approvazione, nuovo commento, ecc.). Il plug-in richiede `View your email message metadata when the add-on is running` autorizzazione a fornire questo valore.
* **Il plug-in deve essere eseguito come componente aggiuntivo Calendario/non sensibile**: Il plug-in Workfront for G Suite si collega al calendario, per consentirti di visualizzare l’impatto delle attività sulle pianificazioni. Il plug-in deve `Run as a Calendar add-on / non-sensitive` il permesso di fare questo.
* **Connettiti a un&#39;autorizzazione del servizio esterno:** In ultima analisi, il plug-in deve connettersi all’API Workfront, che è la spina dorsale del valore del plug-in. L’API di Workfront è un servizio esterno a Google, pertanto il plug-in richiede l’ `Connect to an external service permission` per far funzionare il plug-in.

Per ulteriori informazioni sulla dedizione di Adobe Workfront alla privacy dei clienti, consulta [Avviso sulla privacy Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Per ulteriori informazioni, consulta [Criteri utente dei servizi API Google](https://developers.google.com/terms/api-services-user-data-policy).

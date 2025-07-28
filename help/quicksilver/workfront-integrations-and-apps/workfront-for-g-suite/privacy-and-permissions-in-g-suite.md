---
product-area: workfront-integrations
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacy e autorizzazioni in Workfront per Google Workspace
description: Privacy e autorizzazioni in Workfront per Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Privacy e autorizzazioni in Workfront per Google Workspace

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, le seguenti funzionalità di Workfront per Google Workspace non saranno disponibili dopo il **28 febbraio 2026**:
>
>* Accesso alle funzionalità di Google Workspace da Workfront
>
>* Visualizzazione e gestione delle attività di Workfront da Gmail o dal pannello del sito Calendario di Google
>
>È consigliabile utilizzare l&#39;automazione e l&#39;integrazione di Workfront per le esigenze di integrazione dell&#39;organizzazione con Google Workspace.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Google Workspace, vedere [Moduli Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) e [Moduli calendario Google](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Poiché la privacy dei clienti è importante, Adobe Workfront non memorizza né raccoglie dati identificativi dei clienti derivanti dall’autorizzazione di terze parti di un’app plug-in di Google. L&#39;utilizzo di Workfront per Google Workspace e il trasferimento delle informazioni ricevute dalle API Google a qualsiasi altra app rispetteranno i [Criteri dei dati utente dei servizi API Google](https://developers.google.com/terms/api-services-user-data-policy), inclusi i requisiti per l&#39;utilizzo limitato.

Sono necessarie le seguenti autorizzazioni affinché il plug-in Workfront for Google Workspace possa fornire il valore massimo:

* **Visualizza i messaggi di posta elettronica quando il componente aggiuntivo è in esecuzione**: il plug-in Workfront for Google Workspace consente agli utenti di risparmiare innumerevoli ore di lavoro duplicato convertendo le e-mail in nuove attività in Workfront e popolando automaticamente il titolo e la descrizione dell&#39;attività con l&#39;oggetto e il corpo dell&#39;e-mail. Il plug-in consente inoltre di pubblicare le e-mail in Workfront come nuovi commenti. Per ottenere questo valore, il plug-in deve visualizzare i messaggi e-mail quando il componente aggiuntivo è in esecuzione.
* **Esegui come componente aggiuntivo Gmail/non sensibile**: sono necessarie autorizzazioni affinché il componente aggiuntivo Workfront for Google Workspace funzioni nell&#39;ambiente Gmail. Il plug-in richiede un ambiente Gmail per funzionare, quindi richiede l&#39;autorizzazione `Run as a Gmail add-on / non-sensitive`.
* **Visualizza i metadati del messaggio di posta elettronica quando il componente aggiuntivo è in esecuzione**: per migliorare i flussi di lavoro, il plug-in Workfront for Google Workspace conferma se un&#39;e-mail è una notifica di Workfront e identifica il tipo di notifica di Workfront (nuova richiesta di lavoro, richiesta di approvazione, nuovo commento, ecc.). Il plug-in richiede l&#39;autorizzazione `View your email message metadata when the add-on is running` per fornire questo valore.
* **Il plug-in deve essere eseguito come componente aggiuntivo del calendario o non sensibile**: il plug-in di Workfront for Google Workspace si connette al calendario dell&#39;utente per consentirgli di visualizzare l&#39;impatto delle attività sulle pianificazioni. Il plug-in richiede l&#39;autorizzazione `Run as a Calendar add-on / non-sensitive` per eseguire questa operazione.
* **Connetti a un&#39;autorizzazione del servizio esterno:** In ultima analisi, il plug-in deve connettersi all&#39;API Workfront, che è la spina dorsale del valore del plug-in. L&#39;API Workfront è un servizio esterno a Google, pertanto il plug-in richiede `Connect to an external service permission` per funzionare.

Per ulteriori informazioni sull&#39;impegno di Adobe Workfront per la privacy dei clienti, consulta [Informativa sulla privacy di Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Per ulteriori informazioni, vedere [Criteri dei dati utente dei servizi API di Google](https://developers.google.com/terms/api-services-user-data-policy).

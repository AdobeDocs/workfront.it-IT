---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 - Altri miglioramenti
description: Questa pagina descrive tutti i miglioramenti apportati alle aree generali di Workfront con la versione 2020.1. Questi miglioramenti sono attualmente disponibili nell’ambiente di anteprima e saranno disponibili nell’ambiente di produzione a fine marzo o all’inizio di aprile 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 1%

---

# 2020.1 - Altri miglioramenti

Questa pagina descrive tutti i miglioramenti apportati alle aree generali di Workfront con la versione 2020.1. Questi miglioramenti sono attualmente disponibili nell’ambiente di anteprima e saranno disponibili nell’ambiente di produzione a fine marzo o all’inizio di aprile 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.1, consulta [Panoramica sulla versione 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Modifica necessaria per aggiungere bozze al inserisco nell&#39;elenco Consentiti di

>[!NOTE]
>
>Questa funzione è stata rimossa dalla versione 2020.1. Sarà reso disponibile in un secondo momento.

Il dominio di verifica sta modificando from proofhq.com in workfront.com.

Se il firewall o il server di posta è configurato in modo da consentire l&#39;accesso solo a fornitori specifici, è necessario aggiungere il seguente URL aggiuntivo al inserisco nell&#39;elenco Consentiti di verifica per assicurarsi che gli utenti dell&#39;organizzazione possano visualizzare le bozze all&#39;interno di Workfront sia nel visualizzatore di bozze del browser che nel visualizzatore di bozze del desktop:

&#42;.workfront.com

Anche l&#39;URL &#42;proofhq.com è obbligatorio.

Per ulteriori informazioni sull&#39;aggiornamento del inserisco nell&#39;elenco Consentiti di aggiornamento del tuo, consulta [Configurare il inserisco nell&#39;elenco Consentiti di aggiornamento del tuo firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Questo aggiornamento si applica solo alla verifica in Workfront; non si applica quando si utilizza l’applicazione autonoma Workfront Proof.

## Comportamento dei cookie di Workfront aggiornato per mantenere la compatibilità con Chrome

Per mantenere la compatibilità con un prossimo aggiornamento di Google Chrome (Chrome v80), abbiamo aggiornato la piattaforma Workfront per garantire che i cookie vengano inviati in modo appropriato con le richieste.

Questo aggiornamento di Chrome modifica il valore predefinito dell’attributo per cookie SameSite. Se desideri verificare il comportamento dell’istanza di Workfront dopo l’aggiornamento di Google Chrome, regola i flag in Chrome e abilita le seguenti opzioni:

* &quot;SameSite by default cookies&quot; (Cookie SameSite per impostazione predefinita)
* &quot;Cookies without SameSite must be secure&quot;

## Sincronizzazione commenti Workfront con Jira

L’integrazione Workfront for Jira ora sincronizza i commenti Workfront con il flusso di commenti nativo di Jira.

In precedenza era possibile sincronizzare i commenti da Jira a Workfront, ma non da Workfront a Jira.

Per ulteriori informazioni, vedere [Configurare Adobe Workfront per Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Flash Portfolio Optimizer è stato rimosso

È stata rimossa la possibilità di passare dall’ambiente Portfolio Optimizer nuovo a quello legacy (basato su Flash) dall’ambiente Workfront Classic per tutti i clienti. La versione precedente di Portfolio Optimizer è una funzione obsoleta e i nuovi strumenti forniscono oggi la stessa funzionalità.

Per informazioni su Ottimizzatore portfolio, consulta https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Per informazioni sulla rimozione degli strumenti basati su Flash in Workfront, vedere [Sostituzione degli strumenti basati su Flash in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

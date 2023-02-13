---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Disinstallare il connettore legacy
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Disinstallare Workfront con il connettore legacy Adobe Experience Manager

È necessario disinstallare Workfront con il connettore legacy Adobe Experience Manager per l’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

## Annulla iscrizione a Workfront

1. Apri Adobe Experience Manager.
1. In Experience Manager, vai a **Strumenti** > **Cloud Services** > **Configurazione dell’integrazione Workfront**.
1. Seleziona la configurazione (global-workfront per impostazione predefinita) e fai clic su **Proprietà**.
   ![annullare l’iscrizione al workfront](assets/unsubscribe-from-workfront.png)
1. Disattiva la sincronizzazione di documenti, commenti e metadati. L&#39;etichetta deve essere disabilitata.
Questo rimuoverà gli abbonamenti in Workfront e consentirà all’utente di creare una nuova sottoscrizione utilizzando lo stesso url definito in Day CQ Link Externalizer.

## Eliminare la configurazione di integrazione Workfront

Dopo aver rimosso l’abbonamento, è ora sicuro eliminare la configurazione dell’integrazione di Workfront.

1. Apri la configurazione e seleziona **Elimina**.
   ![elimina configurazione](assets/delete-wf-configuration.png)

## Rimuovi mappatura

Successivamente, devi eliminare la mappatura delle proprietà Workfront.

1. In Experience Manager, vai a **Strumenti** > **Risorse** > **Mappatura delle proprietà Workfront**.

1. Seleziona tutte le mappature e fai clic su **Elimina**.

## Autorizzazioni utente

A tutti gli utenti che accedono AEM Dam da Workfront sono state assegnate autorizzazioni di lettura a `/content/dam`. Se un utente non ne ha più bisogno, è possibile rimuovere le autorizzazioni date a tali utenti.

Il connettore funziona utilizzando il servizio front-service dell&#39;utente del sistema. Questa operazione viene disinstallata durante la disinstallazione del connettore.

>[!NOTE]
>
>Se utilizzi il connettore versione 2.0.3 e hai aggiunto il gruppo `workfront-aem-connector-group`, è necessario rimuovere anche questo **Strumenti** > **Sicurezza** > **Gruppi**.

## Day CQ Link Externalizer

Se non hai bisogno di Day CQ Link Externalizer, puoi ripristinarlo a `localhost:4502` andando `/system/console/configMgr` e cerca &#39;Day CQ Link Externalizer&#39;.

>[!NOTE]
>
>Se utilizzi Adobe Experience Manager as a Cloud Service, puoi modificarlo esaminando il progetto e individuando il file . _com.day.cq.commons.impl.ExternalizerImpl.xml_ interno _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## Disinstallare il pacchetto del connettore

I passaggi necessari per disinstallare il pacchetto del connettore variano a seconda della versione di Adobe Experience Manager in uso.

### Adobe Experience Manager On-Premise

Se utilizzi Adobe Experience Manager on-premise, vai a _crx/packmgr/index.jsp_, e cerca il `workfront-aem-connector.all-<version>.zip`, fai clic su **Altro** e poi **Disinstalla**.

Controlla sotto `/conf` per assicurarsi che tutti i file creati da Workfront siano stati rimossi.

### Adobe Experience Manager as a Cloud Service

Per Adobe Experience Manager as a Cloud Service, puoi rimuovere le dipendenze per il connettore dai file pom.files del progetto.

## Firewall e Dispatcher

Non dimenticare di rimuovere gli URL Workfront inseriti nella whitelist se la comunicazione non è più necessaria. Inoltre, il connettore utilizza le intestazioni apiKey e il nome utente impostati sul dispatcher. Possono essere rimossi.

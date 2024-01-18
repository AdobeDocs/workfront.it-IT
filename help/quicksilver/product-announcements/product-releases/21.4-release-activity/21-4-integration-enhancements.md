---
title: 21.4 Miglioramenti all’integrazione
description: 21.4 Miglioramenti all’integrazione
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 Miglioramenti all’integrazione

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione 21.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 4 ottobre 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.4, consulta [Panoramica sulla versione 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Collega documenti da Dropbox Business

Abbiamo aggiunto Dropbox Business come integrazione di documenti disponibile. Ora è possibile accedere ai documenti archiviati in Dropbox Business direttamente da Workfront.

Dropbox Business consente di collegare documenti condivisi e di caricarli in cartelle condivise. Il Dropbox (non l&#39;azienda di Dropbox) consente solo al proprietario dei documenti di visualizzare il documento in Workfront.

L’amministratore di Workfront può abilitare questa integrazione per la tua organizzazione.

Per ulteriori informazioni, consulta [Collegare documenti da applicazioni esterne](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Per informazioni su come un amministratore di Workfront può abilitare questa opzione, consulta [Configurare le integrazioni dei documenti](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Aggiornamenti a Workfront per Slack

I seguenti aggiornamenti sono ora visibili in Workfront per l’integrazione con Slack:

* Workfront per Slack ha un nuovo aspetto.
* Ora ricevi il Workfront per le notifiche di Slack in tempo reale.

  Ad esempio, se si è assegnati a un&#39;attività, la notifica viene ricevuta non appena si è assegnati. In precedenza, poteva verificarsi un ritardo prima che la notifica apparisse in Slack.

Questo aggiornamento richiede la nuova autorizzazione del Workfront per l’integrazione con Slack. Per informazioni sull’autorizzazione dell’integrazione, consulta [Configurare Adobe Workfront per Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Per ulteriori informazioni su Workfront per le notifiche di Slack, consulta [Ricevere notifiche Adobe Workfront in Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Vedi più chiaramente i dettagli di accesso all’account quando fornisci il consenso alle integrazioni Adobe Workfront

Le schermate di consenso per le integrazioni Adobe Workfront ora sono aggiornate. Ora puoi vedere le azioni e le aree specifiche a cui le integrazioni hanno accesso, in modo da comprendere meglio cosa stai consentendo all’integrazione o all’applicazione di accedere.

Questa nuova schermata di consenso si applica a qualsiasi integrazione Adobe Workfront che utilizza OAuth 2.0.

Per informazioni dettagliate su integrazioni specifiche, consulta la documentazione di tale integrazione.

## L’autenticazione tramite chiave API non è più necessaria per le integrazioni

Le integrazioni Workfront hanno recentemente iniziato a utilizzare OAuth2 per maggiore sicurezza e usabilità. Come parte di questo spostamento, Workfront non richiede più le chiavi API per l’autenticazione delle integrazioni.

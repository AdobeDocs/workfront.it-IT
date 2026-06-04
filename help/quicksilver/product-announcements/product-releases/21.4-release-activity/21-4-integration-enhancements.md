---
title: 21.4 - Miglioramenti per le integrazioni
description: 21.4 - Miglioramenti per le integrazioni
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
TQID: https://experienceleague.adobe.com/dCRr9YQiXiX82Jw7wyeT786T8oJ74-u6kOuevYy-SWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 367
ht-degree: 2%

---

# 21.4 - Miglioramenti per le integrazioni

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione 21.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 4 ottobre 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.4, consulta la [Panoramica sulla versione 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Collega documenti da Dropbox Business

Abbiamo aggiunto Dropbox Business come integrazione di documenti disponibile. Ora è possibile accedere ai documenti archiviati in Dropbox Business direttamente da Workfront.

Dropbox Business consente di collegare documenti condivisi e caricarli in cartelle condivise. Dropbox (non Dropbox Business) consente solo al proprietario dei documenti di visualizzare il documento in Workfront.

L’amministratore di Workfront può abilitare questa integrazione per la tua organizzazione.

Per ulteriori informazioni, consulta [Collegare documenti da applicazioni esterne](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Per informazioni su come un amministratore di Workfront può abilitare questa opzione, vedi [Configurare le integrazioni dei documenti](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Aggiornamenti di Workfront for Slack

Nell’integrazione Workfront for Slack sono ora visibili i seguenti aggiornamenti:

* Workfront per Slack ha un nuovo aspetto.
* Ora ricevi le notifiche Workfront for Slack in tempo reale.

  Ad esempio, se si è assegnati a un&#39;attività, la notifica viene ricevuta non appena si è assegnati. In precedenza, poteva verificarsi un ritardo prima che la notifica apparisse in Slack.

Questo aggiornamento richiede la riautorizzazione dell’integrazione di Workfront per Slack. Per informazioni sull&#39;autorizzazione dell&#39;integrazione, vedere [Configurare Adobe Workfront per Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Per ulteriori informazioni sulle notifiche di Workfront for Slack, vedere [Ricevere notifiche di Adobe Workfront in Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Vedi più chiaramente i dettagli di accesso all’account quando fornisci il consenso alle integrazioni Adobe Workfront

Le schermate di consenso per le integrazioni Adobe Workfront ora sono aggiornate. Ora puoi vedere le azioni e le aree specifiche a cui le integrazioni hanno accesso, in modo da comprendere meglio cosa stai consentendo all’integrazione o all’applicazione di accedere.

Questa nuova schermata di consenso si applica a qualsiasi integrazione Adobe Workfront che utilizza OAuth 2.0.

Per informazioni dettagliate su integrazioni specifiche, consulta la documentazione di tale integrazione.

## L’autenticazione tramite chiave API non è più necessaria per le integrazioni

Le integrazioni Workfront hanno recentemente iniziato a utilizzare OAuth2 per maggiore sicurezza e usabilità. Come parte di questo spostamento, Workfront non richiede più le chiavi API per l’autenticazione delle integrazioni.

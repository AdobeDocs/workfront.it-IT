---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronizzazione degli utenti tra Adobe Workfront e Workfront Proof
description: Le informazioni utente vengono sincronizzate da Adobe Workfront a Workfront Proof; non vengono sincronizzate da Workfront Proof a Workfront. Per questo motivo, ogni volta che crei o modifichi degli utenti, devi apportare tali modifiche all’interno di Workfront. Non è possibile apportare modifiche agli utenti all’interno di Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
TQID: 'https://experienceleague.adobe.com/oHi8YTmAgh3KY1xfh6psNCLr4Gng0iniB3LUqbBzcOw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%
---
# Sincronizzazione degli utenti tra Adobe Workfront e Workfront Proof

Le informazioni utente vengono sincronizzate da Adobe Workfront a Workfront Proof; non vengono sincronizzate da Workfront Proof a Workfront. Per questo motivo, ogni volta che crei o modifichi degli utenti, devi apportare tali modifiche all’interno di Workfront. Non è possibile apportare modifiche agli utenti all’interno di Workfront Proof.

Le sezioni seguenti forniscono informazioni sulla sincronizzazione degli utenti da Workfront a Workfront Proof:

## Informazioni sincronizzate

Workfront sincronizza le seguenti informazioni utente con Workfront Proof:

* Nome (nome e cognome dell’utente)
* Indirizzo e-mail

## Quando si verifica la sincronizzazione

Le informazioni utente vengono sincronizzate da Workfront a Workfront Proof nelle seguenti circostanze:

* Le informazioni di un utente vengono aggiornate in Workfront
* Un utente viene creato in Workfront

A seconda che in Workfront Proof esista un utente con lo stesso indirizzo e-mail, si verifica una delle seguenti situazioni:

* **Se in Workfront Proof e** non esiste alcun utente con un&#39;e-mail corrispondente

  * **La verifica è abilitata per l&#39;utente:** L&#39;utente è stato creato come utente in Workfront Proof.
  * **La verifica non è abilitata per l&#39;utente:** L&#39;utente è stato creato come contatto in Workfront Proof.

* **Se un utente con un messaggio di posta elettronica corrispondente esiste in Workfront Proof:** la verifica è abilitata per tale utente in Workfront (se non era già abilitata) e le informazioni sono sincronizzate tra i due utenti.

  Per ulteriori informazioni, vedere [Configurare l&#39;accesso di verifica di un utente](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Configurare l&#39;accesso di verifica di un utente](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Quando un utente con un messaggio e-mail corrispondente esiste, nel proprio o in un altro ambiente di verifica, Workfront crea un alias e-mail aggiungendo l’ID account dell’utente come suffisso al messaggio e-mail. Ad esempio, *username+accountid@domain.com*. Gli utenti riceveranno comunque le notifiche delle bozze nel caso in cui venga creato un alias e-mail.

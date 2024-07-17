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
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
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

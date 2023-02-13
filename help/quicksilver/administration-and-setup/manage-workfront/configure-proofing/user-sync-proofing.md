---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronizzazione degli utenti tra Adobe Workfront e Workfront Proof
description: Le informazioni utente vengono sincronizzate da Adobe Workfront a Workfront Proof; non viene sincronizzato da Workfront Proof a Workfront. Per questo motivo, ogni volta che crei o modifichi utenti, devi apportare tali modifiche in Workfront. Non è possibile apportare modifiche agli utenti in Workfront Proof.
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

Le informazioni utente vengono sincronizzate da Adobe Workfront a Workfront Proof; non viene sincronizzato da Workfront Proof a Workfront. Per questo motivo, ogni volta che crei o modifichi utenti, devi apportare tali modifiche in Workfront. Non è possibile apportare modifiche agli utenti in Workfront Proof.

Le sezioni seguenti forniscono informazioni sulla sincronizzazione utente da Workfront a Workfront Proof:

## Informazioni sincronizzate

Workfront sincronizza le seguenti informazioni utente con Workfront Proof:

* Nome (nome e cognome dell’utente)
* Indirizzo e-mail

## Quando si verifica la sincronizzazione

Le informazioni utente vengono sincronizzate da Workfront a Workfront Proof nelle seguenti circostanze:

* Le informazioni di un utente vengono aggiornate in Workfront
* Un utente viene creato in Workfront

A seconda che un utente con lo stesso indirizzo e-mail esista in Workfront Proof, si verifica una delle seguenti situazioni:

* **Se non esiste alcun utente con un messaggio e-mail corrispondente in Workfront Proof e**

   * **La correzione è abilitata per l’utente:** L’utente viene creato come utente in Workfront Proof.
   * **La correzione non è abilitata per l’utente:** L’utente viene creato come contatto in Workfront Proof.

* **Se un utente con un messaggio e-mail corrispondente esiste in Workfront Proof:** La correzione è abilitata per tale utente in Workfront (se non era già abilitata) e le informazioni sono sincronizzate tra i due utenti.

   Per ulteriori informazioni, consulta [Configurare l’accesso per la correzione di un utente](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Configurare l’accesso per la correzione di un utente](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Quando esiste un utente con un’e-mail corrispondente, nel proprio o in un altro ambiente di correzione, Workfront crea un indirizzo e-mail alias aggiungendo l’ID account dell’utente come suffisso all’e-mail. Ad esempio: *username+accountid@domain.com*. Gli utenti continueranno a ricevere notifiche di bozza nel caso in cui venga creato un alias e-mail.

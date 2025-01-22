---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Preparare l’onboarding dell’organizzazione in Adobe Admin Console
description: Poiché Adobe Workfront è un prodotto Adobe, puoi accedervi tramite Adobe Admin Console. Questo consente di gestire Workfront insieme ad altri account e prodotti Adobe per i tuoi utenti da una posizione centrale.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Prepara l’onboarding della tua organizzazione in Adobe Admin Console

<!-- Audited: 12/2023 -->

Poiché Adobe Workfront è un prodotto Adobe, puoi accedervi tramite Adobe Admin Console. Questo consente di gestire Workfront insieme ad altri account e prodotti Adobe per i tuoi utenti da una posizione centrale.

Tutti i clienti Workfront verranno infine trasferiti a Adobe Admin Console. Dopo il passaggio dell’organizzazione a Adobe Admin Console, l’autenticazione Workfront viene gestita dalla console. La preparazione e la realizzazione di questo passo in tempi più brevi pongono le basi per l&#39;efficienza nella gestione del lavoro e posizionano la tua organizzazione per un&#39;innovazione più rapida in futuro

Per una panoramica di Adobe Admin Console, vedere [Panoramica di Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html).

## Elenco di controllo per la migrazione

Per garantire che la tua organizzazione possa migrare al Adobe Admin Console, devi eseguire le seguenti azioni.

1. Identifica il Adobe Admin Console desiderato dove desideri aggiungere Workfront.

   * Se la tua organizzazione non dispone di un Adobe Admin Console esistente o se non desideri utilizzare un Adobe Admin Console esistente, il supporto Workfront può aiutarti a crearne uno nuovo.

   * Adobe Se disponi di più Admin Console e non sai quale sia più appropriato aggiungere Workfront a, contatta il supporto Workfront.

1. Confermare con il Supporto Workfront che si desidera utilizzare un Adobe Admin Console esistente o crearne uno nuovo.

1. Configurare la gestione delle identità in Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Preparati a parlare con il supporto Workfront e il tuo team IT in merito alle preferenze di autenticazione, ad esempio Single Sign-on (SSO) o non SSO.

   Per istruzioni, vedere la sezione Identity Management della [Guida alla distribuzione per Adobe Admin Console](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condizionale) Se utilizzi il Single Sign-On, connetti il nuovo Adobe Admin Console al provider SSO esistente.

   Per ulteriori informazioni e istruzioni, vedere [Configurare l&#39;identità](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Se la tua organizzazione non utilizza il Single Sign-On, tutti gli utenti trasferiti a Adobe Admin Console riceveranno un’e-mail per creare il proprio account e la propria password.

1. Assicurati che gli indirizzi e-mail degli utenti siano pronti per la migrazione:

   1. Rimuovi le e-mail duplicate da Workfront.

      Per istruzioni, consulta [Aggiornare gli indirizzi e-mail degli utenti esistenti nella tua istanza di Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [Impedire utenti duplicati](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Se nell&#39;organizzazione sono presenti indirizzi e-mail duplicati, l&#39;utente rappresentato dall&#39;indirizzo e-mail con `lastLoginDate` più recente verrà spostato nell&#39;organizzazione Adobe Admin Console. Tutti gli altri utenti con tale indirizzo e-mail verranno disattivati.

      >[!NOTE]
      >
      >Poiché solo un utente con un determinato indirizzo e-mail può essere attivo alla volta, se devi attivare un altro utente con lo stesso indirizzo e-mail di un utente attualmente attivo, devi disattivare prima l’utente attualmente attivo.

   1. (Condizionale) Se utilizzi integrazioni API personalizzate, verifica che gli utenti dispongano di un indirizzo e-mail valido a cui possono accedere.

   1. (Facoltativo) Si consiglia di disattivare gli utenti che non hanno più bisogno di accedere a Workfront, in modo che non vengano aggiunti al Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Queste azioni relative alle e-mail degli utenti devono essere completate prima che l’organizzazione inizi a spostarsi su Adobe Admin Console.

1. (Facoltativo) Aggiorna tutte le integrazioni personalizzate per utilizzare OAuth2.

   Per istruzioni sulla configurazione delle integrazioni OAuth2, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Questo passaggio è facoltativo ma è vivamente consigliato perché altre forme di autenticazione e autorizzazione API diventeranno in futuro obsolete.

Dopo aver configurato Adobe Admin Console con Workfront, puoi utilizzarlo per creare gli amministratori di sistema di Workfront.

Per ulteriori informazioni, vedere [Gestione degli utenti in Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Per un elenco di altre azioni diverse a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

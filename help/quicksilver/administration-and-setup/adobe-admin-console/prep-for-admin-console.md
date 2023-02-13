---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Preparati a integrare l’organizzazione in Adobe Admin Console
description: Poiché Adobe Workfront è un prodotto di Adobe, puoi accedervi tramite Adobe Admin Console. Questo consente di gestire Workfront insieme ad altri account e prodotti di Adobe per i tuoi utenti in una posizione centrale.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Preparati a integrare l’organizzazione in Adobe Admin Console

Poiché Adobe Workfront è un prodotto di Adobe, puoi accedervi tramite Adobe Admin Console. Questo consente di gestire Workfront insieme ad altri account e prodotti di Adobe per i tuoi utenti in una posizione centrale.

Tutti i clienti Workfront verranno spostati in Adobe Admin Console. Una volta che l’organizzazione si sposta su Adobe Admin Console, l’autenticazione Workfront viene gestita da Adobe Admin Console. La preparazione e la rapida realizzazione di questa iniziativa pone le basi per l&#39;efficienza nella gestione del lavoro e posiziona la tua organizzazione per un&#39;innovazione più rapida in futuro

Per una panoramica di Adobe Admin Console, vedi [Panoramica dell’Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html).

## Lista di controllo della migrazione

Per garantire la migrazione dell’organizzazione a Adobe Admin Console, è necessario eseguire le azioni seguenti

1. Identifica il Adobe Admin Console desiderato in cui desideri aggiungere Workfront.

   * Se la tua organizzazione non dispone di un Adobe Admin Console esistente o se non desideri utilizzare un Adobe Admin Console esistente, il supporto Workfront può aiutarti a crearne uno nuovo.

   * Se disponi di più Admin Console di Adobe e non sei sicuro di quale sia più appropriato aggiungere Adobe Workfront, contatta il supporto Workfront.

1. Conferma con il supporto Workfront se desideri utilizzare un Adobe Admin Console esistente o crearne uno nuovo.

1. Imposta la gestione delle identità su Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Preparati a parlare con il supporto Workfront e il tuo team IT per quanto riguarda le preferenze di autenticazione come Single Sign-on (SSO) o non-SSO.

   Per istruzioni, consulta la sezione Identity Management della Guida alla distribuzione per Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condizionale) Se utilizzi Single Sign-On, connetti il nuovo Adobe Admin Console al provider SSO esistente

   Per ulteriori informazioni e istruzioni, consulta [Imposta identità](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Se la tua organizzazione non utilizza l’accesso Single Sign-On, tutti gli utenti trasferiti a Adobe Admin Console riceveranno un’e-mail per creare il proprio account e la relativa password.

1. Assicurati che gli indirizzi e-mail degli utenti siano pronti per la migrazione:

   1. Rimuovere le e-mail duplicate da Workfront

      Per istruzioni, consulta Aggiornare gli indirizzi e-mail degli utenti esistenti nella tua istanza di Workfront in Impedisci gli utenti duplicati.

      Se nell’organizzazione sono presenti indirizzi e-mail duplicati, l’utente rappresentato dall’indirizzo e-mail con la `lastLoginDate` verranno spostati nell&#39;organizzazione Adobe Admin Console. Tutti gli altri utenti con quell’indirizzo e-mail verranno disattivati.

      >[!NOTE]
      >
      >Poiché solo un utente con un determinato indirizzo e-mail può essere attivo alla volta, se è necessario attivare un altro utente con lo stesso indirizzo e-mail di un utente attualmente attivo, è necessario disattivare l’utente attivo prima di attivare l’utente disattivato.

   2. (Condizionale) Se utilizzi integrazioni API personalizzate, verifica che gli utenti dispongano di un indirizzo e-mail valido a cui possono accedere.

   3. (Facoltativo) Consigliamo di disattivare gli utenti che non hanno più bisogno di accedere a Workfront, in modo che non vengano aggiunti al Adobe Admin Console.
   >[!IMPORTANT]
   >
   >Queste azioni relative alle e-mail degli utenti devono essere completate prima che l’organizzazione inizi a spostarsi su Adobe Admin Console.

1. (Facoltativo) Aggiorna tutte le integrazioni personalizzate per utilizzare OAuth2.

   Per istruzioni sulla configurazione delle integrazioni OAuth2, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   La creazione di integrazioni OAuth2 è disponibile solo nella nuova esperienza Workfront.

   >[!NOTE]
   >
   >Questo passaggio è facoltativo, ma è vivamente consigliato, in quanto in futuro altre forme di autenticazione e autorizzazione API diventeranno obsolete.

Una volta configurato il tuo Adobe Admin Console con Workfront, puoi utilizzarlo per gestire i tuoi utenti.

Per ulteriori informazioni, consulta [Gestione degli utenti in Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Per un elenco delle altre azioni diverse a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

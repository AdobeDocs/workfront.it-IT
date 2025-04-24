---
content-type: overview
navigation-topic: notifications
title: Notifiche degli eventi
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività o problemi. Vengono inviati quando si verifica qualcosa sul progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o entrambe.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Notifiche degli eventi

<!-- Audited: 4/2025 -->

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività o problemi. Vengono inviati quando si verifica qualcosa sul progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o entrambe.

>[!NOTE]
>
>Le notifiche degli eventi sono uno dei diversi tipi di notifiche [!DNL Adobe Workfront]. Per informazioni su tutti i tipi di notifica [!DNL Workfront], vedere [Panoramica notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurazione delle notifiche degli eventi

Le e-mail di notifica degli eventi possono essere configurate ai seguenti livelli:

* **Livello di sistema**: un amministratore di [!DNL Workfront] può attivare e disattivare le notifiche degli eventi a livello di sistema, come spiegato in [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tutti i gruppi ereditano le notifiche di sistema per impostazione predefinita, ma gli amministratori di gruppi potrebbero essere in grado di modificare alcune configurazioni a livello di gruppo se consentito dall&#39;amministratore [!DNL Workfront].

* **Livello gruppo**: un amministratore di gruppo può configurare una notifica evento per i gruppi da gestire dopo che un amministratore [!DNL Workfront] ha sbloccato questa funzionalità per i gruppi. Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per [!DNL Workfront] amministratori (per qualsiasi gruppo). Per ulteriori informazioni, vedere [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **Livello utente**: tutte le notifiche degli eventi attivate a livello di sistema sono elencate nella sezione [!UICONTROL Notifiche] di ogni utente sul suo profilo individuale. Gli utenti possono attivare e disattivare le notifiche dei singoli eventi lì.

  Anche gli amministratori di [!DNL Workfront] e gli utenti con accesso per la modifica di altri utenti possono attivare e disattivare le notifiche nel profilo di un singolo utente.

  Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Le notifiche a livello utente includono anche [!DNL Workfront Goals] notifiche. Tuttavia, l&#39;amministratore di [!DNL Workfront] o l&#39;amministratore del gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Ogni utente deve configurare le proprie notifiche [!DNL Workfront Goals] nel proprio profilo. Se hai accesso a modificare gli utenti, puoi anche modificare queste notifiche per altri utenti. Per abilitare [!DNL Workfront Goals] notifiche per il tuo profilo o per altri utenti a cui hai accesso per la modifica, consulta [Notifiche: Obiettivi](../../workfront-basics/using-notifications/notifications-goals.md).

  Per ulteriori informazioni sulle notifiche configurabili dall&#39;amministratore [!DNL Workfront], vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Contenuto della notifica degli eventi

L&#39;e-mail di notifica dell&#39;evento contiene informazioni sull&#39;evento che si è verificato e un collegamento a [!DNL Workfront] in cui è possibile visualizzare l&#39;evento nel sistema. Per ulteriori informazioni sulla ricezione di notifiche e-mail, vedere [Panoramica delle notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

Un amministratore di [!DNL Workfront] non può modificare il contenuto delle notifiche e-mail come configurato da [!DNL Workfront], ma può modificare le righe dell&#39;oggetto dell&#39;e-mail per le notifiche degli eventi. Per ulteriori informazioni, vedere [Personalizzare gli oggetti e-mail per le notifiche degli eventi](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Per un elenco di tutte le notifiche degli eventi [!DNL Workfront], insieme a una breve descrizione di ogni evento e per informazioni sulla sua attivazione o inattività per impostazione predefinita, vedere [Tipi di notifica degli eventi](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

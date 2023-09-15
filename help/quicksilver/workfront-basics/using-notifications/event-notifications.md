---
content-type: overview
navigation-topic: notifications
title: Notifiche degli eventi
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività o problemi. Vengono inviati quando si verifica qualcosa sul progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o entrambe.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Notifiche degli eventi

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività o problemi. Vengono inviati quando si verifica qualcosa sul progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o entrambe.

>[!NOTE]
>
>Le notifiche degli eventi sono uno dei diversi tipi di [!DNL Adobe Workfront] notifiche. Per informazioni su tutti [!DNL Workfront] tipi di notifica, vedi [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurazione delle notifiche degli eventi

Le e-mail di notifica degli eventi possono essere configurate ai seguenti livelli elencati di seguito. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

* **Livello di sistema**: A [!DNL Workfront] l’amministratore può attivare e disattivare le notifiche degli eventi a livello di sistema, come spiegato in [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tutti i gruppi ereditano le notifiche di sistema per impostazione predefinita, ma gli amministratori di gruppi potrebbero essere in grado di modificare alcune configurazioni a livello di gruppo, se consentito dalla [!DNL Workfront] come spiegato al punto successivo.

* **Livello di gruppo**: un amministratore gruppo può configurare una notifica evento per i gruppi che gestisce dopo un [!DNL Workfront] l’amministratore sblocca questa funzionalità per i gruppi. Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per [!DNL Workfront] amministratori (per qualsiasi gruppo). Per ulteriori informazioni, consulta [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Questa funzionalità è disponibile inizialmente solo per i clienti del cluster 4 come parte di un rollout graduale. Subito dopo sarà disponibile per altri cluster. Questo articolo verrà aggiornato in questo modo.

* **Livello utente**: tutte le notifiche degli eventi attivate a livello di sistema sono elencate in [!UICONTROL Notifiche] sezione sul loro profilo individuale. Gli utenti possono attivare e disattivare le notifiche dei singoli eventi lì.

  [!DNL Workfront] anche gli amministratori e gli utenti con accesso per la modifica di altri utenti possono attivare e disattivare le notifiche nel profilo dei singoli utenti.

  Per ulteriori informazioni, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Le notifiche a livello di utente includono [!DNL Workfront Goals] notifiche. Tuttavia, il [!DNL Workfront] l’amministratore o l’amministratore del gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Ogni utente deve configurare il proprio [!DNL Workfront Goals] nel loro profilo. Se hai accesso a modificare gli utenti, puoi anche modificare queste notifiche per altri utenti. Per abilitare [!DNL Workfront Goals] notifiche per il tuo profilo o per altri utenti a cui puoi accedere per la modifica, consulta [Notifiche: Obiettivi](../../workfront-basics/using-notifications/notifications-goals.md).

  Per ulteriori informazioni sulle notifiche, vedere [!DNL Workfront] l&#39;amministratore può configurare, vedi [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sono disponibili solo in Il nuovo [!DNL Adobe Workfront] esperienza.

## Contenuto della notifica degli eventi

Un messaggio e-mail di notifica dell’evento contiene informazioni sull’evento che si è verificato e contiene un collegamento a [!DNL Workfront] dove puoi vedere l’evento nel sistema. Per ulteriori informazioni sulla ricezione delle notifiche e-mail, consulta [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] l’amministratore non può modificare il contenuto delle notifiche e-mail, in quanto sono configurate da [!DNL Workfront]. Tuttavia, possono modificare l’oggetto delle e-mail di notifica dell’evento. Per ulteriori informazioni, consulta [Personalizzare gli oggetti e-mail per le notifiche degli eventi](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Per un elenco di tutte le [!DNL Workfront] notifiche degli eventi, insieme a una breve descrizione di ciascun evento e del fatto che sia attivo o inattivo per impostazione predefinita, consulta [Notifiche degli eventi disponibili in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

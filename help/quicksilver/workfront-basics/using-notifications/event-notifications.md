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
source-wordcount: '554'
ht-degree: 0%

---

# Notifiche degli eventi

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti come progetti, attività o problemi. Vengono inviati quando si verifica qualcosa sul progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o entrambe.

>[!NOTE]
>
>Le notifiche degli eventi sono uno dei diversi tipi di notifiche [!DNL Adobe Workfront]. Per informazioni su tutti i tipi di notifica [!DNL Workfront], vedi [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurazione delle notifiche degli eventi

Le e-mail di notifica degli eventi possono essere configurate ai seguenti livelli elencati di seguito. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

* **Livello di sistema**: un amministratore di [!DNL Workfront] può attivare e disattivare le notifiche degli eventi a livello di sistema, come spiegato in [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tutti i gruppi ereditano le notifiche di sistema per impostazione predefinita, ma gli amministratori di gruppi potrebbero essere in grado di modificare alcune configurazioni a livello di gruppo, se consentito dall&#39;amministratore [!DNL Workfront], come spiegato nel seguente punto elenco.

* **Livello gruppo**: un amministratore di gruppo può configurare una notifica evento per i gruppi da gestire dopo che un amministratore [!DNL Workfront] ha sbloccato questa funzionalità per i gruppi. Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per [!DNL Workfront] amministratori (per qualsiasi gruppo). Per ulteriori informazioni, vedere [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Questa funzionalità è disponibile inizialmente solo per i clienti del cluster 4 come parte di un rollout graduale. Subito dopo sarà disponibile per altri cluster. Questo articolo verrà aggiornato in questo modo.

* **Livello utente**: tutte le notifiche degli eventi attivate a livello di sistema sono elencate nella sezione [!UICONTROL Notifiche] di ogni utente sul suo profilo individuale. Gli utenti possono attivare e disattivare le notifiche dei singoli eventi lì.

  Anche gli amministratori di [!DNL Workfront] e gli utenti con accesso per la modifica di altri utenti possono attivare e disattivare le notifiche nel profilo dei singoli utenti.

  Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Le notifiche a livello utente includono anche [!DNL Workfront Goals] notifiche. Tuttavia, l&#39;amministratore di [!DNL Workfront] o l&#39;amministratore del gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Ogni utente deve configurare le proprie notifiche [!DNL Workfront Goals] nel proprio profilo. Se hai accesso a modificare gli utenti, puoi anche modificare queste notifiche per altri utenti. Per abilitare [!DNL Workfront Goals] notifiche per il tuo profilo o per altri utenti a cui hai accesso per la modifica, consulta [Notifiche: Obiettivi](../../workfront-basics/using-notifications/notifications-goals.md).

  Per ulteriori informazioni sulle notifiche configurabili dall&#39;amministratore [!DNL Workfront], vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sono disponibili solo nella nuova esperienza [!DNL Adobe Workfront].

## Contenuto della notifica degli eventi

L&#39;e-mail di notifica dell&#39;evento contiene informazioni sull&#39;evento che si è verificato e un collegamento a [!DNL Workfront] in cui è possibile visualizzare l&#39;evento nel sistema. Per ulteriori informazioni sulla ricezione di notifiche e-mail, vedi [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

Un amministratore [!DNL Workfront] non può modificare il contenuto delle notifiche e-mail, in quanto sono configurate da [!DNL Workfront]. Tuttavia, possono modificare l’oggetto delle e-mail di notifica dell’evento. Per ulteriori informazioni, vedere [Personalizzare gli oggetti e-mail per le notifiche degli eventi](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Per un elenco di tutte le notifiche degli eventi [!DNL Workfront], insieme a una breve descrizione di ogni evento e per informazioni sulla sua attivazione o inattività per impostazione predefinita, vedere [Notifiche degli eventi disponibili in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

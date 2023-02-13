---
content-type: overview
navigation-topic: notifications
title: Notifiche degli eventi
description: Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti quali progetti, attività o problemi. Vengono inviati quando si verifica un evento del progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o sia istantanee che giornaliere relative a tale evento.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Notifiche degli eventi

Le notifiche degli eventi sono e-mail attivate da vari tipi di eventi su oggetti quali progetti, attività o problemi. Vengono inviati quando si verifica un evento del progetto di cui altri devono essere a conoscenza. A seconda dell’evento, gli utenti ricevono notifiche e-mail istantanee, giornaliere o sia istantanee che giornaliere relative a tale evento.

>[!NOTE]
>
>Le notifiche degli eventi sono uno dei vari tipi di [!DNL Adobe Workfront] notifiche. Per informazioni su tutti [!DNL Workfront] tipi di notifica, vedi [[!DNL Adobe Workfront] Notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurazione delle notifiche evento

Le e-mail di notifica degli eventi possono essere configurate ai seguenti livelli elencati di seguito. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

* **Livello di sistema**: A [!DNL Workfront] l&#39;amministratore può attivare e disattivare le notifiche degli eventi a livello di sistema, come spiegato in [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Tutti i gruppi ereditano le notifiche di sistema per impostazione predefinita, ma gli amministratori di gruppo potrebbero essere in grado di modificare alcune configurazioni a livello di gruppo, se consentito dal gruppo [!DNL Workfront] amministratore, come spiegato nel punto successivo.

* **Livello del gruppo**: Un amministratore di gruppo può configurare una notifica evento per i gruppi che gestisce dopo un [!DNL Workfront] l’amministratore sblocca questa funzionalità per i gruppi. Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per [!DNL Workfront] amministratori (per qualsiasi gruppo). Per ulteriori informazioni, consulta [Visualizzare e configurare le notifiche evento per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >Questa funzionalità è inizialmente disponibile solo per i clienti del cluster 4 come parte di un rollout graduale. Sarà disponibile per altri cluster a breve. Questo articolo verrà aggiornato man mano che si verifica.

* **Livello utente**: Tutte le notifiche dell&#39;evento attivate a livello di sistema sono elencate nella [!UICONTROL Notifiche] sezione sul loro profilo individuale. Gli utenti possono attivare e disattivare le notifiche dei singoli eventi.

   [!DNL Workfront] gli amministratori e gli utenti con accesso per modificare altri utenti possono anche attivare e disattivare le notifiche nel profilo dei singoli utenti.

   Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >Le notifiche a livello di utente includono anche [!DNL Workfront Goals] notifiche. Tuttavia, [!DNL Workfront] l&#39;amministratore o l&#39;amministratore del gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Ogni utilizzo deve configurare i propri [!DNL Workfront Goals] notifiche nel loro profilo. Se hai accesso per modificare gli utenti, puoi anche modificare queste notifiche per altri utenti. Per attivare [!DNL Workfront Goals] notifiche per il tuo profilo o per altri utenti che hai accesso alla modifica, vedi [Notifiche: Obiettivi](../../workfront-basics/using-notifications/notifications-goals.md).

   Per ulteriori informazioni sulle notifiche di [!DNL Workfront] l&#39;amministratore può configurare, consulta [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sono disponibili solo nel nuovo [!DNL Adobe Workfront] esperienza.

## Contenuto della notifica degli eventi

Un messaggio e-mail di notifica dell’evento contiene informazioni sull’evento che si è verificato e contiene un collegamento a [!DNL Workfront] dove è possibile visualizzare l’evento nel sistema. Per ulteriori informazioni sulla ricezione delle notifiche e-mail, consulta [[!DNL Adobe Workfront] Notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] l’amministratore non può modificare il contenuto delle notifiche e-mail, in quanto sono configurate da [!DNL Workfront]. Tuttavia, possono modificare le righe dell’oggetto delle e-mail di notifica degli eventi. Per ulteriori informazioni, consulta [Personalizzare gli oggetti e-mail per le notifiche degli eventi](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Per un elenco di tutti i [!DNL Workfront] le notifiche degli eventi, insieme a una breve descrizione di ogni evento e se è attivo o inattivo per impostazione predefinita, vedi [Notifiche degli eventi disponibili in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

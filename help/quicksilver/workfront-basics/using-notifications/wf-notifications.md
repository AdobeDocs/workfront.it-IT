---
content-type: overview;reference
navigation-topic: notifications
title: Panoramica delle notifiche
description: Adobe Workfront invia notifiche e-mail, notifiche in-app e notifiche sul dispositivo mobile.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# Panoramica delle notifiche

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] invia notifiche e-mail, notifiche in-app e notifiche sul tuo dispositivo mobile.

## Notifiche e-mail

[!DNL Workfront] invia notifiche e-mail agli utenti in merito alle attività in Workfront e fornisce informazioni e collegamenti utili.

Per modificare le preferenze per le notifiche e-mail, vedi [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Se desideri ricevere notifiche e-mail dall’ambiente Sandbox, devi abilitare le e-mail dal profilo utente in tale ambiente.

Puoi ricevere le seguenti notifiche e-mail da [!DNL Workfront]:

* [Notifiche degli eventi](#event-notifications)
* [Notifiche riepilogo giornaliere](#daily-digest-notifications)
* [Notifica di commenti pubblicati](#notification-of-posted-comments)
* [Promemoria automatici](#automatic-reminders)
* [Notifiche promemoria](#reminder-notifications)
* [Notifiche delle bacheche](#boards-notifications)
* [Altre [!DNL Workfront] e-mail](#other-workfront-emails)

### Notifiche degli eventi

Le notifiche degli eventi vengono in genere attivate da alcuni eventi predefiniti, ad esempio l&#39;assegnazione di un&#39;attività o la ricezione di una risposta a un commento.

Dopo che le notifiche degli eventi sono state attivate nel sistema [!DNL Workfront] dall&#39;amministratore di [!DNL Workfront] o dall&#39;amministratore del gruppo, è possibile selezionare quelle che si desidera ricevere modificando le [!UICONTROL Notifiche] preferenze nel profilo utente. Puoi anche scegliere se ricevere le notifiche man mano che gli eventi si verificano, o se ricevere il riepilogo degli eventi in un’e-mail di riepilogo giornaliero.

È possibile che nelle impostazioni sia presente solo un sottoinsieme di queste notifiche, a seconda di come l&#39;amministratore [!DNL Workfront] ha configurato le notifiche degli eventi per il sistema [!DNL Workfront]. Per ulteriori informazioni, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Lo stato predefinito mostra quali notifiche (giornaliere, istantanee o entrambe) sono abilitate per impostazione predefinita per i nuovi utenti quando li crei.

Per un elenco completo delle notifiche degli eventi e per informazioni su come sono abilitate e configurate a livello di sistema, di gruppo o di utente, vedere [Notifiche degli eventi disponibili in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Per informazioni su come scegliere le notifiche di eventi che si desidera ricevere, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Le notifiche degli eventi sono le uniche notifiche che possono essere configurate per essere consegnate negli aggiornamenti digest giornalieri.

### Notifiche riepilogo giornaliere

Una notifica con riepilogo giornaliero è un’e-mail contenente tutte le notifiche di un certo tipo ricevute nelle 24 ore precedenti l’e-mail.

Per un elenco completo delle notifiche e-mail abilitate per una consegna e-mail di riepilogo giornaliera e per informazioni su tutte le categorie per le notifiche e-mail, vedi [Notifiche evento](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] non invia alcuna notifica di riepilogo giornaliero per le categorie di eventi [!UICONTROL Varie] e [!DNL Goals]. Non è possibile disattivare le notifiche giornaliere per queste categorie.

Quando si ricevono le notifiche di riepilogo giornaliere è necessario tenere presenti diversi aspetti:

* Ogni sezione di [!UICONTROL notifiche] nel pannello **[!UICONTROL Impostazioni personali]** genera il proprio digest e-mail giornaliero. Puoi avere ogni giorno un numero di e-mail di riepilogo pari alle impostazioni di notifica abilitate per le e-mail di riepilogo giornaliero.\
   Ad esempio, se hai selezionato di ricevere un&#39;e-mail di riepilogo giornaliero per diverse azioni nella sezione **[!UICONTROL Informazioni sui progetti di cui sono proprietario],** riceverai una notifica e-mail che elenca tutti gli eventi soddisfatti per quest&#39;area.

* Le notifiche in un messaggio e-mail di riepilogo giornaliero sono raggruppate per vari criteri. Ad esempio, nel caso di **[!UICONTROL Informazioni sui progetti di cui sono proprietario]**, gli eventi sono raggruppati per nome del progetto.

  Per la categoria **[!UICONTROL Comunicazione]**, le notifiche sono raggruppate in base all&#39;oggetto in cui si è verificata la comunicazione.

  >[!NOTE]
  >
  >Per la categoria Comunicazione, puoi selezionare singole notifiche solo per la consegna immediata. Affinché le notifiche vengano recapitate in un riepilogo giornaliero, è necessario selezionarle tutte.

* Il messaggio e-mail di riepilogo giornaliero elenca gli eventi che si sono verificati per le azioni in un&#39;area particolare (come **Informazioni sui progetti di cui sono proprietario**) entro le 24 ore precedenti l&#39;ora scelta per la consegna.
* Il fuso orario per l’ora selezionata per la consegna del riepilogo giornaliero corrisponde al fuso orario, in quanto è configurato sul browser.
* Le e-mail di riepilogo giornaliero hanno il nome della sezione nell’oggetto e la data in cui vengono consegnate.
* Affinché il riepilogo giornaliero possa essere consegnato, almeno un evento deve attivare una notifica. I digest giornalieri non vengono inviati se non vengono soddisfatti eventi contrassegnati per le e-mail di riepilogo giornaliere.

### Notifica di commenti pubblicati

Le notifiche nella categoria [!UICONTROL Comunicazione] ti avvisano dei commenti pubblicati nel flusso [!UICONTROL Aggiornamento] di un elemento specifico.

Le e-mail di riepilogo giornaliero per la categoria [!UICONTROL Comunicazione] sono selezionate per tutte le notifiche disponibili.

Le informazioni vengono riepilogate per l&#39;oggetto in cui si è verificata la comunicazione e per ogni oggetto viene visualizzato un numero totale di messaggi di comunicazione.

Per rispondere al commento o visualizzarlo in Workfront:

1. Fai clic sul pulsante **[!UICONTROL Commento]** nell&#39;e-mail.

   Viene aperta l&#39;area [!UICONTROL Aggiornamenti] dell&#39;oggetto, con il commento specifico evidenziato in blu.

   È aperta una casella di risposta che è possibile utilizzare per rispondere al commento.

Per ulteriori informazioni sulla configurazione delle notifiche e-mail, inclusa l&#39;attivazione delle notifiche di riepilogo giornaliere, vedere [Visualizzare e modificare le impostazioni delle notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [Modificare le notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Promemoria automatici

I promemoria automatici sono abilitati dall&#39;amministratore [!DNL Workfront] per segnalare attività e problemi scaduti, in ritardo o prossimi alla data di completamento pianificata. Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema. Una volta configurati dall&#39;amministratore, non è più possibile disattivarli. Inoltre, non puoi modificare il contenuto o la riga dell’oggetto di un messaggio e-mail attivato da un promemoria automatico.

Possono essere inviati a uno o più dei seguenti individui:

* Gli utenti assegnati a un’attività o a un problema
* Responsabile immediato dell’utente
* Il manager del manager immediato

Le e-mail di promemoria automatici vengono inviate dall&#39;indirizzo e-mail selezionato dall&#39;amministratore [!DNL Workfront] per la gestione delle e-mail in uscita.

A seconda del promemoria automatico attivato, nell’e-mail del promemoria automatico sono disponibili i seguenti tipi di informazioni:

* Data di creazione dell’attività o del problema
* Nome attività o problema
* Nome del progetto in cui si trova l’attività o il problema
* Descrizione dell’attività o del problema
* Un elenco di utenti assegnati all’attività o al problema
* Nome dell’utente che ha inserito l’attività o il problema
* Priorità dell’attività o del problema
* Data di scadenza dell’attività o del problema

Per informazioni sull&#39;attivazione dei promemoria automatici, vedere [Configurare i promemoria automatici](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notifiche promemoria

Un amministratore di [!DNL Workfront] (o un utente con un livello di accesso [!UICONTROL Planner] e accesso amministrativo alle notifiche dei promemoria) può progettare le notifiche dei promemoria sulle scadenze in arrivo e associarle manualmente a progetti, attività, problemi e schede orario.

>[!IMPORTANT]
>
>Se la scadenza cambia dopo che un utente riceve una notifica di promemoria per uno qualsiasi degli oggetti sopra menzionati, l’utente non riceve un’altra notifica di promemoria.

Le notifiche di promemoria vengono inviate dall&#39;indirizzo e-mail selezionato dall&#39;amministratore [!DNL Workfront] per la gestione delle e-mail in uscita.

Per informazioni sulla configurazione e l&#39;attivazione delle notifiche dei promemoria, vedere [Configurare le notifiche dei promemoria](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Per informazioni su come ottenere l&#39;accesso amministrativo richiesto, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notifiche delle bacheche

[!DNL Adobe Workfront] [!UICONTROL Bacheche] ti invia un&#39;e-mail quando sei aggiunto a una bacheca e quando ti viene assegnata una scheda. Puoi selezionare le e-mail che desideri ricevere nelle preferenze delle Bacheche.

Per ulteriori informazioni, consulta [Notifiche e preferenze e-mail per le bacheche](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Altre e-mail di [!DNL Workfront]

Non è possibile configurare altre e-mail che potresti ricevere da [!DNL Workfront].

Le seguenti e-mail vengono inviate automaticamente da [!DNL Workfront] quando vengono soddisfatte queste condizioni:

* Ripristinare un elemento: quando l&#39;amministratore [!DNL Workfront] ripristina un oggetto dal Cestino [!UICONTROL Recycle], viene inviata un&#39;e-mail all&#39;amministratore [!DNL Workfront].
* Impossibile ripristinare: quando l&#39;amministratore [!DNL Workfront] tenta di ripristinare un oggetto dal Cestino e il ripristino non riesce, viene inviata un&#39;e-mail all&#39;amministratore [!DNL Workfront].

Le e-mail seguenti possono essere configurate solo a livello di profilo utente. Non possono essere attivati o disattivati a livello di sistema:

* Completamento di un’attività personale: quando un’attività personale che hai assegnato a un altro utente viene completata, riceverai un’e-mail.
* Commento aggiunto all’utente: quando qualcuno aggiunge un commento al tuo profilo utente, riceverai un’e-mail.

## Notifiche in-app

È possibile ricevere notifiche all&#39;interno dell&#39;applicazione Web [!DNL Workfront] quando si verificano determinati eventi.

Per ulteriori informazioni sulle notifiche in-app, vedere [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notifiche e-mail nell’app e-mail per dispositivi mobili

Puoi ricevere [!DNL Workfront] notifiche e-mail nella tua app e-mail mobile, sul tuo dispositivo mobile.

Se sul telefono è installata l&#39;app mobile [!DNL Workfront], toccando i collegamenti nell&#39;e-mail li si apre nell&#39;app mobile [!DNL Workfront]. Ciò include il tocco di uno dei seguenti pulsanti di azione:

* [!UICONTROL Lavoraci]
* [!UICONTROL Commento]
* [!UICONTROL Decisione di approvazione]
* [!UICONTROL Visualizza tutte le notifiche]
* [!UICONTROL Aggiungi]
* [!UICONTROL Introduzione]
* [!UICONTROL Ulteriori dettagli]

Per ulteriori informazioni sull&#39;app mobile [!DNL Workfront], vedere [Utilizzare l&#39;app mobile  [!DNL Adobe Workfront] ](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).

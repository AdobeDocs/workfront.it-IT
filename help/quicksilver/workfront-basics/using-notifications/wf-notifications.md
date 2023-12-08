---
content-type: overview;reference
navigation-topic: notifications
title: Panoramica delle notifiche
description: Adobe Workfront invia notifiche e-mail, notifiche in-app e notifiche sul dispositivo mobile.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: f0ad08f21101bca3f881b6e5a8267d30ce3988ed
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Panoramica delle notifiche

[!DNL Adobe Workfront] invia notifiche e-mail, notifiche in-app e notifiche sul dispositivo mobile.

## Notifiche e-mail

[!DNL Workfront] invia notifiche e-mail agli utenti in merito all’attività in Workfront e fornisce informazioni e collegamenti utili.

Per modificare le preferenze per le notifiche e-mail, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
* [Altro [!DNL Workfront] email](#other-workfront-emails)

### Notifiche degli eventi

Le notifiche degli eventi vengono in genere attivate da alcuni eventi predefiniti, ad esempio l&#39;assegnazione di un&#39;attività o la ricezione di una risposta a un commento.

Dopo l’attivazione delle notifiche degli eventi nel [!DNL Workfront] sistema in base al [!DNL Workfront] amministratore o amministratore gruppo, puoi selezionare quelli che desideri ricevere modificando il tuo [!UICONTROL Notifiche] preferenze nel profilo utente. Puoi anche scegliere se ricevere le notifiche man mano che gli eventi si verificano, o se ricevere il riepilogo degli eventi in un’e-mail di riepilogo giornaliero.

È possibile che nelle impostazioni venga visualizzato solo un sottoinsieme di queste notifiche, a seconda di come [!DNL Workfront] l&#39;amministratore ha configurato le notifiche degli eventi per [!DNL Workfront] di rete. Per ulteriori informazioni, consulta [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Lo stato predefinito mostra quali notifiche (giornaliere, istantanee o entrambe) sono abilitate per impostazione predefinita per i nuovi utenti quando li crei.

Per un elenco completo delle notifiche degli eventi e informazioni su come vengono abilitate e configurate a livello di sistema, gruppo o utente, consulta [Notifiche degli eventi disponibili in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Per informazioni su come scegliere le notifiche degli eventi da ricevere, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Le notifiche degli eventi sono le uniche notifiche che possono essere configurate per essere consegnate negli aggiornamenti digest giornalieri.

### Notifiche riepilogo giornaliere

Una notifica con riepilogo giornaliero è un’e-mail contenente tutte le notifiche di un certo tipo ricevute nelle 24 ore precedenti l’e-mail.

Per un elenco completo delle notifiche e-mail abilitate per una consegna e-mail con riepilogo giornaliero e per informazioni su tutte le categorie per le notifiche e-mail, consulta [Notifiche degli eventi](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] non invia alcuna notifica di riepilogo giornaliero per [!UICONTROL Varie] e [!DNL Goals] categorie di eventi. Non è possibile disattivare le notifiche giornaliere per queste categorie.

Quando si ricevono le notifiche di riepilogo giornaliere è necessario tenere presenti diversi aspetti:

* Ogni [!UICONTROL notifiche] sezione nel tuo **[!UICONTROL Le mie impostazioni]** il pannello genera la propria e-mail di riepilogo giornaliero. Puoi avere ogni giorno un numero di e-mail di riepilogo pari alle impostazioni di notifica abilitate per le e-mail di riepilogo giornaliero.\
   Ad esempio, se hai selezionato di ricevere un’e-mail di riepilogo giornaliero per diverse azioni effettuate sotto **[!UICONTROL Informazioni sui progetti I] Proprietario,** ricevi un’e-mail di notifica in cui sono elencati tutti gli eventi soddisfatti per questa area.

* Le notifiche in un messaggio e-mail di riepilogo giornaliero sono raggruppate per vari criteri. Ad esempio, nel caso di **[!UICONTROL Informazioni sui progetti di cui sono proprietario]**, gli eventi sono raggruppati per nome del progetto.

  Per **[!UICONTROL Comunicazione]** categoria, le notifiche sono raggruppate in base all’oggetto in cui si è verificata la comunicazione.

  >[!NOTE]
  >
  >Per la categoria Comunicazione, puoi selezionare singole notifiche solo per la consegna immediata. Affinché le notifiche vengano recapitate in un riepilogo giornaliero, è necessario selezionarle tutte.

* L’e-mail di riepilogo giornaliero elenca gli eventi che si sono verificati per le azioni in una particolare area (come **Informazioni sui progetti di cui sono proprietario**) entro le 24 ore precedenti l&#39;orario scelto per la consegna.
* Il fuso orario per l’ora selezionata per la consegna del riepilogo giornaliero corrisponde al fuso orario, in quanto è configurato sul browser.
* Le e-mail di riepilogo giornaliero hanno il nome della sezione nell’oggetto e la data in cui vengono consegnate.
* Affinché il riepilogo giornaliero possa essere consegnato, almeno un evento deve attivare una notifica. I digest giornalieri non vengono inviati se non vengono soddisfatti eventi contrassegnati per le e-mail di riepilogo giornaliere.

### Notifica di commenti pubblicati

Le notifiche in [!UICONTROL Comunicazione] la categoria ti avvisa in caso di commenti pubblicati in [!UICONTROL Aggiorna] flusso di un elemento specifico.

E-mail di riepilogo giornaliero per [!UICONTROL Comunicazione] vengono selezionate per tutte le notifiche disponibili.

Le informazioni vengono riepilogate per l&#39;oggetto in cui si è verificata la comunicazione e per ogni oggetto viene visualizzato un numero totale di messaggi di comunicazione.

Per rispondere al commento o visualizzarlo in Workfront:

1. Fai clic su **[!UICONTROL Commento]** nell’e-mail.

   Il [!UICONTROL Aggiornamenti] viene aperta l&#39;area dell&#39;oggetto, con il commento specifico evidenziato in blu.

   È aperta una casella di risposta che è possibile utilizzare per rispondere al commento.

Per ulteriori informazioni sulla configurazione delle notifiche e-mail, inclusa l’abilitazione delle notifiche con riepilogo giornaliero, consulta [Visualizzare e modificare le impostazioni delle notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Promemoria automatici

I promemoria automatici sono abilitati dal tuo [!DNL Workfront] per segnalare all&#39;utente attività e problemi scaduti, in ritardo o prossimi alla data di completamento pianificata. Per le notifiche in ritardo, l’e-mail viene inviata ogni notte fino al completamento dell’attività o del problema. Una volta configurati dall&#39;amministratore, non è più possibile disattivarli. Inoltre, non puoi modificare il contenuto o la riga dell’oggetto di un messaggio e-mail attivato da un promemoria automatico.

Possono essere inviate a uno o più dei seguenti indirizzi:

* Gli utenti assegnati a un’attività o a un problema
* Responsabile immediato dell’utente
* Il manager del manager immediato

Le e-mail di promemoria automatici vengono inviate dall’indirizzo e-mail a cui l’utente [!DNL Workfront] l’amministratore ha selezionato per gestire le e-mail in uscita.

A seconda del promemoria automatico attivato, nell’e-mail del promemoria automatico sono disponibili i seguenti tipi di informazioni:

* Data di creazione dell’attività o del problema
* Nome attività o problema
* Nome del progetto in cui si trova l’attività o il problema
* Descrizione dell’attività o del problema
* Un elenco di utenti assegnati all’attività o al problema
* Nome dell’utente che ha inserito l’attività o il problema
* Priorità dell’attività o del problema
* Data di scadenza dell’attività o del problema

Per informazioni sull&#39;attivazione dei promemoria automatici, vedere [Impostare promemoria automatici](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notifiche promemoria

A [!DNL Workfront] amministratore (o un utente con [!UICONTROL Planner] livello di accesso e accesso amministrativo per le notifiche dei promemoria) può progettare notifiche dei promemoria sull’approssimarsi delle scadenze e associarle manualmente a progetti, attività, problemi e schede orario.

>[!IMPORTANT]
>
>Se la scadenza cambia dopo che un utente riceve una notifica di promemoria per uno qualsiasi degli oggetti sopra menzionati, l’utente non riceve un’altra notifica di promemoria.

Le notifiche di promemoria vengono inviate dall’indirizzo e-mail che [!DNL Workfront] l’amministratore ha selezionato per gestire le e-mail in uscita.

Per informazioni sulla configurazione e l&#39;attivazione delle notifiche di promemoria, vedere [Configurare le notifiche di promemoria](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Per informazioni su come ottenere l’accesso amministrativo richiesto, consulta [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notifiche delle bacheche

[!DNL Adobe Workfront] [!UICONTROL Schede] ti invia un’e-mail quando sei aggiunto a una bacheca e quando ti viene assegnata una scheda. Puoi selezionare le e-mail che desideri ricevere nelle preferenze delle Bacheche.

Per ulteriori informazioni, consulta [Bacheche notifiche e preferenze e-mail](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Altro [!DNL Workfront] email

Potresti ricevere altre e-mail da [!DNL Workfront] che non può essere configurato.

Le seguenti e-mail vengono inviate automaticamente da [!DNL Workfront] quando sono soddisfatte le seguenti condizioni:

* Ripristina un elemento: quando [!DNL Workfront] l&#39;amministratore ripristina un oggetto da [!UICONTROL Ricicla] Raccoglitore, viene inviata un’e-mail al [!DNL Workfront] amministratore.
* Impossibile ripristinare: quando [!DNL Workfront] l&#39;amministratore tenta di ripristinare un oggetto dal Cestino e il ripristino non riesce, viene inviata un&#39;e-mail al [!DNL Workfront] amministratore.

Le e-mail seguenti possono essere configurate solo a livello di profilo utente. Non possono essere attivati o disattivati a livello di sistema:

* Completamento di un’attività personale: quando un’attività personale che hai assegnato a un altro utente viene completata, riceverai un’e-mail.
* Commento aggiunto all’utente: quando qualcuno aggiunge un commento al tuo profilo utente, riceverai un’e-mail.

## Notifiche in-app

Puoi ricevere notifiche all&#39;interno di [!DNL Workfront] applicazione web, quando si verificano determinati eventi.

Per ulteriori informazioni sulle notifiche in-app, consulta [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notifiche e-mail nell’app e-mail per dispositivi mobili

Puoi ricevere [!DNL Workfront] notifiche e-mail nell’app e-mail mobile, sul dispositivo mobile.

Se si dispone di [!DNL Workfront] L’app mobile installata sul telefono, toccando i collegamenti nell’e-mail, li apre in [!DNL Workfront] App mobile. Ciò include il tocco di uno dei seguenti pulsanti di azione:

* [!UICONTROL Lavoraci]
* [!UICONTROL Commento]
* [!UICONTROL Decidi l&#39;approvazione]
* [!UICONTROL Visualizza tutte le notifiche]
* [!UICONTROL Aggiungi]
* [!UICONTROL Introduzione]
* [!UICONTROL Vedi altri dettagli]

Per ulteriori informazioni su [!DNL Workfront] App mobile, vedi [Utilizza il [!DNL Adobe Workfront] app mobile](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).

---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Accesso [!DNL Adobe Workfront] da [!DNL Slack]
description: Integrazione [!DNL Adobe Workfront] con [!DNL Slack] consente di accedere [!DNL Workfront] dallo Slack, o esegui determinate azioni in [!DNL Workfront] utilizzando un comando slash. L’integrazione può essere utilizzata da qualsiasi [!DNL Slack] ambiente, compresi [!DNL Slack] app mobile.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# Accesso [!DNL Adobe Workfront] da [!DNL Slack]

Integrazione [!DNL Adobe Workfront] con [!DNL Slack] consente di accedere [!DNL Workfront] da [!DNL Slack]o esegue determinate azioni in [!DNL Workfront] utilizzando un comando slash. L’integrazione può essere utilizzata da qualsiasi [!DNL Slack] ambiente, compresi [!DNL Slack] app mobile.

Tu o il tuo [!DNL Slack] l&#39;amministratore deve installare [!DNL Workfront] nella tua app [!DNL Slack] istanza prima di poter utilizzare [!DNL Workfront] da [!DNL Slack]. Per ulteriori informazioni, consulta [Configurare Adobe Workfront per Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Informazioni sui comandi della barra {#about-slash-commands}

Quando utilizzi [!DNL Slack], i messaggi vengono digitati all’interno di un campo messaggio. Quando si avvia il messaggio con una barra, questo diventa un comando e si comporta in modo diverso rispetto a un semplice messaggio. Il comando comunica [!DNL Slack] per eseguire un&#39;azione.

Puoi accedere al tuo [!DNL Workfront] istanza da [!DNL Slack] digitando un comando slash in qualsiasi [!DNL Slack] canale.

Ricorda quanto segue quando si utilizza un comando slash in [!DNL Slack] accesso [!DNL Workfront]:

* I comandi Sbarra sono sensibili all’uso di maiuscole e minuscole.
* Comandi per [!DNL Workfront] sono visibili solo per voi, indipendentemente dal canale in cui li digitate.
* Il comando deve sempre iniziare con `/workfront` o `/wf`, seguito da uno spazio e dal nome di un&#39;azione da eseguire in [!DNL Workfront].

   Indica che il comando è destinato al [!DNL Workfront] app. Comandi per [!DNL Workfront] funziona solo se hai già configurato il [!DNL Workfront] con la tua app [!DNL Slack] istanza.

Per un elenco di tutti i comandi eseguibili dallo Slack [!DNL Workfront], vedi [Accesso [!DNL Workfront] da un comando slash in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Accedi a [!DNL Workfront] da [!DNL Slack] {#log-in-to-workfront-from-slack}

Quando si digita un comando nel campo messaggio in Slack, verrà richiesto di accedere a [!DNL Workfront] prima.\
Per un elenco completo dei [!DNL Workfront] comandi da [!DNL Slack], vedi [Accesso [!DNL Workfront] da un comando slash in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) in questo articolo.

Per accedere a [!DNL Workfront] da [!DNL Slack]:

1. Accedi al tuo [!DNL Slack] istanza.
1. Da qualsiasi canale, digitare uno dei seguenti comandi:\
   `/workfront log in`

   Oppure

   `/wf log in`

1. Fai clic sul pulsante [!DNL Workfront] **[!UICONTROL Accesso]** link visualizzato nella risposta.\
   Viene visualizzata una nuova scheda con campi per [!DNL Workfront] credenziali.

1. Segui le istruzioni per accedere a [!DNL Workfront] utilizzando l’URL SAML (Enhanced Authentication, OAuth 2.0 o Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Quando viene richiesto di accedere all&#39;host del [!DNL Workfront] account, digitare il formato: *la tua azienda&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L’autenticazione avanzata non è disponibile finché non viene [!DNL Workfront] l&#39;amministratore lo abilita per questa integrazione.



   La pagina di configurazione per [!DNL Workfront] notifiche in [!DNL Slack] si apre.

1. (Facoltativo) Disattiva qualsiasi [!DNL Workfront] notifiche che non desideri ricevere in [!DNL Slack].

   Per informazioni sulla configurazione [!DNL Workfront] impostazioni per [!DNL Slack], vedi [Configurare le impostazioni](#configure-settings-configure-settings) sezione del presente articolo

1. Torna alla pagina [!DNL Slack] canale.

   Hai effettuato l&#39;accesso a [!DNL Workfront] dal [!DNL Slack] istanza.

## Accesso [!DNL Workfront] da [!DNL Slack]

* [Informazioni sui comandi della barra](#about-slash-commands-about-slash-commands)
* [Accesso [!DNL Workfront] da un collegamento condiviso in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Accesso [!DNL Workfront] da un comando slash in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedi [Accedi a [!DNL Workfront] da [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo messaggio:

   `/workfront help`

   Oppure

   `/wf help`

1. Selezionare uno dei seguenti comandi:

   * `/wf home`

      Visualizza pulsanti che consentono di accedere a elenchi di attività, problemi e approvazioni. Facendo clic su uno dei pulsanti vengono visualizzati i primi 20 elementi di ciascun elenco in [!DNL Slack].

      Per ulteriori informazioni sulla gestione [!DNL Workfront] elementi di lavoro da [!DNL Slack], vedi [Gestisci il tuo lavoro e le tue approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Includi il nome dell’attività così come apparirà nella [!DNL Workfront] interfaccia.

      Aggiunge un’attività a [!DNL Workfront].

      Per ulteriori informazioni sull’aggiunta di attività a [!DNL Workfront] dallo Slack, vedere &quot;Creazione di attività da [!DNL Slack]&quot; sezione in [Crea attività e problemi da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Includi il nome del problema così come apparirà nella [!DNL Workfront] interfaccia.

      Aggiunge un problema a [!DNL Workfront]

      Per ulteriori informazioni sull’aggiunta di problemi a [!DNL Workfront] da [!DNL Slack], vedi &quot;Creazione di problemi da [!DNL Slack]&quot; sezione in [Crea attività e problemi da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Visualizza l&#39;elenco delle [!DNL Workfront] Preferiti.

      Per ulteriori informazioni sull&#39;accesso ai Preferiti da [!DNL Slack], vedi [Accesso al [!UICONTROL Preferiti] Elenco da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) nella sezione [Accesso a Preferiti ed elementi recenti da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) articolo.

   * `/wf recent`

      Visualizza l&#39;elenco degli elementi a cui hai effettuato l&#39;accesso più di recente in [!DNL Workfront].

      Per ulteriori informazioni sull&#39;accesso agli elementi recenti da [!DNL Slack], vedi [Accesso al [!UICONTROL Articoli recenti] Elenco da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] e [!UICONTROL articoli recenti da [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) articolo.

   * `wf tasks`

      Visualizza un elenco delle attività.

      Per ulteriori informazioni sulla gestione delle attività da [!DNL Slack], consulta &quot;Gestione delle attività da [!DNL Slack]&quot; sezione in [Gestione del lavoro e delle approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Visualizza un elenco dei problemi.

      Per ulteriori informazioni sulla gestione dei problemi, consulta [!DNL Slack], consulta &quot;Gestione dei problemi da [!DNL Slack]&quot; sezione in [Gestione del lavoro e delle approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Visualizza il tuo [!DNL Workfront] approvazioni.\

      Per ulteriori informazioni sulla gestione delle approvazioni da [!DNL Slack], consulta &quot;Gestione delle approvazioni da [!DNL Slack]&quot; sezione in [Gestisci il tuo lavoro e le tue approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      Parola chiave Include.

      Cerca una parola chiave specifica. È possibile cercare i seguenti tipi di oggetti:

      * Progetto
      * Attività
      * Problema
      * Rapporto
      * Persone
      * Modello
      * Documento
      * Portfolio
      * Programma
      * Dashboard
      * Azienda
      * Nota  \

         Per ulteriori informazioni sulla ricerca in [!DNL Slack], vedi [Cerca [!DNL Adobe Workfront] elementi dello Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Accedi a [!DNL Workfront] da [!DNL Slack].

   * `/wf log out `

      Ti disconnette [!DNL Workfront] da [!DNL Slack]. Resta connesso a [!DNL Workfront] se disponi di un [!DNL Workfront] istanza aperta in un&#39;altra scheda del browser in in un&#39;altra applicazione.
   * `/wf settings`

      Consente di configurare il [!DNL Workfront] impostazioni in [!DNL Slack].

      Per informazioni sulla configurazione [!DNL Workfront] Slack, vedere [Configurare le impostazioni](#configure-settings-configure-settings).

   * `/wf help`
Visualizza un elenco completo dei comandi per [!DNL Workfront].


   * `Visit Workfront Help`: Apre la [!UICONTROL Slack] sezione [!DNL Workfront] Sito della guida in una nuova scheda del browser.


1. (Facoltativo) Per eliminare il messaggio di qualsiasi comando, passa il mouse sull&#39;angolo superiore destro del messaggio di Slack contenente il comando e fai clic su &#x200B;**[!UICONTROL Mostra azioni messaggio]**, quindi fai clic su **[!UICONTROL Elimina messaggio]**.

1. (Facoltativo e condizionale) Fai clic su **[!UICONTROL Elimina]** per confermare l&#39;eliminazione del messaggio.

### Accesso [!DNL Workfront] da un collegamento condiviso in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Puoi accedere a [!DNL Workfront] oggetti da un collegamento agli oggetti condivisi con te in [!DNL Slack].

Per ulteriori informazioni sull&#39;accesso [!DNL Workfront] da un collegamento condiviso, vedi [Accesso [!DNL Adobe Workfront] oggetti da un collegamento condiviso in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configurare le impostazioni {#configure-settings}

1. Dentro un [!DNL Slack] campo messaggio, digitare il comando seguente:

   `/workfront settings`

   Oppure

   `/wf settings`

   Tutte le impostazioni sono abilitate per impostazione predefinita.

1. Deseleziona le seguenti opzioni per disabilitare le impostazioni per Workfront:

   * In **[!UICONTROL Impostazioni generali]** area, disattivare **[!UICONTROL Quando si incolla un [!DNL Workfront] URL in un [!DNL Slack] canale, mostrare descrizione aggiuntiva, data di scadenza o nome del richiedente]**&#x200B; impostazione se non desideri [!DNL Slack] per aggiungere ulteriori informazioni sulle [!DNL Workfront] quando si condivide un URL all&#39;oggetto in [!UICONTROL Slack].

   * In **[!UICONTROL Impostazioni delle notifiche]** disattivare le notifiche che si desidera interrompere la ricezione da Workfront.\

      Per informazioni sulla ricezione [!DNL Workfront] notifiche in [!DNL Slack], vedi [Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Esci [!DNL Workfront] da [!DNL Slack]

1. Dentro un [!DNL Slack] campo messaggio, digitare il comando seguente:\
   `/workfront log out` Oppure\
   `/wf log out`\
   Ricevi una conferma della disconnessione [!DNL Workfront].\
   Resta connesso a [!DNL Workfront] se disponi di un [!DNL Workfront] istanza aperta in un&#39;altra scheda del browser in in un&#39;altra applicazione.

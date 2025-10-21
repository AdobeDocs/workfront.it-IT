---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Accesso [!DNL Adobe Workfront] da [!DNL Slack]
description: L'integrazione di  [!DNL Adobe Workfront] con [!DNL Slack] ti consente di accedere a [!DNL Workfront] da Slack o di eseguire determinate azioni in [!DNL Workfront] utilizzando un comando barra. L'integrazione può essere utilizzata da qualsiasi ambiente  [!DNL Slack] , inclusa l'app mobile  [!DNL Slack] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# Accedi a [!DNL Adobe Workfront] da [!DNL Slack]

L&#39;integrazione di [!DNL Adobe Workfront] con [!DNL Slack] consente di accedere a [!DNL Workfront] da [!DNL Slack] o di eseguire determinate azioni in [!DNL Workfront] utilizzando un comando barra. L&#39;integrazione può essere utilizzata da qualsiasi ambiente [!DNL Slack], inclusa l&#39;app mobile [!DNL Slack].

Prima di poter utilizzare [!DNL Slack] da [!DNL Workfront], l&#39;utente o l&#39;amministratore di [!DNL Slack] deve installare l&#39;app [!DNL Workfront] nell&#39;istanza [!DNL Slack]. Per ulteriori informazioni, vedere [Configurare Adobe Workfront per Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Qualsiasi</p>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sui comandi barra {#about-slash-commands}

Quando si utilizza [!DNL Slack], i messaggi vengono digitati all&#39;interno di un campo del messaggio. Quando si avvia un messaggio con una barra, questo diventa un comando e si comporta in modo diverso rispetto a un semplice messaggio. Il comando indica a [!DNL Slack] di eseguire un&#39;azione.

È possibile accedere all&#39;istanza [!DNL Workfront] da [!DNL Slack] digitando un comando barra in qualsiasi canale [!DNL Slack].

Quando si utilizza un comando barra in [!DNL Slack] per accedere a [!DNL Workfront], tenere presente quanto segue:

* I comandi barra fanno distinzione tra maiuscole e minuscole.
* I comandi per [!DNL Workfront] sono visibili solo a te, indipendentemente dal canale in cui li stai digitando.
* Il comando deve sempre iniziare con `/workfront` o `/wf`, seguito da uno spazio e dal nome di un&#39;azione da eseguire in [!DNL Workfront].

  Ciò indica che il comando è destinato all&#39;app [!DNL Workfront]. I comandi per [!DNL Workfront] funzionano solo se l&#39;app [!DNL Workfront] è già stata configurata con l&#39;istanza [!DNL Slack].

Per un elenco di tutti i comandi eseguibili da Slack per [!DNL Workfront], vedere [Accesso [!DNL Workfront] da un comando barra in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Accedi a [!DNL Workfront] da [!DNL Slack] {#log-in-to-workfront-from-slack}

Quando si digita un comando nel campo del messaggio in Slack, verrà richiesto di accedere prima a [!DNL Workfront].\
Per un elenco completo dei comandi [!DNL Workfront] di [!DNL Slack], vedere la sezione [Access [!DNL Workfront] from a slash command in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) in questo articolo.

Per accedere a [!DNL Workfront] da [!DNL Slack]:

1. Accedi all&#39;istanza [!DNL Slack].
1. Da qualsiasi canale, digitate uno dei seguenti comandi:\
   `/workfront log in`

   Oppure

   `/wf log in`

1. Fai clic sul collegamento [!DNL Workfront] **[!UICONTROL Accedi]** visualizzato nella risposta.\
   Viene aperta una nuova scheda con campi per le credenziali [!DNL Workfront].

1. Segui le istruzioni per accedere a [!DNL Workfront] utilizzando l&#39;autenticazione avanzata, OAuth 2.0 o l&#39;URL SAML (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Quando viene richiesto di immettere l&#39;host dell&#39;account [!DNL Workfront], digitarlo in questo formato: *yourCompany&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L&#39;autenticazione avanzata non è disponibile finché non viene abilitata da un amministratore [!DNL Workfront] per questa integrazione.


   Viene visualizzata la pagina di configurazione per le notifiche [!DNL Workfront] in [!DNL Slack].

1. (Facoltativo) Disattivare le notifiche [!DNL Workfront] che non si desidera ricevere in [!DNL Slack].

   Per informazioni sulla configurazione delle impostazioni di [!DNL Workfront] per [!DNL Slack], vedere la sezione [Configurare le impostazioni](#configure-settings-configure-settings) in questo articolo

1. Torna al tuo canale [!DNL Slack].

   Hai effettuato l&#39;accesso a [!DNL Workfront] dalla tua istanza di [!DNL Slack].

## Accedi a [!DNL Workfront] da [!DNL Slack]

* [Informazioni sui comandi barra](#about-slash-commands-about-slash-commands)
* [Accedi [!DNL Workfront] da un collegamento condiviso in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Accedere a [!DNL Workfront] da un comando barra in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere [Accedere a  [!DNL Workfront] da [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo del messaggio:

   `/workfront help`

   Oppure

   `/wf help`

1. Selezionare uno dei seguenti comandi:

   * `/wf home`

     Visualizza i pulsanti da cui è possibile accedere agli elenchi delle attività, dei problemi e delle approvazioni. Facendo clic su uno dei pulsanti vengono visualizzati i primi 20 elementi di ogni elenco in [!DNL Slack].

     Per ulteriori informazioni sulla gestione di [!DNL Workfront] elementi di lavoro da [!DNL Slack], vedi [Gestire il lavoro e le approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Includere il nome dell&#39;attività così come verrà visualizzata nell&#39;interfaccia [!DNL Workfront].

     Aggiunge un&#39;attività a [!DNL Workfront].

     Per ulteriori informazioni sull&#39;aggiunta di attività a [!DNL Workfront] da Slack, vedere la sezione &quot;Creazione di attività da [!DNL Slack]&quot; in [Creazione di attività e problemi da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Includi il nome del problema così come verrà visualizzato nell&#39;interfaccia [!DNL Workfront].

     Aggiunge un problema a [!DNL Workfront]

     Per ulteriori informazioni sull&#39;aggiunta di problemi a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Creazione di problemi da [!DNL Slack]&quot; in [Creare attività e problemi da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Visualizza l&#39;elenco dei Preferiti di [!DNL Workfront].

     Per ulteriori informazioni sull&#39;accesso ai preferiti da [!DNL Slack], vedere la sezione [Accesso all&#39;elenco dei [!UICONTROL preferiti] da  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) nell&#39;articolo [Accesso ai preferiti e agli elementi recenti da  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Visualizza l&#39;elenco degli elementi a cui si è effettuato l&#39;accesso più recente in [!DNL Workfront].

     Per ulteriori informazioni sull&#39;accesso agli elementi recenti da [!DNL Slack], vedere l&#39;articolo [Accesso all&#39;elenco [!UICONTROL Elementi recenti] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] e [!UICONTROL Elementi recenti da [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Visualizza un elenco delle attività.

     Per ulteriori informazioni sulla gestione delle attività da [!DNL Slack], vedere la sezione &quot;Gestione delle attività da [!DNL Slack]&quot; in [Gestione del lavoro e delle approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Visualizza un elenco dei problemi.

     Per ulteriori informazioni sulla gestione dei problemi da [!DNL Slack], consulta la sezione &quot;Gestione dei problemi da [!DNL Slack]&quot; in [Gestione del lavoro e delle approvazioni da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Visualizza le tue [!DNL Workfront] approvazioni.\

     Per ulteriori informazioni sulla gestione delle approvazioni da [!DNL Slack], vedere la sezione &quot;Gestione delle approvazioni da [!DNL Slack]&quot; in [Gestione del lavoro e delle approvazioni da  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Includi parola chiave.

     Cercare una parola chiave specifica. È possibile cercare i seguenti tipi di oggetti:

      * Progetto
      * Attività
      * Problema
      * Rapporto
      * People
      * Modello
      * Documento
      * Portfolio
      * Programma
      * Dashboard di
      * Azienda
      * Nota \

        Per ulteriori informazioni sulla ricerca in [!DNL Slack], vedere [Ricerca di [!DNL Adobe Workfront] elementi da Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Accedi a [!DNL Workfront] da [!DNL Slack].

   * `/wf log out`

     Consente di uscire da [!DNL Workfront] da [!DNL Slack]. Se in un&#39;altra scheda del browser in un&#39;altra applicazione è aperta un&#39;istanza di [!DNL Workfront] separata, l&#39;accesso a [!DNL Workfront] rimane eseguito.
   * `/wf settings`

     Consente di configurare le impostazioni di [!DNL Workfront] in [!DNL Slack].

     Per informazioni sulla configurazione delle impostazioni di [!DNL Workfront] in Slack, vedere [Configurare le impostazioni](#configure-settings-configure-settings).

   * `/wf help`
Visualizza un elenco completo dei comandi per [!DNL Workfront].


   * `Visit Workfront Help`: apre la sezione [!UICONTROL Slack] nel sito della Guida [!DNL Workfront] in una nuova scheda del browser.


1. (Facoltativo) Per eliminare il messaggio di un comando, posizionare il mouse sull&#39;angolo superiore destro del messaggio di Slack contenente il comando e fare clic su&#x200B;**[!UICONTROL Mostra azioni messaggio]**, quindi fare clic su **[!UICONTROL Elimina messaggio]**.

1. (Facoltativo e condizionale) Fare clic su **[!UICONTROL Elimina]** per confermare l&#39;eliminazione del messaggio.

### Accedere a [!DNL Workfront] da un collegamento condiviso in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

È possibile accedere a [!DNL Workfront] oggetti da un collegamento agli oggetti condivisi con te in [!DNL Slack].

Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da un collegamento condiviso, vedere [Accedere agli oggetti [!DNL Adobe Workfront] da un collegamento condiviso in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configurare le impostazioni {#configure-settings}

1. All&#39;interno di un campo di messaggio [!DNL Slack], digitare il comando seguente:

   `/workfront settings`

   Oppure

   `/wf settings`

   Tutte le impostazioni sono attivate per impostazione predefinita.

1. Deseleziona tra le seguenti opzioni, per disabilitare le impostazioni per Workfront:

   * Nell&#39;area **[!UICONTROL Impostazioni generali]**, disabilitare **[!UICONTROL Quando si incolla un URL [!DNL Workfront] in un canale [!DNL Slack], mostrare una descrizione aggiuntiva, una data di scadenza o il nome del richiedente]**&#x200B;impostazione se non si desidera che [!DNL Slack] aggiunga ulteriori informazioni sugli oggetti [!DNL Workfront] quando si condivide un URL all&#39;oggetto in [!UICONTROL Slack].

   * Nell&#39;area **[!UICONTROL Impostazioni notifiche]**, disattivare le notifiche che si desidera interrompere la ricezione da Workfront.\

     Per informazioni sulla ricezione di [!DNL Workfront] notifiche in [!DNL Slack], vedere [Ricevi [!DNL Adobe Workfront] notifiche in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Disconnetti da [!DNL Workfront] da [!DNL Slack]

1. All&#39;interno di un campo di messaggio [!DNL Slack], digitare il comando seguente:\
   `/workfront log out` O\
   `/wf log out`\
   Si riceve la conferma della disconnessione da [!DNL Workfront].\
   Se in un&#39;altra scheda del browser in un&#39;altra applicazione è aperta un&#39;istanza di [!DNL Workfront] separata, l&#39;accesso a [!DNL Workfront] rimane eseguito.

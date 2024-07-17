---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gestire il lavoro e le approvazioni da Slack
description: Puoi accedere alla sezione Work List (Elenco di lavoro) dell’area Home, esaminare e accettare di lavorare su attività e problemi, e rivedere o prendere decisioni sulle approvazioni direttamente dallo Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# Gestisci il tuo lavoro e le approvazioni da [!DNL Slack]

Dopo aver installato [!DNL Adobe Workfront for Slack], è possibile effettuare le seguenti operazioni:

* Accedi agli elenchi degli elementi della [!UICONTROL Home] da [!DNL Slack]
* Rivedi e accetta per lavorare su attività e problemi da [!DNL Slack]
* Rivedi e prendi decisioni sulle approvazioni da [!DNL Slack]

Per ulteriori informazioni sulla configurazione di [!DNL Workfront] con [!DNL Slack], vedere [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Prima di poter gestire il lavoro e le approvazioni da [!DNL Slack], è necessario

* Configura [!DNL Workfront for Slack]\
  Per istruzioni sulla configurazione di [!DNL Workfront for Slack], vedere [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gestisci il tuo lavoro da [!DNL Slack]

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo del messaggio:

   `/workfront home`

   >[!NOTE]
   >
   >* I comandi distinguono tra maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` invece di `/workfront`.

   Vengono visualizzati i pulsanti da cui è possibile accedere agli elenchi delle attività, dei problemi e delle approvazioni. Facendo clic su uno dei pulsanti vengono visualizzati i primi 20 elementi di ogni elenco in [!DNL Slack].

1. (Facoltativo) Fai clic su **[!UICONTROL Attività]** per visualizzare tutte le attività.

   Per ulteriori informazioni sulla gestione delle attività in [!DNL Slack], vedere [Gestione delle attività da [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Facoltativo) Fai clic su **[!UICONTROL Problemi]** per visualizzare tutti i tuoi problemi.

   Per ulteriori informazioni sulla gestione dei problemi in [!DNL Slack], vedere [Gestione dei problemi da [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Facoltativo) Fai clic su **[!UICONTROL Approvazioni]** per visualizzare tutte le approvazioni in attesa della tua decisione.\
   Per ulteriori informazioni sulla gestione delle approvazioni in [!DNL Slack], vedi [Gestire le approvazioni da [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gestisci le tue attività da [!DNL Slack] {#manage-your-tasks-from-slack}

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo del messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Attività]**

   Oppure

   `/workfront tasks`

   >[!NOTE]
   >
   >* I comandi distinguono tra maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` invece di `/workfront`.

   Vengono visualizzate le prime 20 attività dell&#39;elenco.

1. Fai clic su **[!UICONTROL +`<remaining number>` ulteriori]** per visualizzare altre attività.
1. Esaminare le informazioni seguenti relative agli elementi di lavoro:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Nome progetto]** o **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** elemento di lavoro.
   * **[!DNL Assigned By Name]**: nome dell&#39;utente che ti ha assegnato l&#39;attività.
   * **[!UICONTROL Stato]**

1. (Facoltativo) Fai clic sul nome di un elemento per aprirlo in Workfront in una scheda del browser separata.
1. (Facoltativo) Nel campo **[!UICONTROL Stato]**, seleziona un nuovo Stato.
1. (Facoltativo) Fai clic su **[!UICONTROL Ora registro]**, quindi seleziona un Tipo di **[!UICONTROL Ora]** e un&#39;ora per registrare l&#39;ora sull&#39;elemento.

   >[!NOTE]
   >
   >* Puoi registrare le ore solo con incrementi di un’ora intera o di mezz’ora, fino a 12 ore e 30 minuti.
   >* Le ore registrate hanno una data di ingresso di oggi. Impossibile registrare l&#39;ora per una data passata o futura da [!DNL Slack].

   Ricevi una conferma che l’ora è stata registrata.

1. (Facoltativo) Fai clic su **[!UICONTROL Lavoraci]** per accettare di lavorare su un&#39;attività. Il pulsante [!UICONTROL Lavoraci] scompare.

## Gestisci i tuoi problemi da [!DNL Slack] {#manage-your-issues-from-slack}

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere [Accesso a [!DNL Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo del messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Problemi]**

   Oppure

   `/workfront issues`

   >[!NOTE]
   >
   >* I comandi distinguono tra maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` invece di `/workfront`.

   Vengono visualizzati i primi 20 problemi dell’elenco.

1. Fai clic su **[!UICONTROL + rimanenti `<number>` ulteriori]** per visualizzare elementi aggiuntivi.
1. Esaminare le informazioni seguenti relative agli elementi di lavoro:

   * **[!UICONTROL Nome]**
   * Nome **[!UICONTROL Progetto]** o nome oggetto padre
   * **[!UICONTROL Scadenza il]** Data: questa è la data di completamento pianificata dell&#39;elemento di lavoro.
   * Nome **[!DNL Requested by]**: è il contatto principale (per i problemi) o l&#39;utente che ha effettuato l&#39;assegnazione (per le attività).

1. (Facoltativo) Fai clic sul nome del problema per aprirlo in Workfront in una scheda del browser separata.
1. (Facoltativo) Fai clic su **[!DNL Work on it]** per iniziare a lavorare su problemi che non hai ancora accettato.

   Il pulsante [!UICONTROL Lavoraci] scompare.

## Gestisci le tue approvazioni da [!DNL Slack] {#manage-your-approvals-from-slack}

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo del messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Approvazioni]**

   Oppure

   `/workfront approvals`

   >[!NOTE]
   >
   >* I comandi distinguono tra maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` invece di `/workfront`.

   Vengono visualizzati i primi 20 elementi dell&#39;elenco **[!UICONTROL Approvazioni]**. Vengono visualizzate anche informazioni aggiuntive sugli elementi, come il nome dell’utente che lo ha richiesto o il nome del progetto a cui appartiene l’elemento.

1. Fai clic su **[!UICONTROL + rimanenti `<number>` ulteriori]** per visualizzare elementi aggiuntivi.

1. Valuta la gestione delle approvazioni per i seguenti oggetti:

   * **Progetti**

     Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per accettare o rifiutare la modifica dello stato di un progetto.

   * **Attività**

     Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per accettare o rifiutare la modifica dello stato di un&#39;attività.

   * **Problemi**

     Fai clic su **[!UICONTROL Approva]** o **[!DNL Reject]** per accettare o rifiutare la modifica di stato di un problema.

   * **Documenti**

     Fai clic su **[!UICONTROL Approva]** per approvare un documento, **[!UICONTROL Rifiuta]** per rifiutarlo o **[!UICONTROL Modifiche]** per indicare che è stato approvato, ma che il documento richiede ulteriori modifiche.\
     (Facoltativo) Posizionare il puntatore del mouse sulla miniatura del documento per fare clic sulla lente di ingrandimento e visualizzare l&#39;anteprima del documento.

   * **Bozze**&#x200B;Fare clic sul nome della bozza per aprirla in [!DNL Workfront] in una scheda separata e gestire l&#39;approvazione.
   * **Richieste di accesso**

     Fai clic su **[!UICONTROL Concedi l&#39;accesso]** per concedere autorizzazioni avanzate all&#39;oggetto richiesto oppure su **[!UICONTROL Ignora]** per ignorare la richiesta di accesso aggiuntivo.

1. (Facoltativo) Fare clic sul nome dell&#39;oggetto inviato per l&#39;approvazione per aprirlo in [!DNL Workfront] in una nuova scheda del browser.

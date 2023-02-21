---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gestione del lavoro e delle approvazioni dallo Slack
description: È possibile accedere all'elenco Home Work, rivedere e accettare di lavorare su attività e problemi, e rivedere o prendere decisioni sulle approvazioni direttamente dallo Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 1%

---

# Gestisci il tuo lavoro e le tue approvazioni da [!DNL Slack]

Dopo aver installato [!DNL Adobe Workfront for Slack], puoi effettuare le seguenti operazioni:

* Elenchi di accesso [!UICONTROL Pagina principale] oggetti da [!DNL Slack]
* Consulta e accetta di lavorare su attività e problemi da [!DNL Slack]
* Rivedere e prendere decisioni sulle approvazioni da [!DNL Slack]

Per ulteriori informazioni sulla configurazione [!DNL Workfront] con [!DNL Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di gestire il lavoro e le approvazioni da [!DNL Slack], devi

* Configura [!DNL Workfront for Slack]\
   Per istruzioni sulla configurazione [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gestire il lavoro da [!DNL Slack]

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo messaggio:

   `/workfront home`

   >[!NOTE]
   >
   >* I comandi sono sensibili all’uso di maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` anziché `/workfront`.


   Vengono visualizzati i pulsanti che consentono di accedere agli elenchi delle attività, dei problemi e delle approvazioni. Facendo clic su uno dei pulsanti vengono visualizzati i primi 20 elementi di ciascun elenco in [!DNL Slack].

1. (Facoltativo) Fai clic su **[!UICONTROL Attività]** per visualizzare tutte le attività.

   Per ulteriori informazioni sulla gestione delle attività in [!DNL Slack], vedi [Gestione delle attività da [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Facoltativo) Fai clic su **[!UICONTROL Problemi]** per visualizzare tutti i problemi.

   Per ulteriori informazioni sulla gestione dei problemi in [!DNL Slack], vedi [Gestione dei problemi da [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Facoltativo) Fai clic su **[!UICONTROL Approvazioni]** per visualizzare tutte le approvazioni in attesa della decisione.\
   Per ulteriori informazioni sulla gestione delle approvazioni in [!DNL Slack], vedi [Gestisci le approvazioni da [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gestione delle attività da [!DNL Slack] {#manage-your-tasks-from-slack}

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Attività]**

   Oppure

   `/workfront tasks`

   >[!NOTE]
   >
   >* I comandi sono sensibili all’uso di maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` anziché `/workfront`.


   Vengono visualizzate le prime 20 attività dell’elenco.

1. Fai clic su **[!UICONTROL +`<remaining number>` more]** per visualizzare attività aggiuntive.
1. Considera la revisione delle seguenti informazioni sugli elementi di lavoro:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Nome progetto]** o **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** dell&#39;elemento di lavoro.
   * **[!DNL Assigned By Name]**: nome dell’utente che ha assegnato l’attività.
   * **[!UICONTROL Stato]**

1. (Facoltativo) Fai clic sul nome di un elemento per aprirlo in Workfront in una scheda separata del browser.
1. (Facoltativo) In **[!UICONTROL Stato]** selezionare un nuovo stato.
1. (Facoltativo) Fai clic su **[!UICONTROL Tempo di log]**, quindi seleziona un **[!UICONTROL Tipo ora]** e un importo di un&#39;ora per il log time sull&#39;elemento.

   >[!NOTE]
   >
   >* È possibile registrare solo ore in incrementi di un&#39;ora intera o di mezz&#39;ora, fino a 12 ore e 30 minuti.
   >* Le ore di registrazione hanno una data di ingresso di oggi. Non è possibile registrare l&#39;ora di una data passata o futura da [!DNL Slack].


   Ricevi una conferma che l’ora è stata registrata.

1. (Facoltativo) Fai clic su **[!UICONTROL Lavorare]** accettare di lavorare su un&#39;attività. La [!UICONTROL Lavorare] il pulsante scompare.

## Gestire i problemi da [!DNL Slack] {#manage-your-issues-from-slack}

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedi [Accesso a [!DNL Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Problemi]**

   Oppure

   `/workfront issues`

   >[!NOTE]
   >
   >* I comandi sono sensibili all’uso di maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` anziché `/workfront`.


   Vengono visualizzati i primi 20 problemi dell’elenco.

1. Fai clic su **[!UICONTROL + rimanente `<number>` more]** per visualizzare elementi aggiuntivi.
1. Considera la revisione delle seguenti informazioni sugli elementi di lavoro:

   * **[!UICONTROL Nome]**
   * **[!UICONTROL Progetto]** Nome o nome dell&#39;oggetto principale
   * **[!UICONTROL A causa di]** Data: Si tratta della data di completamento pianificata dell&#39;elemento di lavoro.
   * **[!DNL Requested by]** Nome: Si tratta del contatto principale (per i problemi) o dell&#39;utente che ha effettuato l&#39;assegnazione (per le attività).

1. (Facoltativo) Fai clic sul nome del problema per aprirlo in Workfront in una scheda separata del browser.
1. (Facoltativo) Fai clic su **[!DNL Work on it]** per iniziare a lavorare su problemi che non hai ancora accettato.

   La [!UICONTROL Lavorare] il pulsante scompare.

## Gestisci le approvazioni da [!DNL Slack] {#manage-your-approvals-from-slack}

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo messaggio:

   `/workfront home`, quindi fai clic su **[!UICONTROL Approvazioni]**

   Oppure

   `/workfront approvals`

   >[!NOTE]
   >
   >* I comandi sono sensibili all’uso di maiuscole e minuscole.
   >* Puoi avviare il comando con `/wf` anziché `/workfront`.


   I primi 20 elementi sul tuo **[!UICONTROL Approvazioni]** visualizzazione elenco. Vengono visualizzate anche informazioni aggiuntive sugli elementi, ad esempio il nome dell’utente che lo ha richiesto o il nome del progetto a cui appartiene l’elemento.

1. Fai clic su **[!UICONTROL + rimanente `<number>` more]** per visualizzare elementi aggiuntivi.

1. È consigliabile gestire le approvazioni per i seguenti oggetti:

   * **Progetti**

      Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per accettare o rifiutare la modifica dello stato di un progetto.

   * **Attività**

      Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per accettare o rifiutare la modifica dello stato di un&#39;attività.

   * **Problemi**

      Fai clic su **[!UICONTROL Approva]** o **[!DNL Reject]** per accettare o rifiutare la modifica dello stato di un problema.

   * **Documenti**

      Fai clic su **[!UICONTROL Approva]** per approvare un documento, **[!UICONTROL Rifiuta]** per respingerlo, oppure **[!UICONTROL Modifiche]** per indicare che è stato approvato, ma che il documento necessita di ulteriori modifiche.\
      (Facoltativo) Passa il puntatore del mouse sulla miniatura del documento per fare clic sulla lente di ingrandimento e visualizzare l’anteprima del documento.

   * **Bozze**&#x200B; Fai clic sul nome della bozza per aprirla in [!DNL Workfront] in una scheda separata e gestisci l’approvazione.
   * **Richieste di accesso**

      Fai clic su **[!UICONTROL Accesso concesso]** per concedere autorizzazioni avanzate all’oggetto richiesto, oppure **[!UICONTROL Ignora]** per ignorare la richiesta di maggiore accesso.

1. (Facoltativo) Fai clic sul nome dell’oggetto inviato per l’approvazione per aprirlo in [!DNL Workfront] in una nuova scheda del browser.

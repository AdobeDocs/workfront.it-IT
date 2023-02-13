---
product-area: requests
navigation-topic: create-requests
title: Creare e inviare richieste Adobe Workfront
description: Il lavoro pianificato è rappresentato in Adobe Workfront da progetti e attività. Tuttavia, puoi lavorare in un ambiente in cui il lavoro non pianificato, sotto forma di richieste casuali, può arrivare in qualsiasi momento. Workfront fornisce un flusso di lavoro per soddisfare questo tipo di ambiente tramite l’utilizzo di Code di richieste.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# Creare e inviare richieste Adobe Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

Il lavoro pianificato è rappresentato in Adobe Workfront da progetti e attività. Tuttavia, puoi lavorare in un ambiente in cui il lavoro non pianificato, sotto forma di richieste casuali, può arrivare in qualsiasi momento. Workfront fornisce un flusso di lavoro per soddisfare questo tipo di ambiente tramite l’utilizzo di Code di richieste. 

Dopo aver creato una richiesta in una coda di richiesta, è possibile assegnarla per il completamento oppure convertirla in un&#39;attività o in un progetto.\
Per ulteriori informazioni sulla conversione dei problemi in un&#39;attività o in un progetto, consulta l&#39;articolo [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Puoi creare una richiesta nei seguenti modi:

* Da zero come descritto in questo articolo.
* Da bozze. Per informazioni, consulta [Creare richieste dalle bozze](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* Da una richiesta esistente, copiando e inviando una copia. Per informazioni, consulta [Copia e invia richieste](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Requisiti di accesso

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti per l’utilizzo delle code di richiesta

In qualità di amministratore di Workfront, è necessario creare code di richiesta e renderle disponibili agli utenti prima che possano utilizzare questa funzionalità. Anche un utente con una licenza Planner e con accesso Modifica a progetti e autorizzazioni Gestione a un progetto specifico può creare code di richieste. 

Per informazioni su come creare code di richieste, consulta l’articolo [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

È necessario creare i seguenti componenti di una coda richieste:

* Un progetto nello stato Corrente, pubblicato come coda di richiesta della Guida.
* Argomenti Coda.\
   Per ulteriori informazioni, consulta l’articolo [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Regole di instradamento.\
   Per ulteriori informazioni, consulta l’articolo [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Facoltativo) Gruppi Di Argomenti.\
   Per ulteriori informazioni, consulta l’articolo [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Facoltativo) Richiedi modulo personalizzato.\
   Per ulteriori informazioni, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Facoltativo) Richiedi il processo di approvazione.\
   Per ulteriori informazioni, consulta l’articolo [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Creare richieste e generare bozze nell’app web Workfront

Quando crei una richiesta nell’app Web Workfront, Workfront la salva come bozza prima di inviarla. Workfront crea una bozza non appena selezioni la coda di richiesta e inizi a immettere le relative informazioni.

Puoi continuare a inviare la richiesta oppure completare tutte le informazioni disponibili e navigare lontano per completarla in un secondo momento. Workfront salva la richiesta di bozza avviata nella cartella Bozze.

>[!IMPORTANT]
>
>Quando si utilizzano le bozze, tenere presente quanto segue:
>
>* Workfront non crea richieste di bozza quando le invii da un’applicazione di terze parti, ad esempio inviandole tramite e-mail in Workfront, o creandole utilizzando un’altra applicazione. Quando invii una richiesta da fuori dell’app Web Workfront, la richiesta viene salvata nella sezione Inviata .
>* Se la struttura di una coda di richiesta cambia, non è più possibile accedere alle bozze esistenti. Ad esempio, se un argomento della coda viene rimosso o viene aggiunto un gruppo di argomenti, le bozze salvate non saranno più accessibili.
>


Per informazioni sulla creazione di richieste da bozze esistenti, vedi [Creare richieste dalle bozze](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Per informazioni sull&#39;eliminazione delle bozze di richiesta, vedere anche [Eliminare una bozza di richiesta](../../../manage-work/requests/create-requests/delete-request-draft.md).

Per creare una richiesta nell’app Web Workfront: 

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Fai clic su  **Richieste**, quindi fai clic su **Nuova richiesta** nell’angolo superiore destro della pagina.

   >[!TIP]
   >
   >* Puoi accedere all’opzione Nuova richiesta da qualsiasi sezione dell’area Richieste .
   >* L’opzione Nuova richiesta è disattivata quando non hai accesso per creare problemi.


1. (Condizionale) Fai clic all’interno del **Tipo di richiesta** e eseguire una delle operazioni seguenti:

   * Da **Percorsi recenti** seleziona un percorso utilizzato di recente per aprire una coda di richiesta. Un percorso include la coda delle richieste, i gruppi di argomenti e l&#39;argomento della coda a cui hai inviato di recente. Per impostazione predefinita vengono visualizzati gli ultimi tre percorsi.

      >[!NOTE]
      >
      >Workfront salva un percorso solo quando hai effettivamente inviato una richiesta ad esso. Non crea percorsi per le richieste di abbozzo.

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * Da **Code di richieste** seleziona una coda di richiesta.
   * Immetti una parola chiave che appartiene a un percorso precedentemente visitato per cercare una coda di richieste.

      Ad esempio, se disponi di una coda di richiesta denominata &quot;Help Desk&quot; con un gruppo di argomenti denominato &quot;Location&quot; e un argomento della coda denominato &quot;Remote&quot;, puoi digitare &quot;remote&quot; e tutte le code di richiesta che contengono &quot;remote&quot; in qualsiasi elemento del loro percorso di visualizzazione.

      >[!TIP]
      >
      >Quando si digita un nome che contiene un carattere speciale, vengono visualizzati la coda di richiesta, l&#39;argomento della coda o il gruppo di argomenti anche quando si omette di digitare il carattere.

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      L’elenco delle code di richiesta disponibili e dei percorsi recenti viene aggiornato dinamicamente per includere solo i percorsi che contengono la parola chiave evidenziata nei risultati.

      I risultati della ricerca vengono visualizzati nelle seguenti aree:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Code di richieste</td> 
        <td>Richiedi code che contengono la parola chiave nel loro nome</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Percorsi delle richieste</td> 
        <td> <p>Percorsi (che includono code di richiesta, gruppi di argomenti, argomenti di coda) che contengono la parola chiave in uno qualsiasi dei nomi dei loro elementi</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* Le prime 200 code di richieste vengono visualizzate per impostazione predefinita, in ordine alfabetico.
   >* Il nome della coda di richiesta è il nome del progetto pubblicato come coda di richiesta della Guida.
   >* La descrizione del progetto configurato come coda di richiesta selezionata viene visualizzata a destra del nome della coda di richiesta.

   >   
   >Per ulteriori informazioni su come pubblicare un progetto come coda di richiesta della Guida, consulta l’articolo [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. In **Nuova richiesta** eseguire una delle operazioni seguenti:

   * (Condizionale) Seleziona una bozza disponibile dal messaggio di notifica visualizzato nel campo Tipo di richiesta .

      Questa area viene visualizzata solo se prima sono state salvate le bozze senza inviarle.

      Per impostazione predefinita vengono visualizzate le tre bozze più recenti di tre diversi argomenti della coda.

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Inizia a immettere una nuova richiesta nella coda selezionata.

      Una nuova bozza ti viene salvata automaticamente nella sezione Bozze dopo aver inserito le informazioni per la nuova richiesta e aver assegnato un nome alla richiesta nel campo Oggetto.

1. (Facoltativo) Se la coda di richiesta include gruppi di argomenti, selezionare il nome del gruppo di argomenti nel primo campo a discesa. In caso contrario, selezionare un argomento della coda.

   >[!TIP]
   Quando si passa il mouse su un gruppo di argomenti o su un argomento della coda, il campo Descrizione viene visualizzato a destra. Questo contiene informazioni aggiuntive sul gruppo di argomenti o sull&#39;argomento della coda.
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   Nella coda delle richieste è possibile integrare fino a 10 livelli di gruppi di argomenti.\
   Per ulteriori informazioni su come creare gruppi di argomenti, consulta l’articolo [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Per ulteriori informazioni sulla creazione degli argomenti della coda, consulta l’articolo [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   Se hai selezionato una bozza o un percorso precedente, i gruppi di argomenti e gli argomenti della coda sono già selezionati. Se necessario, puoi selezionarne uno diverso.

1. A seconda dei campi abilitati dall’amministratore di Workfront nel **Nuovi campi problema** della sezione **Dettagli coda** nella sottoscheda del progetto, potresti trovare uno dei campi seguenti quando invii una nuova richiesta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Oggetto</strong> </td> 
      <td>Specifica un nome per la richiesta. Questo campo è obbligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Specifica una descrizione della richiesta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Specifica un URL che potrebbe riferirsi alla richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorità</strong> </td> 
      <td> <p>Specifica una priorità per la richiesta. La priorità dovrebbe definire la velocità con cui si ritiene che questa richiesta debba essere risolta. Le opzioni predefinite sono: </p> 
       <ul> 
        <li>Nessuno</li> 
        <li>Basso </li> 
        <li>Normal</li> 
        <li>Alta</li> 
        <li>Urgente</li> 
       </ul> <p>L’amministratore di sistema può modificare i nomi delle priorità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravità</strong> </td> 
      <td> <p>Specifica una gravità per la richiesta. La gravità deve definire l'impatto che questa richiesta ha sul tuo lavoro se non viene risolta in tempo. Le opzioni predefinite sono:</p> 
       <ul> 
        <li>Cosmetico</li> 
        <li>Causa Confusione</li> 
        <li>Bug con workaround</li> 
        <li>Bug senza workaround</li> 
        <li>Errore Fatale</li> 
       </ul> <p>L’amministratore di sistema può modificare i nomi delle severità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contatto principale</strong> </td> 
      <td>Per impostazione predefinita, il contatto principale di una richiesta viene contattato automaticamente, in quanto tu sei la persona che punta a rispondere a qualsiasi domanda relativa alla richiesta. Tuttavia, è possibile modificare questo valore in qualsiasi altro utente Workfront.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Assegnazioni</strong> </td> 
      <td> <p><span>Specifica il nome di un utente attivo, un ruolo di lavoro o un team a cui assegnare la richiesta.</span> </p> <p>È possibile specificare un solo team.</p>

   <p> A seconda della configurazione della coda di richiesta, è possibile assegnare alla richiesta solo uno o due tipi di risorsa, invece dei tre (ad esempio, è possibile assegnare la richiesta solo agli utenti).</p>

   <p>Se una regola di instradamento è associata anche alla coda di richiesta e instrada automaticamente la richiesta a un tipo diverso di risorsa (ad esempio, un team), la richiesta viene assegnata sia all'entità specificata manualmente durante l'invio della richiesta (utenti) sia alla risorsa specificata nella regola di instradamento (team). </p>

   <p> Per ulteriori informazioni, consulta i seguenti articoli:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di routing</a> <br> </p> </li> 
      </ul> </p>

   <p><span>È consigliabile utilizzare le regole di routing per le code di richieste in modo che possano essere instradate automaticamente alle risorse appropriate.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Lavoro Necessario</strong> </td> 
      <td> <p>Stimare quante ore sono necessarie per il completamento della richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di inizio pianificata</strong> </td> 
      <td> <p>Specifica la data in cui deve iniziare il lavoro su questa richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di completamento Pianificata</strong> </td> 
      <td>Specifica la data in cui desideri risolvere la richiesta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Stato</strong> </td> 
      <td>Lo stato predefinito di una nuova richiesta è "Nuovo". Il nome dello stato potrebbe essere stato modificato dall'amministratore di sistema. È inoltre possibile modificare lo stato impostandolo su un'altra opzione nel menu a discesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documenti</strong> </td> 
      <td> <p>Aggiungi i documenti alla tua richiesta. </p> <p> A seconda di come è stata impostata la coda di richiesta, la sezione Documenti potrebbe essere visualizzata prima o dopo i campi personalizzati. </p> <p>I documenti caricati in Workfront vengono memorizzati per 24 ore in una richiesta redatta. Dopo di che, è necessario allegarle nuovamente quando si torna a modificare e inviare la bozza. I documenti collegati da altre unità vengono salvati in modo permanente nella bozza. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Se l’amministratore di Workfront ha associato un modulo personalizzato alla coda di richiesta o all’argomento della coda, specificare i campi all’interno del modulo personalizzato.\
   I moduli personalizzati sono diversi per ogni istanza di Workfront. 
1. (Facoltativo e condizionale) In qualsiasi momento durante l’immissione della richiesta, fai clic su [!UICONTROL **Elimina bozza**] per eliminare la bozza creata automaticamente. Questo elimina la bozza che non può essere recuperata. Viene visualizzato un messaggio di conferma per confermare l&#39;eliminazione della bozza.

1. (Facoltativo) Fai clic su [!UICONTROL **Annulla**] nel messaggio di conferma se desideri ripristinare l’azione e mantenere la bozza.

1. Esegui una delle operazioni seguenti:

   * Fai clic su **Invia** se sei pronto a inviare la richiesta. La richiesta viene salvata nella sezione Inviata . A seconda della regola di routing della coda di richiesta, questa richiesta potrebbe essere indirizzata a un progetto diverso da quello designato come coda di richiesta. Per informazioni sulle regole di routing, vedi [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      Oppure

      Fai clic su **Chiudi** se non sei pronto a inviarlo e potresti tornare e finirlo più tardi. La richiesta viene salvata nella sezione Bozze e sarà disponibile al prossimo invio di una richiesta per questa coda di richiesta.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   Quando invii la richiesta, la bozza elimina automaticamente e non può essere ripristinata.

   Per informazioni sulla gestione delle richieste in arrivo, consulta l’articolo [Gestione delle richieste di lavoro e team](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Per informazioni sull’individuazione delle richieste inviate o redatte, consulta anche [Individua richieste inviate](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Creare richieste dall’esterno di Workfront

Puoi condividere un collegamento diretto a una coda di richiesta quando invii una nuova richiesta e incorporala in altre applicazioni. Gli utenti che accedono a questo collegamento dal web o da altre applicazioni devono anche essere connessi con un account Workfront attivo per poter accedere a questa coda e inviare le richieste ad essa. Per informazioni, consulta [Condividere un collegamento a una coda di richiesta](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Creare richieste tramite e-mail in Workfront

Se la coda richieste è abilitata per ricevere le richieste tramite e-mail, puoi inviare le richieste direttamente all’e-mail associata alla coda richieste.

Il testo del corpo dell’e-mail viene aggiunto come descrizione della richiesta.

>[!NOTE]
La formattazione di HTML viene rimossa quando la richiesta entra in Workfront, ma le firme e il contenuto del thread Reply-to esistente non vengono rimossi e vengono visualizzati nella descrizione della richiesta.

Per informazioni su come abilitare una coda di richieste per ricevere le richieste tramite e-mail, vedi [Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Creare richieste utilizzando il client di Outlook

È possibile inviare richieste utilizzando il client di Outlook. Puoi creare una nuova richiesta oppure convertire un’e-mail in una richiesta. 

Per informazioni sull&#39;invio di richieste tramite il client di Outlook, vedere l&#39;articolo [Creare una richiesta Adobe Workfront da un messaggio e-mail di Outlook](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Creare richieste utilizzando l’app mobile Workfront

Puoi inviare richieste utilizzando l’app mobile sul tuo smartphone. Puoi creare una nuova richiesta e inviarla alle code di richiesta a cui hai accesso per visualizzare nell’applicazione web. 

Per informazioni sull’invio di richieste tramite l’app mobile, consulta la [Richieste](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) sezione degli articoli:

* [Adobe Workfront per Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront per iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## Creare richieste da altre applicazioni

Puoi inviare richieste utilizzando qualsiasi applicazione integrata con Workfront: 

* Puoi creare un’integrazione personalizzata tra Workfront e un’altra applicazione che ti consente di inviare richieste a Workfront dall’altra applicazione.\
   Per ulteriori informazioni sulle integrazioni personalizzate di Workfront, consulta l’articolo [Integrazioni Adobe Workfront](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Puoi inviare richieste da Salesforce se hai installato l’app Workfront per Salesforce.\
   Per informazioni sull’invio di richieste da Salesforce tramite la nostra app Workfront per Salesforce, consulta l’articolo [Inviare richieste Adobe Workfront dagli oggetti Salesforce](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Individua richieste inviate

Per informazioni su come individuare le richieste inviate o redatte, vedi [Individua richieste inviate](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

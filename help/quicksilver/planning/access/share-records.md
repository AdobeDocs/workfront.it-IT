---
title: Condividi record
description: Puoi condividere i record utilizzando il pulsante Condividi per aumentare la collaborazione in Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# Condividere i record

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

È possibile modificare le autorizzazioni delle persone per singoli record di un tipo di record.

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Condividere un collegamento al record.

  Per ulteriori informazioni, vedere [Condividere record utilizzando un collegamento](/help/quicksilver/planning/records/share-records.md).

* Condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro e il tipo di record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Condividere un’area di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

   * [Condividere un tipo di record](/help/quicksilver/planning/access/share-record-types.md)

* Condividi un record utilizzando l&#39;opzione **Condividi**.

  Questo articolo descrive come condividere un record con altri utenti utilizzando l&#39;opzione **Condividi**.

>[!IMPORTANT]
>
>Gli utenti con accesso a un&#39;area di lavoro ottengono automaticamente almeno le autorizzazioni di visualizzazione per tutti i record dell&#39;area di lavoro.
>La condivisione delle visualizzazioni non concede agli utenti le autorizzazioni per i record. Solo le aree di lavoro condivise possono concedere agli utenti le autorizzazioni per tipi di record e record.
>
>Per informazioni generali sulla condivisione di oggetti in Workfront Planning, vedere anche [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> 
Oppure
<p>Qualsiasi pacchetto di Workflow e Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
   <p><b>NOTA</b></p>
   <p>Solo le persone con una licenza Standard possono ottenere le autorizzazioni di gestione per i record. Tutte le altre licenze possono disporre solo delle autorizzazioni di visualizzazione e l’opzione Gestisci non è attiva.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  <p>Gestire le autorizzazioni per un'area di lavoro, un tipo di record e il record</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Solo gli utenti con le autorizzazioni di gestione di un'area di lavoro possono condividere un record</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la condivisione dei record

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* Puoi condividere i record con le seguenti entità: persone, gruppi, team, aziende o mansioni.
* Quando si condivide un record, gli utenti hanno lo stesso accesso ovunque tale record venga visualizzato nel sistema.
* Se si limitano le autorizzazioni a un record, gli utenti non visualizzano più tale record e i valori dei relativi campi di ricerca in qualsiasi punto del sistema in cui viene aggiunto il record.
* Workfront controlla le autorizzazioni dei record nelle connessioni fino a 5 record in profondità, garantendo agli utenti di visualizzare solo i record condivisi con loro.
* È possibile concedere a un record i livelli di autorizzazione seguenti:

   * Visualizzazione
   * Gestione
* Per impostazione predefinita, quando si condivide un&#39;area di lavoro e un tipo di record con gli utenti, questi ultimi ricevono anche le stesse autorizzazioni per i record nell&#39;area di lavoro.
Quando gli utenti dispongono delle autorizzazioni Contribute per un&#39;area di lavoro o un tipo di record, ricevono le autorizzazioni Manage (Gestione) per i record di quel tipo.
* Quando rimuovi un’entità da un’area di lavoro, tutte le autorizzazioni di condivisione vengono rimosse dai tipi di record e da tutti i record in essa contenuti.
* L’accesso di un utente al record è determinato dalla combinazione delle tre impostazioni seguenti:

   * Le relative autorizzazioni ereditate dal tipo di record e dall’area di lavoro
   * Autorizzazioni aggiunte singolarmente nella finestra di dialogo di condivisione dei record
   * Le seguenti autorizzazioni:

      * **Tutti nell&#39;area di lavoro possono visualizzare**: in questo modo il record sarà visualizzabile da tutti gli utenti nell&#39;area di lavoro <!-- is this OK to say "workspace? should it be "record"??-->
      * **Solo le persone invitate possono accedere**: questa opzione è selezionata per impostazione predefinita e consente di limitare l&#39;accesso al record a persone specifiche.

     >[!NOTE]
     >
     >Se si sceglie di concedere a **Everyone nell&#39;area di lavoro l&#39;autorizzazione di visualizzazione** per un tipo di record o un record, tutti gli utenti elencati nell&#39;elenco di condivisione delle autorizzazioni dell&#39;area di lavoro disporranno delle stesse autorizzazioni per il tipo di record e il record, anche quando le autorizzazioni ereditate sono disabilitate.


* Per impostazione predefinita, quando si condivide un record con un utente, questi vengono aggiunti con la stessa autorizzazione disponibile per il tipo di record.

  Ad esempio:

   * Se dispongono delle autorizzazioni di visualizzazione per il tipo di record, ottengono le autorizzazioni di visualizzazione per il record
   * Se dispongono delle autorizzazioni Contribuisci o Gestisci per il tipo di record, ottengono le autorizzazioni Gestione per il record

* In qualità di manager area di lavoro, puoi condividere un record con un utente che non dispone di autorizzazioni per il tipo di record o l’area di lavoro. In questo caso, accanto all’entità aggiunta viene visualizzato un avviso che informa che non è possibile accedere all’area di lavoro o al tipo di record. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> È possibile continuare ad aggiungere l&#39;utente al record e aggiungerlo anche al tipo di record e all&#39;area di lavoro oppure annullare la condivisione.

* Quando un utente dispone delle autorizzazioni Gestisci o Contribuisci per l’area di lavoro e il tipo di record e li aggiungi alle autorizzazioni del record, le autorizzazioni Visualizza vengono disattivate. Mantengono le stesse autorizzazioni del record di quelle del tipo di record e non è possibile concedere loro autorizzazioni inferiori. <!--Lilit is checking on this, it is not working correctly-->

  Se dispongono delle autorizzazioni di visualizzazione per l&#39;area di lavoro o il tipo di record, conservano le autorizzazioni di visualizzazione per i record. Puoi concedere loro le autorizzazioni di gestione del record disabilitando le autorizzazioni ereditate e selezionando l’impostazione Accesso consentito solo alle persone invitate. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* È possibile disabilitare le autorizzazioni ereditate per un singolo record, nel qual caso è possibile assegnare loro autorizzazioni per singoli record oppure ottenere autorizzazioni se appartengono all&#39;opzione **Tutti nell&#39;area di lavoro possono visualizzare**.

* Se più autorizzazioni di condivisione si applicano allo stesso utente, quest&#39;ultimo riceve l&#39;autorizzazione più elevata.

  Ad esempio, se un record è condiviso con un utente con autorizzazioni di visualizzazione e il relativo gruppo con l&#39;accesso Gestisci, ottengono le autorizzazioni di gestione per il record.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Se un campo formula o un campo di ricerca di un record connesso è basato su un campo di un record per il quale non si dispone di autorizzazioni, verrà visualizzato il calcolo corretto per i fattori del record ai quali non è possibile accedere in altro modo.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Condividere le autorizzazioni dei record

In qualità di manager dell&#39;area di lavoro, è possibile modificare le autorizzazioni per singoli record.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera condividere i record.
1. Fare clic sul tipo di record di cui si desidera condividere i record.

1. Esegui una delle operazioni seguenti:

   * Nella vista tabella, passa il puntatore del mouse sul nome di un record e fai clic sul menu **Altro** ![Altro](assets/more-menu.png), quindi fai clic su **Condividi**.
   * Nella vista a tabella, seleziona un record, quindi fai clic su **Condividi** nella barra degli strumenti blu in fondo all&#39;elenco.
   * Da qualsiasi visualizzazione, fai clic sul nome di un record, quindi fai clic su **Condividi** nell&#39;angolo superiore destro della pagina dei dettagli del record.

   Viene visualizzata la casella **Condividi**.

   ![Autorizzazioni per i record con autorizzazioni ereditate su](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Facoltativo) Nell&#39;area **Chi ha accesso**, l&#39;opzione **Tutti nell&#39;area di lavoro possono visualizzare** è selezionata per impostazione predefinita.  Tutti gli utenti con autorizzazioni **View** o superiori per l&#39;area di lavoro e il tipo di record dispongono delle stesse autorizzazioni per il record.

1. (Facoltativo) Fai clic sul numero di utenti nell&#39;opzione **Autorizzazioni ereditate** per visualizzare utenti, team, gruppi, aziende o ruoli che ereditano le autorizzazioni dall&#39;area di lavoro.

   >[!TIP]
   >
   >Non è possibile rimuovere singole entità dall&#39;elenco Autorizzazioni ereditate.

1. (Facoltativo e condizionale) Se si desidera condividere il record con entità specifiche e concedere loro un accesso diverso al tipo di record rispetto a quello già disponibile per l&#39;area di lavoro, eseguire le operazioni seguenti:

   1. Seleziona **Disattiva** dal menu a discesa **Autorizzazioni ereditate**.

   >[!TIP]
   >
   >I manager di Workspace continuano a disporre delle autorizzazioni di gestione per il tipo di record e il record.

   1. (Facoltativo) Seleziona **Solo gli invitati possono accedere** dall&#39;area **Chi ha accesso**.

   1. Nel campo **Concedi l&#39;accesso a questo tipo di record**, aggiungi gli utenti, i team, i gruppi, le aziende o le mansioni a cui desideri concedere un livello di autorizzazione diverso da quello che hanno per l&#39;area di lavoro o il tipo di record.
   1. Scegliere uno dei seguenti livelli di autorizzazione:

      * Visualizzazione
      * Gestione

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Oltre a team, gruppi, aziende e ruoli, puoi condividere solo con gli utenti che sono stati aggiunti al Adobe Admin Console. Non è possibile aggiungere utenti solo Workfront. Per informazioni, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Se gli utenti dispongono delle autorizzazioni Contribute (Contribuisci) o Manage (Gestisci) per l&#39;area di lavoro e il tipo di record, manterranno le autorizzazioni Manage (Gestisci) per il record. L’autorizzazione Visualizzazione è disabilitata. <!--this is not dimmed at this time, Lilit to check-->
   >* Non potete concedere agli utenti un&#39;autorizzazione minore per il record se dispongono di Contribute o di una versione successiva per il tipo di record.
   > Per ulteriori informazioni, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Per consentire agli utenti che non dispongono delle autorizzazioni per l&#39;area di lavoro di visualizzare un record, nel campo **Concedi l&#39;accesso a questa visualizzazione**, inizia a digitare il nome di un utente, un gruppo, un team, una società o una mansione, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   L&#39;entità selezionata viene aggiunta al record, al tipo di record e all&#39;area di lavoro con autorizzazioni **Visualizza**.

   Gli amministratori di sistema ricevono sempre le autorizzazioni di gestione per i record condivisi con loro e vi è un&#39;indicazione che un utente è un amministratore di sistema.

1. (Facoltativo) Fai clic su **Copia collegamento** per copiare un collegamento al record negli Appunti e condividerlo con altri utenti. Il collegamento apre la pagina dei dettagli del record.
1. Fai clic su **Salva**.

   Il record è ora condiviso con altri utenti.

   Gli utenti con cui hai condiviso il record ricevono una notifica in-app e una notifica e-mail relativa alle autorizzazioni concesse alle seguenti entità:

   * Il record
   * Tipo di record, se non sono mai stati autorizzati in precedenza
   * L’area di lavoro, se non disponevano delle autorizzazioni necessarie prima che il record fosse condiviso con loro.

   Per informazioni, vedere [Notifiche di Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/notifications/notifications-information.md).

1. Condividi il collegamento copiato con altri utenti. Gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront per poter accedere alla pagina del tipo di record e visualizzarla nella visualizzazione selezionata. Per visualizzarlo, è necessario disporre delle autorizzazioni per il tipo di record. Per ulteriori informazioni, vedere anche [Condividere record utilizzando un collegamento](/help/quicksilver/planning/records/share-records.md).

## Rimuovere le autorizzazioni da un record

È possibile rimuovere le autorizzazioni degli utenti da un record. Tuttavia, manterranno almeno le autorizzazioni View (Visualizzazione) per l&#39;area di lavoro, che assegnano loro almeno le autorizzazioni View (Visualizzazione) per il tipo di record. È necessario rimuoverne l&#39;accesso dall&#39;area di lavoro se si desidera che non dispongano di autorizzazioni per i tipi di record o i record nell&#39;area di lavoro.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera interrompere la condivisione dei record, quindi fare clic su una scheda del tipo di record. Verrà aperta la pagina del tipo di record.
1. Esegui una delle operazioni seguenti:

   * Nella vista tabella, passa il puntatore del mouse sul nome di un record e fai clic sul menu **Altro** ![Altro](assets/more-menu.png), quindi fai clic su **Condividi**.
   * Nella vista a tabella, seleziona un record, quindi fai clic su **Condividi** nella barra degli strumenti blu in fondo all&#39;elenco.
   * Da qualsiasi visualizzazione, fai clic sul nome di un record, quindi fai clic su **Condividi** nell&#39;angolo superiore destro della pagina dei dettagli del record.

   Viene visualizzata la casella **Condividi**.
1. Individuare l&#39;utente, il gruppo, il team, la società o la mansione di cui si desidera rimuovere le autorizzazioni, espandere il menu a discesa delle autorizzazioni a destra del nome, quindi fare clic su **Rimuovi**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Rimuovi le autorizzazioni dal record](assets/remove-option-on-record-sharing-drop-down.png)

1. Fai clic su **Salva**.

   Gli utenti non dispongono più delle autorizzazioni indicate per il record. Tuttavia, dispongono ancora delle autorizzazioni per il tipo di record e l’area di lavoro, a meno che non vengano rimosse anche da tali autorizzazioni.

   Agli utenti che sono stati rimossi dall’accesso al record non viene notificato che non dispongono più di queste autorizzazioni.

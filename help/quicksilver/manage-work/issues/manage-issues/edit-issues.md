---
product-area: projects
navigation-topic: manage-issues
title: Modifica problemi
description: Puoi modificare le informazioni sui problemi che hai creato o che altri utenti hanno creato se hanno condiviso i problemi con te.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '2508'
ht-degree: 2%

---

# Modifica problemi

Puoi modificare le informazioni sui problemi che hai creato o che altri utenti hanno creato se hanno condiviso i problemi con te.

Puoi modificare un singolo problema oppure i problemi in un elenco. Per informazioni sulla modifica dei problemi in un elenco, vedi [Modifica problemi in un elenco](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> <p>Revisiona o ottieni la licenza per modificare i problemi nella sezione Problemi di un'attività o di un progetto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni sull&#39;accesso ai problemi nel tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l&#39;accesso ai problemi</a>. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per un problema che consente di modificare i campi seguenti nell’area Dettagli: </p>
   <ul>
   <li>Descrizione</li>
   <li>Stato</li>
   <li>Gravità</li>
   </ul>
   <p>Gestire le autorizzazioni per un problema per modificare tutti i campi nell’area Dettagli o nella casella Modifica problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Limitazioni durante la modifica dei problemi

Esistono alcune limitazioni che potrebbero impedire la modifica dei problemi.

* Non è possibile modificare i problemi che si trovano in un processo di approvazione. Puoi registrare solo l’ora o aggiornare lo stato solo per un problema in Attesa di approvazione.
* È possibile modificare e aggiungere documenti ai problemi di un progetto con stato Completato, Inattivo o In attesa di approvazione solo quando l&#39;amministratore di Workfront o un amministratore di gruppo ha abilitato questa funzionalità nell&#39;area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Modificare un singolo problema

È possibile modificare un problema utilizzando le aree Modifica problema o Dettagli problema. I passaggi seguenti descrivono come modificare un problema nella casella Modifica problema.

1. Passa al **menu principale**.
1. Fai clic su **Progetti**, quindi fai clic sul nome di un progetto per aprirlo.
1. (Facoltativo) Fai clic su **Attività**, quindi fai clic sul nome di un&#39;attività per aprirla.
1. Fai clic su **Problemi** nel pannello a sinistra.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Facoltativo) Per modificare informazioni limitate su un problema, fai clic su **Dettagli problema** nel pannello a sinistra.

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell’amministratore di Workfront o del gruppo, i campi nell’area Dettagli problema potrebbero essere ridisposti o non visualizzati. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per modificare le informazioni nella sezione Dettagli, effettuare le seguenti operazioni:

   1. (Facoltativo) Fai clic sull&#39;icona **Comprimi tutto** nell&#39;angolo superiore destro per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un&#39;area è compressa, fare clic sulla **freccia rivolta a destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l&#39;area che si desidera modificare.
   1. (Facoltativo) Per allegare un modulo personalizzato, inizia a digitare il nome di un modulo nel campo **Aggiungi modulo personalizzato**, quindi selezionalo quando viene visualizzato nell&#39;elenco, quindi fai clic su **Salva modifiche**.
   1. (Facoltativo) Fai clic sull&#39;icona **Esporta** ![](assets/export.png) per esportare le informazioni sulla panoramica e sui moduli personalizzati in un file PDF, quindi fai clic su **Esporta**. Selezionare una delle opzioni seguenti:

      * Seleziona tutto (viene visualizzato solo se è allegato almeno un modulo personalizzato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato nel computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Per ulteriori informazioni, vedere [Esportare moduli personalizzati e dettagli oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Per informazioni sui campi visibili nella sezione Dettagli problema, continua a modificare il problema nella casella Modifica problema come descritto di seguito.

1. Per modificare tutte le informazioni su un problema, seleziona un problema in un elenco, quindi fai clic su **Modifica** nella parte superiore dell&#39;elenco

   Oppure

   Fai clic sul nome di un problema in un elenco, quindi fai clic sul menu **Altro** accanto al nome del problema, quindi su **Modifica.**

   Viene visualizzata la finestra di dialogo **Modifica problema**.

   >[!IMPORTANT]
   >
   >Per visualizzare il collegamento Modifica, è necessario disporre delle autorizzazioni di gestione per il problema.

   Tutti i campi relativi ai problemi sono disponibili nella casella Modifica problema e sono raggruppati per le aree elencate nel pannello a sinistra.

1. Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [Nome Issue](#issue-name)
   * [Panoramica](#overview)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Impostazioni](#settings)

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront configura il modello di layout, i campi nella casella Modifica problema potrebbero essere diversi nel tuo ambiente. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >Quando crei un problema, la maggior parte dei campi elencati nelle sezioni seguenti è accessibile anche dalla casella Nuovo problema. Le sezioni in cui si trovano i campi non corrispondono alla casella Nuovo problema. Per informazioni sulla creazione dei problemi, vedi [Crea problemi](../../issues/manage-issues/create-issues.md).

### Nome Issue {#issue-name}

1. Inizia a modificare un problema come descritto in precedenza.
1. Fai clic su **Nome problema**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Aggiorna il campo **Nome problema**.
1. Fai clic su **Salva** o continua a modificare le sezioni seguenti.

### Panoramica {#overview}

1. Inizia a modificare un problema come descritto in precedenza.
1. Fare clic su **Panoramica**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Aggiornare o rivedere uno dei campi della tabella seguente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td> <p>Aggiungi ulteriori informazioni sul problema.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Sezione Informazioni di base</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td> <p>Seleziona lo stato del problema. Per ulteriori informazioni sugli stati dei problemi, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all'elenco degli stati dei problemi di sistema</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorità</td> 
      <td> <p>Questo è un flag visivo che ti consente di assegnare la priorità ai problemi.</p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p><strong>Nessuno</strong> </p> </li> 
        <li> <p><strong>Basso</strong> </p> </li> 
        <li> <p><strong>Normale</strong> </p> </li> 
        <li> <p><strong>Alta</strong> </p> </li> 
        <li> <p><strong>Urgente</strong> </p> </li> 
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall'amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per ulteriori informazioni sulla modifica delle priorità, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Creare e personalizzare le priorità</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravità</td> 
      <td> <p>Questo è un flag visivo che indica la gravità del problema descritto nel problema. Le gravità sono specifiche dei problemi. Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmetico</p> </li> 
        <li> <p style="font-weight: bold;">Causa Confusione</p> </li> 
        <li> <p style="font-weight: bold;">Bug con workaround</p> </li> 
        <li> <p style="font-weight: bold;">Bug senza workaround</p> </li> 
        <li> <p style="font-weight: bold;">Errore Fatale</p> </li> 
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall'amministratore di Workfront, i nomi delle gravità potrebbero essere diversi per te. Per ulteriori informazioni sulla modifica delle gravità, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Creare o personalizzare le gravità dei problemi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Digita un collegamento web relativo alle informazioni sul problema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td> <p>In base alle Proprietà coda selezionate dal project manager nell'area Dettagli coda del progetto, è possibile specificare il tipo di problema. Selezionare una delle opzioni seguenti nel menu a discesa <b>Tipo</b>: </p> 
       <ul> 
        <li> <p><strong>Segnalazione Bug</strong> </p> </li> 
        <li> <p><strong>Richiesta di Modifica</strong> </p> </li> 
        <li> <p><strong>Problema</strong> </p> </li> 
        <li> <p><strong>Richiesta</strong> </p> </li> 
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall’amministratore di Workfront, i nomi dei tipi di problemi potrebbero essere diversi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contatto principale</td> 
      <td>Per impostazione predefinita, il contatto principale è l’autore del problema. Per modificare questa impostazione, inizia a digitare il nome di qualsiasi utente attivo in Workfront, quindi selezionalo dall’elenco. Un problema può avere un solo contatto principale.<br> Se si modifica il contatto principale, il contatto principale originale dispone ancora dell'accesso di gestione al problema. È necessario rimuovere manualmente questo accesso dalla casella Issue Access (Accesso al problema) quando si condivide un problema.

   <b>SUGGERIMENTO</b>

   <p>Quando aggiungi un utente del contatto principale, osserva l’avatar, il ruolo principale dell’utente e il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.</p>
      <p> Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Concedere l'accesso agli utenti</a>.</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Conferma data e ora</td> 
      <td> <p>Questa è la data in cui l'assegnatario del problema stima che il problema sarà completato. Solo gli assegnatari possono modificare questo campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data Inizio Pianificata</td> 
      <td>Per impostazione predefinita, la Data inizio pianificata è la data e l’ora in cui è stato creato il problema. Puoi aggiornare la <strong>Data inizio pianificata</strong> del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di completamento pianificate</td> 
      <td> Per impostazione predefinita, la Data di completamento pianificata è 24 ore dalla Data di inizio pianificata predefinita. Per impostazione predefinita, i problemi hanno una durata di 1 giorno. Puoi aggiornare la <strong>Data di completamento pianificata</strong> del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio effettive</td> 
      <td>La data di inizio effettiva viene compilata automaticamente quando si cambia lo stato del problema in <strong>In corso</strong>. Puoi aggiornare la <strong>Data di inizio effettiva</strong> del problema. Se necessario, puoi aggiornare manualmente la data. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di completamento effettive</td> 
      <td>La data di completamento effettiva viene compilata automaticamente quando si cambia lo stato del problema in <strong>Chiuso</strong> o<strong>Risolto</strong>. Puoi aggiornare la <strong>Data di completamento effettiva</strong> per il problema. Se necessario, puoi aggiornare manualmente la data.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risoluzione di</td> 
      <td> <p>Questo mostra se il problema è risolto da un altro oggetto. Puoi scegliere se risolvere il problema con un’attività, un progetto o un altro problema dal menu a discesa, quindi inizia a digitare il nome dell’attività, del progetto o del problema che risolverà il problema. Selezionala quando viene visualizzata nell’elenco.</p>

   <b>NOTA</b>

   Quando si seleziona un oggetto per risolvere un problema, lo stato del problema viene collegato allo stato dell&#39;oggetto di risoluzione e non può essere modificato sul problema. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.

   <b>SUGGERIMENTO</b>

   Quando l’amministratore di sistema o di gruppo aggiunge il campo &quot;Risolto da&quot; a un’intestazione personalizzata di un problema, il campo cambia in &quot;Risolto un problema&quot;, &quot;Attività risolutiva&quot; o &quot;Progetto risolutivo&quot; se al problema è associato un oggetto di risoluzione.

   Non puoi modificare questo campo quando viene visualizzato nell’intestazione del problema. Per ulteriori informazioni sulla personalizzazione delle intestazioni dei problemi, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personalizzare le intestazioni degli oggetti utilizzando un modello di layout </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Risoluzione di un problema, attività risolutiva o progetto risolutivo</td> 
      <td>Il nome collegato del problema, dell’attività o del problema che risolve il problema.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Questo risolve</td> 
      <td>Il nome collegato del problema che viene completato quando viene risolto il problema a cui accedi.  </td> 
     </tr>


   </tbody> 
   </table>





1. Fai clic su **Salva** o continua a modificare le sezioni seguenti.

#### Assegnazioni {#assignments}

1. Inizia a modificare il problema come descritto in precedenza.
1. Fai clic su **Assegnazioni** nel pannello a sinistra.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Fai clic su **Cerca persone, mansione e team** e inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare all&#39;attività, quindi fai clic su di esso o premi Invio quando viene visualizzato nell&#39;elenco.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Se il nome dell&#39;utente contiene un carattere speciale, è necessario includere tale carattere nel campo di ricerca.

   >[!TIP]
   >
   >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
   >
   >
   >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >
   >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

1. (Facoltativo) Indica se un assegnatario è l&#39;assegnatario principale del problema, passando il puntatore del mouse sul nome dell&#39;assegnatario e facendo clic su **Rendi principale**. Un team non può essere l&#39;assegnatario principale di un problema.
1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lavoro Necessario</td> 
      <td> <p>Si tratta del tempo effettivo necessario agli assegnatari del problema per completarlo. Digita il numero di ore pianificate per il problema.<br></p> <p>Nota: la modifica delle ore pianificate del problema non modificherà la Data di completamento pianificata del problema. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Mansione dell'assegnatario</td> 
      <td> <p>Selezionare una mansione dal menu a discesa <strong>Ruolo dell'assegnatario</strong> quando si seleziona una persona come assegnatario. Questo è il ruolo che l’assegnatario può svolgere su questo problema. </p> <p><b>SUGGERIMENTO</b>

   Nel menu a discesa vengono visualizzati solo i ruoli associati a ciascun assegnatario nel relativo profilo.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** o continua a modificare le sezioni seguenti.

### Forms personalizzato

1. Inizia a modificare un problema come descritto in precedenza.
1. Fare clic su **Forms personalizzato**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. Nel campo **Aggiungi modulo personalizzato**, seleziona il modulo o i moduli personalizzati che desideri associare al problema. Devi creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Progettare un modulo con Progettazione moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). A un problema è possibile aggiungere fino a dieci moduli personalizzati.

1. (Condizionale) Se hai allegato un modulo personalizzato al problema, modifica tutti i campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare il problema.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront imposta le autorizzazioni per le sezioni nel modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni di cui disponi per il problema stesso. Per informazioni sull&#39;impostazione delle autorizzazioni per le sezioni di un modulo personalizzato, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Per informazioni sull&#39;impostazione delle autorizzazioni relative ai problemi, vedere [Condividere un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Fai clic su **Salva** o continua a modificare la sezione seguente.

### Impostazioni {#settings}

1. Inizia a modificare un problema come descritto in precedenza.
1. Fare clic su **Impostazioni**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Aggiorna le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td> 
       <div> 
       <p>Selezionare un processo di approvazione da associare al problema. Prima di poter associare i processi ai problemi, l'amministratore di Workfront deve definirli a livello di sistema. Gli utenti con accesso amministrativo ai processi di approvazione <span> possono inoltre creare processi di approvazione specifici per il gruppo.</span>Per ulteriori informazioni sulla creazione di processi di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creare un processo di approvazione per gli elementi di lavoro</a>. </p> 
       <p>Quando aggiungi processi di approvazione, tieni presente quanto segue: </p> 
       <ul> 
       <li>Nell'elenco vengono visualizzati solo i processi di approvazione attivi. </li> 
       <li> <p>I processi di approvazione a livello di sistema e di gruppo vengono visualizzati nell’elenco. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.</p> <p>Importante: se il gruppo del progetto cambia, il processo di approvazione specifico del gruppo diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati</a>. </p> </li> 
       <li> <p>È possibile definire processi di approvazione predefiniti da allegare automaticamente ai problemi durante la creazione di code di richieste o di argomenti della coda. Per informazioni sull'aggiornamento dei dettagli della coda, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richieste</a>. Per informazioni sulla creazione degli argomenti della coda, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Creare argomenti della coda</a>. </p> </li> 
       <li>Quando si verificano problemi di modifica in blocco, si verificano i seguenti scenari: 
       <ul> 
       <li><p>Quando selezioni più problemi dallo stesso gruppo, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli specifici del gruppo.</p></li> 
       <li><p>Quando si selezionano più problemi da gruppi diversi, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema.</p></li> 
       <li><p>Quando a uno dei problemi è associato un processo di approvazione a utente singolo, questo viene sostituito dal processo di approvazione a livello di sistema o di gruppo selezionato. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td> <p>Seleziona la casella di controllo per la quale desideri allegare gli Avvisi di Promemoria a questo problema. Vengono visualizzate tutte le notifiche di promemoria per i problemi. Prima di poter selezionare le notifiche di promemoria in un problema, l'amministratore di Workfront deve configurarle. Per ulteriori informazioni sulla configurazione delle notifiche di promemoria, vedere <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurare le notifiche di promemoria</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva.**

## Modificare un problema nell’intestazione del problema (limitato)

Puoi modificare una quantità limitata di informazioni nell’intestazione del problema.

L’amministratore di sistema o di gruppo può personalizzare i campi visualizzati nell’intestazione del problema. Per informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

I seguenti campi sono inclusi nell’intestazione del problema, per impostazione predefinita:

* Nome problema
* Percentuale completata
* Assegnazioni
* Data e ora di completamento pianificate
* Stato
* Prendere decisioni di approvazione se si è impostati come approvatore in un processo di approvazione corrente

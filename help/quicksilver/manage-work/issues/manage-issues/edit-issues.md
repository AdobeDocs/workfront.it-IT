---
product-area: projects
navigation-topic: manage-issues
title: Modifica dei problemi
description: Puoi modificare le informazioni sui problemi che hai creato o che altri utenti hanno creato se hanno condiviso con te i problemi.
author: Alina
feature: Work Management
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 3%

---

# Modifica dei problemi

Puoi modificare le informazioni sui problemi che hai creato o che altri utenti hanno creato se hanno condiviso con te i problemi.

È possibile modificare un singolo problema o un elenco. Per informazioni sulla modifica dei problemi in un elenco, vedi [Modificare i problemi in un elenco](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Requisiti di accesso

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
   <td> <p>Richiesta o superiore</p> <p>Rivedi o una licenza superiore per modificare i problemi nella sezione Problemi di un'attività o di un progetto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull&#39;accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute a un problema per modificarlo nell'area Dettagli problema </p> <p>Gestisci le autorizzazioni per un problema per modificarlo nella casella Modifica problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Limitazioni per la modifica dei problemi

Sono presenti alcune limitazioni che potrebbero impedire la modifica di problemi.

* Non è possibile modificare i problemi che si trovano in un processo di approvazione. È possibile registrare solo l&#39;ora o aggiornare lo stato di un problema in sospeso.
* È possibile modificare e aggiungere documenti ai problemi relativi a un progetto con stato Completato, Morto o In attesa di approvazione solo quando questa funzionalità è stata abilitata dall’amministratore di Workfront o da un amministratore di gruppo nell’area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Modificare un singolo problema

È possibile modificare un problema utilizzando le aree Modifica problema o Dettagli problema. I passaggi seguenti descrivono la modifica di un problema nella casella Modifica problema .

1. Vai a **Menu principale**.
1. Fai clic su **Progetti**, quindi fai clic sul nome di un progetto per aprire il progetto.
1. (Facoltativo) Fai clic su **Attività** , quindi fai clic sul nome di un’attività per aprirla.
1. Fai clic su **Problemi** nel pannello a sinistra.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Facoltativo) Per modificare informazioni limitate su un problema, fai clic su **Dettagli del problema** nel pannello a sinistra.

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront o di gruppo ha modificato il modello di layout, i campi nell’area Dettagli problema potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per modificare le informazioni nella sezione Dettagli, procedi come segue:

   1. (Facoltativo) Fai clic sul pulsante **Comprimi tutto** nell’angolo in alto a destra per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un’area viene compressa, fai clic sul pulsante **freccia verso destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l’area da modificare.
   1. (Facoltativo) Per allegare un modulo personalizzato, iniziare a digitare il nome di un modulo nel **Aggiungi modulo personalizzato** , quindi selezionalo quando viene visualizzato nell’elenco, quindi fai clic su **Salva modifiche**.
   1. (Facoltativo) Fai clic sul pulsante **Esporta** icona ![](assets/export.png) per esportare le informazioni generali e i moduli personalizzati in un file PDF, fai clic su **Esporta**. Seleziona una delle seguenti opzioni:

      * Seleziona tutto (viene visualizzato solo quando è presente almeno un modulo personalizzato allegato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato sul computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Per ulteriori informazioni, consulta [Esportare moduli personalizzati e dettagli dell’oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   Per informazioni sui campi visibili nella sezione Dettagli problema, continua a modificare il problema nella casella Modifica problema come descritto di seguito.

1. Per modificare tutte le informazioni su un problema, seleziona un problema in un elenco, quindi fai clic su **Modifica** in cima all&#39;elenco

   Oppure

   Fai clic sul nome di un problema in un elenco, quindi fai clic sul pulsante **Altro** accanto al nome del problema, quindi **Modifica.**

   La **Modifica problema** viene visualizzata la finestra di dialogo.

   >[!IMPORTANT]
   >
   >Per visualizzare il collegamento Modifica, devi disporre delle autorizzazioni di gestione per il problema.

   Tutti i campi dei problemi sono disponibili nella casella Modifica problema e sono raggruppati in base alle aree elencate nel pannello a sinistra.

1. È consigliabile specificare le informazioni in una delle sezioni seguenti:

   * [Nome Issue](#issue-name)
   * [Panoramica](#overview)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Impostazioni](#settings)

   >[!NOTE]
   >
   >A seconda della configurazione del modello di layout da parte dell’amministratore di Workfront, i campi nella casella Modifica problema potrebbero essere diversi nell’ambiente in uso. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome Issue {#issue-name}

1. Inizia a modificare un problema come descritto sopra.
1. Fai clic su **Nome problema**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Aggiorna **Nome problema** campo .
1. Fai clic su **Salva** oppure continua a modificare le sezioni seguenti.

### Panoramica {#overview}

1. Inizia a modificare un problema come descritto sopra.
1. Fai clic su **Panoramica**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Aggiorna o controlla uno dei campi nella tabella seguente:

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
      <td> <p>Seleziona lo stato del problema. Per ulteriori informazioni sugli stati dei problemi, vedi <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi del sistema</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorità</td> 
      <td> <p>Questo è un flag visivo che ti consente di assegnare priorità ai problemi.</p> <p>Seleziona tra le seguenti opzioni:</p> 
       <ul> 
        <li> <p><strong>Nessuno</strong> </p> </li> 
        <li> <p><strong>Basso</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>Alta</strong> </p> </li> 
        <li> <p><strong>Urgente</strong> </p> </li> 
       </ul> <p>A seconda delle preferenze del progetto selezionate dall’amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per ulteriori informazioni sulle priorità di modifica, vedi <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Creare e personalizzare le priorità</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravità</td> 
      <td> <p>Questo è un flag visivo per te che indica la gravità del problema descritto nel problema. I problemi sono specifici. Seleziona tra le seguenti opzioni:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmetico</p> </li> 
        <li> <p style="font-weight: bold;">Causa Confusione</p> </li> 
        <li> <p style="font-weight: bold;">Bug con workaround</p> </li> 
        <li> <p style="font-weight: bold;">Bug senza workaround</p> </li> 
        <li> <p style="font-weight: bold;">Errore Fatale</p> </li> 
       </ul> <p>A seconda delle preferenze del progetto selezionate dall’amministratore di Workfront, i nomi delle severità potrebbero essere diversi. Per ulteriori informazioni sulla modifica delle gravità, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Creare o personalizzare le gravità dei problemi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Digita un collegamento web relativo alle informazioni sul problema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td> <p>In base alle proprietà coda selezionate dal project manager nell'area Dettagli coda del progetto, è possibile specificare il tipo di problema. Seleziona tra le seguenti opzioni nel <b>Tipo</b> menu a discesa: </p> 
       <ul> 
        <li> <p><strong>Segnalazione Bug</strong> </p> </li> 
        <li> <p><strong>Richiesta di Modifica</strong> </p> </li> 
        <li> <p><strong>Problema</strong> </p> </li> 
        <li> <p><strong>Richiesta</strong> </p> </li> 
       </ul> <p>A seconda delle preferenze del progetto selezionate dall’amministratore di Workfront, i nomi dei tipi di problemi potrebbero essere diversi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contatto principale</td> 
      <td>Per impostazione predefinita, il contatto principale è il creatore del problema. Per modificare questa impostazione, inizia a digitare il nome di qualsiasi utente attivo in Workfront, quindi selezionalo dall’elenco. Un problema può avere un solo contatto primario.<br> Se si modifica il contatto primario, il contatto principale originale dispone ancora dell'accesso Gestisci al problema. Quando condividi un problema, devi rimuovere manualmente questo accesso dalla casella Accesso al problema.

   <b>SUGGERIMENTO</b>

   Quando aggiungi un utente di contatto primario, osserva l’avatar, il ruolo principale dell’utente e il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora dell’impegno</td> 
      <td> <p>Questa è la data in cui l’assegnatario del problema stima che il problema sarà completato. Solo gli assegnatari possono modificare questo campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data di inizio prevista</td> 
      <td>Per impostazione predefinita, la data di inizio pianificata è la data e l’ora in cui è stato creato il problema. È possibile aggiornare <strong>Data di inizio prevista</strong> del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora del completamento pianificati</td> 
      <td> Per impostazione predefinita, la data di completamento pianificata è 24 ore dalla data di inizio pianificata predefinita. Per impostazione predefinita, i problemi hanno una Durata di 1 giorno. È possibile aggiornare <strong>Data completamento pianificata</strong> del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio effettive</td> 
      <td>La data di inizio effettivo viene compilata automaticamente quando lo stato del problema viene modificato in <strong>In corso</strong>. È possibile aggiornare <strong>Data di inizio effettiva</strong> del problema. Se necessario, puoi aggiornare manualmente la data. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora del completamento effettivo</td> 
      <td>La data di completamento effettivo viene compilata automaticamente quando si modifica lo stato del problema in <strong>Chiuso</strong> o<strong>Risolto</strong>. È possibile aggiornare <strong>Data completamento effettivo</strong> per il problema. Se necessario, puoi aggiornare manualmente la data.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risoluzione di</td> 
      <td> <p>Questo indica se il problema è stato risolto da un altro oggetto. Puoi scegliere se questo problema è risolto da un'attività, un progetto o un altro problema dal menu a discesa, quindi iniziare a digitare il nome dell'attività, del progetto o del problema che risolverà il problema. Selezionalo quando viene visualizzato nell’elenco.</p>

   <b>NOTA</b>

   Quando si seleziona un oggetto per risolvere un problema, lo stato del problema è collegato allo stato dell&#39;oggetto di risoluzione e non può essere modificato sul problema. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.

   <b>SUGGERIMENTO</b>

   Quando l’amministratore di sistema o di gruppo aggiunge il campo &quot;Risolto da&quot; a un’intestazione personalizzata del problema, il campo diventa &quot;Risoluzione del problema&quot;, &quot;Risoluzione del problema&quot; o &quot;Risoluzione del progetto&quot; quando è presente un oggetto di risoluzione associato al problema.

   Non puoi modificare questo campo quando viene visualizzato nell’intestazione del problema. Per ulteriori informazioni sulla personalizzazione delle intestazioni dei problemi, vedi <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personalizzare le intestazioni degli oggetti utilizzando un modello di layout </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Risoluzione del problema, risoluzione dell'attività o risoluzione del progetto</td> 
      <td>Nome collegato del problema, dell'attività o del problema che risolve il problema.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Questo risolve</td> 
      <td>Il nome collegato del problema che viene completato quando il problema a cui stai accedendo viene risolto.  </td> 
     </tr>


   </tbody> 
   </table>





1. Fai clic su **Salva** oppure continua a modificare le sezioni seguenti.

#### Assegnazioni {#assignments}

1. Inizia a modificare il problema come descritto sopra.
1. Fai clic su **Assegnazioni** nel pannello a sinistra.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Fai clic su **Cercare persone, ruoli e team** e iniziare a digitare il nome di un utente, ruolo o team che si desidera assegnare all&#39;attività, quindi fare clic su di essa o premere Invio quando viene visualizzato nell&#39;elenco.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Se il nome dell’utente contiene un carattere speciale, è necessario includere il carattere speciale nel campo di ricerca.

   >[!TIP]
   >
   >È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
   >
   >
   >Se un utente, un ruolo o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
   >
   >* Riassegna l&#39;elemento di lavoro alle risorse attive.
   >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


1. (Facoltativo) Indicare se un assegnatario è il primo assegnatario sul problema, passando con il mouse sul nome dell&#39;assegnatario e facendo clic su **Rendi primario**. Un team non può essere l&#39;assegnatario principale di un problema.
1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lavoro Necessario</td> 
      <td> <p>Questo è il tempo effettivo necessario agli assegnatari del problema per completarlo. Digita il numero di ore pianificate per il problema.<br></p> <p>Nota: La modifica dell’ora pianificata del problema non modificherà il problema Data di completamento pianificata. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Mansione dell'assegnatario</td> 
      <td> <p>Seleziona un ruolo dal <strong>Ruolo dell'assegnatario</strong> menu a discesa quando hai selezionato una persona come assegnatario. Questo è il ruolo che l'assegnatario può svolgere su questo problema. </p> <p><b>SUGGERIMENTO</b>

   Nel menu a discesa vengono visualizzati solo i ruoli di lavoro associati a ciascun assegnatario nel proprio profilo.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** oppure continua a modificare le sezioni seguenti.

### Forms personalizzato

1. Inizia a modificare un problema come descritto sopra.
1. Fai clic su **Forms personalizzato**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. In **Aggiungi modulo personalizzato** selezionare il modulo o i moduli personalizzati che si desidera associare al problema. È necessario creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). È possibile aggiungere fino a dieci moduli personalizzati a un problema.

1. (Condizionale) Se hai allegato un modulo personalizzato al problema, modifica tutti i campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare il problema.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront ha impostato le autorizzazioni per le sezioni del modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni disponibili per il problema stesso. Per informazioni sull’impostazione delle autorizzazioni per le sezioni di un modulo personalizzato, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Per informazioni sull&#39;impostazione delle autorizzazioni per i problemi, vedi [Condividere un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Fai clic su **Salva** oppure continua a modificare la sezione seguente.

### Impostazioni {#settings}

1. Inizia a modificare un problema come descritto sopra.
1. Fai clic su **Impostazioni**.

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
       <p>Selezionare un processo di approvazione da associare al problema. Per poter essere associati a problemi, l’amministratore di Workfront deve definire i processi di approvazione a livello di sistema. Utenti con accesso amministrativo ai processi di approvazione <span> può anche creare processi di approvazione specifici per il gruppo.</span>Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creazione di un processo di approvazione per gli elementi di lavoro</a>. </p> 
       <p>Quando si aggiungono processi di approvazione, considera quanto segue: </p> 
       <ul> 
       <li>Nell’elenco vengono visualizzati solo i processi di approvazione attivi. </li> 
       <li> <p>Nell'elenco vengono visualizzati i processi di approvazione a livello di sistema e di gruppo. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.</p> <p>Importante: Se il gruppo del progetto viene modificato, il processo di approvazione specifico per gruppo diventa un processo di approvazione a uso singolo. Per ulteriori informazioni su come le modifiche apportate al gruppo del progetto o al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati</a>. </p> </li> 
       <li> <p>È possibile definire i processi di approvazione predefiniti da allegare automaticamente ai problemi durante la creazione di code di richiesta o argomenti di coda. Per informazioni sull'aggiornamento dei dettagli della coda, vedi <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>. Per informazioni sulla creazione degli argomenti della coda, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crea argomenti coda</a>. </p> </li> 
       <li>Quando si verificano problemi di modifica in serie, esistono i seguenti scenari: 
       <ul> 
       <li><p>Quando selezioni più problemi dallo stesso gruppo, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli specifici per gruppo.</p></li> 
       <li><p>Quando selezioni più problemi da gruppi diversi, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema.</p></li> 
       <li><p>Quando uno dei problemi presenta un processo di approvazione a uso singolo allegato, viene sostituito dal processo di approvazione a livello di sistema o di gruppo selezionato. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td> <p>Seleziona la casella di controllo per cui desideri allegare le notifiche dei promemoria a questo problema. Vengono visualizzate tutte le notifiche di promemoria relative ai problemi. L’amministratore di Workfront deve configurare le notifiche dei promemoria prima di poter selezionarle in caso di problemi. Per ulteriori informazioni sulla configurazione delle notifiche dei promemoria, vedi <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Impostare le notifiche dei promemoria</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva.**

## Modifica un problema nell&#39;intestazione del problema (limitato)

Puoi modificare una quantità limitata di informazioni nell’intestazione del problema.

L’amministratore di sistema o di gruppo può personalizzare i campi visualizzati nell’intestazione del problema. Per informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

Per impostazione predefinita, nell’intestazione del problema sono inclusi i seguenti campi:

* Nome problema
* Percentuale completata
* Assegnazioni
* Data e ora del completamento pianificati
* Stato
* Prendere decisioni di approvazione se si è impostati come approvatore in un processo di approvazione corrente

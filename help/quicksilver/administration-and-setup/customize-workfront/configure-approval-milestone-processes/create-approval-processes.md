---
title: Creazione di un processo di approvazione per gli elementi di lavoro
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: È possibile creare un processo di approvazione che gli utenti possono allegare a un elemento di lavoro (progetto, task, problema, modello o task modello), a un documento o a una bozza. Un processo di approvazione assicura che gli assegnatari designati sull'oggetto esaminino alcune modifiche prima che l'oggetto progredisca nel sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '2201'
ht-degree: 2%

---

# Creazione di un processo di approvazione per gli elementi di lavoro

È possibile creare un processo di approvazione che gli utenti possono allegare a un elemento di lavoro (progetto, task, problema, modello o task modello), a un documento o a una bozza. Un processo di approvazione assicura che gli assegnatari designati sull&#39;oggetto esaminino alcune modifiche prima che l&#39;oggetto progredisca nel sistema.

Questo articolo descrive come creare processi di approvazione globale a livello di sistema o di gruppo per gli elementi di lavoro (progetto, task, problema, modello o modello).

Per informazioni sulle approvazioni associate a documenti o bozze, vedere i seguenti articoli:

* [Richiedere l&#39;approvazione del documento](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Gli utenti possono inoltre creare un processo di approvazione a uso singolo per un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello in cui dispongono delle autorizzazioni di gestione.
>
>Questo articolo utilizza il termine &quot;processo di approvazione globale&quot; per differenziare dal processo di approvazione per uso singolo. È possibile utilizzare ripetutamente un processo di approvazione globale.
>
>A livello di gruppo, un processo di approvazione globale è limitato agli elementi di lavoro e agli stati appartenenti al gruppo.
>
>Per informazioni sui processi di approvazione a uso singolo, vedi [Panoramica del processo di approvazione](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) e [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Se sei un amministratore di Workfront o disponi di accesso amministrativo ai processi di approvazione, puoi creare un processo di approvazione a livello di sistema o un processo di approvazione a livello di gruppo per un determinato gruppo.</p> 
   <p>Gli amministratori di gruppo possono creare processi di approvazione a livello di gruppo per i gruppi gestiti.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un processo di approvazione globale a livello di sistema o di gruppo per gli elementi di lavoro

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. (Condizionale) Se si sta creando un processo di approvazione a livello di sistema, fare clic su **Processi** > **Approvazioni** nel pannello a sinistra.

   Oppure

   Se si sta creando un processo di approvazione a livello di gruppo, fare clic su **Gruppi** ![](assets/groups-icon.png), fai clic sul nome del gruppo, quindi fai clic su **Approvazioni**.

1. Fai clic sul pulsante **Approvazioni del progetto**, **Approvazioni attività** oppure **Approvazione del rilascio** a seconda del tipo di processo di approvazione che si desidera creare.

1. Fai clic su **Nuovo processo di approvazione**.
1. Nella casella visualizzata, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome processo di approvazione</td> 
      <td>Digitare un nome descrittivo per il processo di approvazione. Gli utenti visualizzano questo nome quando applicano il processo di approvazione a un oggetto, come descritto in <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associa un processo di approvazione nuovo o esistente al lavoro</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione del processo di approvazione. Viene visualizzato nel <b>Approvazioni</b> nella sezione <b>Configurazione</b> area accanto al nome del processo di approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>Mantieni questa opzione attivata se desideri che altri utenti possano allegare il processo di approvazione a progetti, attività e problemi creati. </p> <p>Questa opzione è attivata per impostazione predefinita.</p> <p> Contrassegnare un processo di approvazione come inattivo è utile quando l'organizzazione non deve più utilizzarlo, ma si desidera conservare le informazioni cronologiche relative al suo utilizzo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Questa approvazione è utilizzabile da </td> 
      <td> <p>Se si desidera che il processo di approvazione sia disponibile per progetti, attività, problemi e modelli appartenenti solo a un gruppo specifico, iniziare a digitare il nome del gruppo, quindi selezionare il nome quando viene visualizzato:</p> 
       <ul> 
       <li>Se si è un amministratore di sistema o si dispone dell'accesso amministrativo ai processi di approvazione, è possibile visualizzare qualsiasi gruppo nel sistema quando si digita il nome. <b>Tutti i gruppi</b> è selezionato per impostazione predefinita. </li> 
       <li>Se si è un amministratore di gruppo senza accesso amministrativo ai processi di approvazione, è possibile assegnare il processo di approvazione a qualsiasi gruppo gestito quando si digita il nome. La <b>Tutti i gruppi</b> opzione non disponibile.</li> 
       </ul> 
       <p>Questa opzione non è disponibile per i processi di approvazione a uso singolo.</p> 
       <p><b>AVVISO</b>: Quando si apportano modifiche al processo di approvazione specifico per gruppo, è possibile che vengano modificati i processi di approvazione esistenti già associati agli elementi di lavoro. Per informazioni su queste modifiche, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati</a>.</p> 
       <p>Per informazioni sull'elenco e sulla gestione dei processi di approvazione del gruppo dalla pagina del gruppo, consulta <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processi di approvazione a livello di gruppo</a>. </p> 
       <p>Per informazioni sull'accesso amministrativo ai processi di approvazione, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configura un percorso per il processo di approvazione utilizzando le opzioni seguenti.

   Un percorso è il percorso in cui specificare cosa deve accadere nel processo di approvazione. Si creano le fasi in un percorso per indicare chi deve eseguire il lavoro di approvazione e in quale ordine.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Avvia il processo di approvazione quando lo stato è impostato su</p> </td> 
      <td> <p>Selezionare lo stato che attiverà il processo di approvazione per gli elementi di lavoro. Quando un utente aggiorna un elemento di lavoro a questo stato, inizia il processo di approvazione. </p> <p>Impossibile selezionare lo stesso stato per più percorsi del processo di approvazione.</p> <p>Gli stati disponibili si basano su quelli selezionati nell’opzione . <b>Questa approvazione può essere utilizzata da</b> (spiegato nella tabella precedente):</p> 
       <ul> 
       <li> Se <b>Tutti i gruppi</b> è selezionato, sono disponibili solo gli stati a livello di sistema
       <li> <p>Se è selezionato un gruppo specifico, sono disponibili solo gli stati disponibili per tale gruppo</p> </li> 
       </ul> <p>Per informazioni sul funzionamento del processo di approvazione con gli stati, consulta la sezione . <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Come i processi di approvazione si basano sugli stati</a> nell'articolo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome fase</td> 
      <td>(Facoltativo) Digita un nome che descrive il primo passaggio del percorso. Se non si specifica un nome di area di visualizzazione, il nome predefinito è <b>Fase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approvatori</td> 
      <td> <p>Inizia a digitare il nome dell’utente, del team o del ruolo di lavoro che desideri designare come approvatore per questa fase, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa. Puoi aggiungere solo gli utenti attivi, <span>ruoli</span>e i team. </p>

   <p><b>SUGGERIMENTO</b>:</p>

   <p>Quando aggiungi un utente come approvatore, osserva l’avatar, il ruolo principale dell’utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l'aggiunta.</p>

   <p><b>NOTA</b>:

   L&#39;aggiunta di un utente, un team o un ruolo come approvatore non concede automaticamente le autorizzazioni all&#39;oggetto associato a tale approvazione. Essi ricevono le autorizzazioni per l&#39;oggetto quando viene attivato il passaggio di approvazione. In caso contrario, gli oggetti devono essere condivisi con loro prima di poter prendere una decisione di approvazione. </p> <p>Puoi anche designare una persona come approvatore specificando il ruolo della persona. Ad esempio, è possibile assegnare come approvatore un Proprietario progetto, Sponsor progetto, Proprietario Portfolio, Proprietario programma o Manager. Queste opzioni vengono visualizzate automaticamente all&#39;inizio della digitazione.</p>

   <p><b>IMPORTANTE</b>:  
       <ul> 
       <li> <p>Quando si assegna un'approvazione allo sponsor del progetto e nessuno viene designato come sponsor di un progetto, l'approvazione viene riassegnata al proprietario del progetto. Se nessuno è designato come proprietario del progetto, l’approvazione viene assegnata all’amministratore Workfront. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Quando assegni un'approvazione a un ruolo e <b>L’approvatore non deve far parte del team di progetto (per i processi di approvazione che includono un ruolo)</b> è disattivato ma non sono presenti ruoli nel team di progetto che corrispondono al ruolo nell’approvazione, l’approvazione viene riassegnata al proprietario del progetto. Per informazioni sulle impostazioni di approvazione, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Quando si assegna un'approvazione al proprietario del progetto e nessuno viene designato come proprietario di un progetto, l'approvazione viene riassegnata all'amministratore principale di Workfront come indicato nella sezione Informazioni cliente nell'area Configurazione. Per informazioni, consulta <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurare le informazioni di base per il sistema</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>È possibile ripetere questo processo per aggiungere più approvatori all'area di visualizzazione. Una singola fase può includere una combinazione di utenti, team e ruoli di lavoro come approvatori. Non esiste alcun limite al numero di approvatori che è possibile aggiungere a un passaggio.</p> <p><b>IMPORTANTE</b>:  <p>Quando si assegnano ruoli di lavoro come approvatori, tutti gli utenti associati a tale ruolo di lavoro che fanno parte anche del team di progetto possono decidere in merito all'approvazione. </p> <p>Quando assegni un team come approvatore, qualsiasi utente del team può prendere una decisione sull'approvazione. </p> <p>Per ulteriori informazioni sul team di progetto, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team di progetto</a>. Per ulteriori informazioni sull'approvazione del lavoro, vedi <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approvazione del lavoro </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">È necessaria solo una decisione</td> 
      <td> <p>(Visualizza solo se si aggiungono più approvatori all'area di visualizzazione) Selezionare questa opzione se uno degli approvatori sullo stadio può approvare o rifiutare l'elemento di lavoro durante questa fase. Questa azione consente all’elemento di lavoro di uscire dall’area di visualizzazione. </p> <p>Se questa opzione non è selezionata, tutti gli approvatori identificati devono approvare o rifiutare lo stadio (in qualsiasi ordine) prima che l'articolo lasci lo stadio. Se uno degli approvatori rifiuta la fase, il processo interrompe e inizia di nuovo in modo da poter apportare le modifiche necessarie. Gli approvatori possono quindi approvare o rifiutare nuovamente lo stadio.</p> <p>Quando un team viene designato come approvatore, qualsiasi membro del team può concedere o rifiutare una fase.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Aggiungi fase</p> </td> 
      <td>(Facoltativo) Aggiungi un altro passaggio al percorso, utilizzando le opzioni illustrate nelle tre righe precedenti. Puoi aggiungere al percorso tutti gli stadi necessari.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scegli cosa succede quando l’approvazione viene rifiutata</p> </td> 
      <td> <p>Selezionare l'azione da eseguire se l'elemento di lavoro viene rifiutato in una qualsiasi fase del percorso:</p> 
       <ul> 
       <li><b>Creare un problema</b>: (Disponibile solo per i processi di approvazione di progetti e task) Viene creato un problema nel progetto o nell'attività in cui è in esecuzione il processo di approvazione. Al problema viene assegnata la risorsa assegnata predefinita sull'attività o il proprietario del progetto. Per impostazione predefinita, il nome del problema creato è <b>Approvazione rifiutata (&lt;project or="" task="" name=""&gt;)</b>. Si tratta di un problema di rifiuto, inserito nell'attività o nel progetto, a seconda del processo di approvazione in cui si è verificato il rifiuto.</li> 
       <li> <p><b>Imposta stato su</b>: Scegliere una delle seguenti opzioni:</p> 
       <ul> 
       <li><b>Stato precedente</b>: Il progetto, l'attività o il problema rifiutati viene ripristinato allo stato precedente allo stato che attiva il processo di approvazione.</li> 
       <li><p><b>Qualsiasi altro stato dell’elenco</b>: L'oggetto rifiutato si sposta sullo stato scelto, ad esempio Bloccato. È possibile scegliere uno degli stati predefiniti o uno stato personalizzato aggiunto al sistema Workfront.</p>
       <p>Se si seleziona uno stato associato a un processo di approvazione come stato di rifiuto, l'oggetto rifiutato si sposta sullo stato selezionato e verrà contrassegnato come "Approvazione in sospeso".</p> 
       <p> Ad esempio, se si seleziona Bloccato per lo stato di rifiuto e lo stato Bloccato è associato a un processo di approvazione, l'oggetto rifiutato viene posizionato nello stato di "In attesa - In attesa di approvazione", che richiede l'approvazione.</p>

   </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic su **Aggiungi percorso** per aggiungere un altro percorso al processo di approvazione, facendo riferimento all&#39;elenco delle opzioni del passaggio precedente.

   Il nuovo percorso deve essere associato a un altro stato. Il percorso si attiva quando l&#39;elemento viene aggiornato per mostrare questo stato. Non puoi avere due percorsi per lo stesso stato.

1. Fai clic su **Salva**.
1. Una volta creato il processo di approvazione, continua con uno dei seguenti elementi:

   * Associa il processo di approvazione a progetti, attività o problemi specifici in tutto il sistema, come descritto in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Al di fuori di Workfront, notifica agli utenti che il processo di approvazione è disponibile per essere associati ai loro progetti, attività o problemi, come descritto in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Crea un altro processo di approvazione che viene attivato se questo processo di approvazione viene rifiutato e l&#39;elemento assume un altro stato. Questo consente di collegare insieme i processi di approvazione.

Per informazioni sulla modifica di un processo di approvazione, consulta [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Associazione di un processo di approvazione a un elemento di lavoro

Quando si desidera creare un processo di approvazione per un elemento di lavoro (progetto, attività o problema), creare prima il processo di approvazione, quindi creare l&#39;elemento di lavoro e quindi associare il processo di approvazione all&#39;elemento di lavoro.

Per istruzioni sull&#39;associazione di un processo di approvazione a un elemento di lavoro, vedere [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Qualsiasi utente Workfront con autorizzazioni di gestione per un progetto, un&#39;attività o un problema può creare processi di approvazione a uso singolo da utilizzare solo sull&#39;oggetto in cui sono stati creati. Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Consentire agli utenti di modificare i processi di approvazione globale per un singolo elemento di lavoro

Per impostazione predefinita, gli utenti che dispongono di autorizzazioni di gestione per progetti, attività e problemi possono creare processi di approvazione a uso singolo. Per informazioni sull’aggiunta di processi di approvazione a uso singolo a progetti, attività e problemi, consulta la sezione . [Associa un processo di approvazione a uso singolo a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) nell&#39;articolo [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Gli utenti possono inoltre modificare le impostazioni di un processo di approvazione globale associato a un elemento di lavoro. Queste modifiche interessano solo il progetto, l&#39;attività o il problema associato al processo di approvazione a livello di sistema. Per ulteriori informazioni, consulta la sezione . [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) nell&#39;articolo [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).

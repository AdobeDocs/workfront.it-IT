---
title: Creare un processo di approvazione per gli elementi di lavoro
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: È possibile creare un processo di approvazione che gli utenti possono allegare a un elemento di lavoro (progetto, attività, problema, modello o attività modello), a un documento o a una bozza. Un processo di approvazione garantisce che gli assegnatari designati dell'oggetto rivedano alcune modifiche prima che l'oggetto progredisca nel sistema.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2193'
ht-degree: 1%

---

# Creare un processo di approvazione per gli elementi di lavoro

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

È possibile creare un processo di approvazione che gli utenti possono allegare a un elemento di lavoro (progetto, attività, problema, modello o attività modello), a un documento o a una bozza. Un processo di approvazione garantisce che gli assegnatari designati dell&#39;oggetto rivedano alcune modifiche prima che l&#39;oggetto progredisca nel sistema.

Questo articolo descrive come creare processi di approvazione globali a livello di sistema o di gruppo per gli elementi di lavoro (progetto, attività, problema, modello o attività modello).

Per informazioni sulle approvazioni associate a documenti o bozze, vedi i seguenti articoli:

* [Richiedi approvazioni documenti](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Gli utenti possono anche creare un processo di approvazione a utente singolo per un progetto, un’attività, un problema, un modello o un’attività modello per cui dispongono delle autorizzazioni di gestione.
>
>In questo articolo viene utilizzato il termine &quot;processo di approvazione globale&quot; per differenziare il processo di approvazione da quello a uso singolo. Un processo di approvazione globale può essere utilizzato ripetutamente.
>
>A livello di gruppo, un processo di approvazione globale è limitato agli elementi di lavoro e agli stati che appartengono al gruppo.
>
>Per informazioni sui processi di approvazione a utente singolo, vedere [Panoramica del processo di approvazione](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) e [Associare un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Processo di approvazione a livello di sistema o a utente singolo: qualsiasi</p>
   <p>Processo di approvazione a livello di gruppo: Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard </p>
 <p>oppure</p> 
<p>Corrente: Piano </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Se si è un amministratore di sistema o si dispone dell'accesso amministrativo ai processi di approvazione, è possibile creare un processo di approvazione a livello di sistema o un processo di approvazione a livello di gruppo per un determinato gruppo.</p> 
   <p>Gli amministratori di gruppi possono creare processi di approvazione a livello di gruppo per i gruppi gestiti.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un processo di approvazione globale a livello di sistema o di gruppo per gli elementi di lavoro

{{step-1-to-setup}}

1. (Condizionale) Se stai creando un processo di approvazione a livello di sistema, fai clic su **Processi** > **Approvazioni** nel pannello a sinistra.

   Oppure

   Se stai creando un processo di approvazione a livello di gruppo, fai clic su **Gruppi** ![Icona Gruppi](assets/groups-icon.png), fai clic sul nome del gruppo, quindi su **Approvazioni**.

   <!--hidden for the new tab redesign - August 2023: 
   ![Approvals area in setup](assets/approvals-area-in-setup-processes.png)
   -->

1. Scegliere la scheda **Approvazioni progetti**, **Approvazioni attività** o **Approvazioni problemi**.

1. Fare clic su **Nuovo processo di approvazione**.
1. Specifica le seguenti informazioni nella casella visualizzata:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome processo di approvazione</td> 
      <td><p>Digitare un nome descrittivo per il processo di approvazione. Gli utenti visualizzano questo nome quando applicano il processo di approvazione a un oggetto, come descritto in <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associare un processo di approvazione nuovo o esistente a un lavoro</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td><p>Digitare una descrizione del processo di approvazione. Verrà visualizzato nella sezione <b>Approvazioni</b> nell'area <b>Configurazione</b> accanto al nome del processo di approvazione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>Mantieni questa opzione attivata se desideri che altri utenti possano allegare il processo di approvazione ai progetti, alle attività e ai problemi creati. </p> <p>Questa opzione è attivata per impostazione predefinita.</p> <p> Suggerimento: contrassegnare un processo di approvazione come inattivo è utile quando l’organizzazione non deve più utilizzarlo, ma desideri conservare le informazioni storiche sul suo utilizzo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Questa approvazione è utilizzabile da </td> 
      <td> <p>Se desideri che il processo di approvazione sia disponibile per progetti, attività, problemi e modelli appartenenti solo a un determinato gruppo, inizia a digitare il nome del gruppo, quindi, quando viene visualizzato, seleziona il nome:</p> 
       <ul> 
       <li>Se si è un amministratore di sistema o si dispone dell'accesso amministrativo ai processi di approvazione, è possibile visualizzare qualsiasi gruppo del sistema quando si digita il relativo nome. <b>Tutti i gruppi</b> sono selezionati per impostazione predefinita. </li> 
       <li>Se si è un amministratore di gruppo senza accesso amministrativo ai processi di approvazione, è possibile assegnare il processo di approvazione a qualsiasi gruppo gestito quando si digita il relativo nome. Opzione <b>Tutti i gruppi</b> non disponibile.</li> 
       </ul> 
       <p>Questa opzione non è disponibile per i processi di approvazione a utente singolo.</p> 
       <p><b>AVVISO</b>: quando si apportano modifiche al processo di approvazione specifico del gruppo, i processi di approvazione esistenti già associati agli elementi di lavoro potrebbero cambiare. Per informazioni su queste modifiche, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati</a>.</p> 
       <p>Per informazioni sull'elenco e sulla gestione dei processi di approvazione del gruppo dalla pagina del gruppo, vedere <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processi di approvazione a livello di gruppo</a>. </p> 
       <p>Per informazioni sull'accesso amministrativo ai processi di approvazione, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configura un percorso per il processo di approvazione utilizzando le opzioni seguenti.

   Un percorso è quello in cui si specifica cosa deve accadere nel processo di approvazione. Puoi creare delle fasi in un percorso per indicare chi deve eseguire il lavoro di approvazione e in quale ordine.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Avvia il processo di approvazione quando lo stato è impostato su</p> </td> 
      <td> <p>Selezionare lo stato che attiverà il processo di approvazione sugli elementi di lavoro. Quando un utente aggiorna un elemento di lavoro con questo stato, inizia il relativo processo di approvazione. </p> <p>Impossibile selezionare lo stesso stato per più percorsi del processo di approvazione.</p> <p>Gli stati disponibili si basano su quanto selezionato nell'opzione <b>Questa approvazione può essere utilizzata da</b> (illustrato nella tabella precedente):</p> 
       <ul> 
       <li> Se è selezionato <b>Tutti i gruppi</b>, sono disponibili solo gli stati a livello di sistema
       <li> <p>Se è selezionato un gruppo specifico, sono disponibili solo gli stati disponibili per tale gruppo</p> </li> 
       </ul> <p>Per informazioni sul funzionamento del processo di approvazione con gli stati, vedere la sezione <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Utilizzo degli stati nei processi di approvazione</a> nell'articolo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome fase</td> 
      <td>(Facoltativo) Digitate un nome che descriva la prima fase del percorso. Se non si specifica un nome di fase, il nome predefinito è <b>Fase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approvatori</td> 
      <td> <p>Iniziare a digitare il nome dell'utente, del team o della mansione che si desidera designare come approvatore per questa fase, quindi fare clic sul nome quando viene visualizzato nell'elenco a discesa. È possibile aggiungere solo utenti attivi, <span>mansioni</span> e team. </p>

   <p><b>SUGGERIMENTO</b>:</p>

   <p>Quando aggiungi un utente come approvatore, osserva l’avatar, il Ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.</p>
      <p>Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Concedere l'accesso agli utenti</a>. </p>

   <p><b>NOTA</b>:

   L&#39;aggiunta di un utente, un team o un ruolo come approvatore non concede automaticamente le autorizzazioni per l&#39;oggetto associato a tale approvazione. Ricevono le autorizzazioni per l’oggetto quando viene attivato il passaggio di approvazione. In caso contrario, gli oggetti devono essere condivisi con loro prima di poter prendere una decisione di approvazione. </p> <p>È inoltre possibile designare una persona come approvatore specificandone il ruolo. È ad esempio possibile assegnare un Proprietario progetto, uno Sponsor progetto, un Proprietario Portfolio, un Proprietario programma o un Manager come approvatore. Queste opzioni vengono visualizzate automaticamente quando si inizia a digitare.</p>

   <p><b>IMPORTANTE</b>:  
       <ul> 
       <li> <p>Quando si assegna un'approvazione allo sponsor del progetto e nessuno viene designato come sponsor di un progetto, l'approvazione viene riassegnata al proprietario del progetto. Se nessuno è designato come proprietario del progetto, l’approvazione viene assegnata all’amministratore di Workfront. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Quando si assegna un'approvazione a una mansione e l'<b>Approvatore non deve necessariamente essere nel team di progetto (per i processi di approvazione che includono una mansione)</b> è disabilitato ma non vi sono ruoli nel team di progetto che corrispondono al ruolo nell'approvazione, l'approvazione viene riassegnata al proprietario del progetto. Per informazioni sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurare le impostazioni di approvazione globali</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Quando si assegna un'approvazione al proprietario del progetto e nessuno viene designato come proprietario di un progetto, l'approvazione viene riassegnata all'amministratore principale di Workfront come indicato nella sezione Informazioni cliente nell'area Configura. Per informazioni, vedere <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurare le informazioni di base per il sistema</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>È possibile ripetere questo processo per aggiungere più approvatori all'area di visualizzazione. Una singola fase può includere una combinazione di utenti, team e ruoli come approvatori. Non esiste alcun limite al numero di approvatori che è possibile aggiungere a una fase.</p> <p><b>IMPORTANTE</b>:  <p>Quando si assegnano mansioni come approvatori, tutti gli utenti associati a tale mansione che sono anche nel team del progetto possono prendere una decisione sull'approvazione. </p> <p>Quando si assegna un team come approvatore, qualsiasi utente del team può prendere una decisione in merito all'approvazione. </p> <p>Per ulteriori informazioni sul team di progetto, vedere <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica team di progetto</a>. Per ulteriori informazioni sull'approvazione del lavoro, vedere <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approvazione del lavoro </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">È necessaria una sola decisione <br> <br> (viene visualizzata solo se si aggiungono più approvatori alla fase) </td> 
      <td> <p>Selezionare questa opzione se uno qualsiasi degli approvatori sullo stage può approvare o rifiutare l'elemento di lavoro durante questa fase. Questa azione consente all'elemento di lavoro di uscire dall'area di visualizzazione. </p> <p>Se questa opzione non è selezionata, tutti gli approvatori identificati devono approvare o rifiutare lo stadio (in qualsiasi ordine) prima che l'elemento lasci lo stadio. Se uno qualsiasi degli approvatori rifiuta la fase, il processo si interrompe e ricomincia in modo da poter apportare le modifiche necessarie. Quindi gli approvatori possono approvare o rifiutare di nuovo la fase.</p> <p>Quando un team viene designato come approvatore, qualsiasi membro del team può concedere o rifiutare una fase.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Aggiungi fase</p> </td> 
      <td><p>(Facoltativo) Aggiungete un'altra fase al percorso, utilizzando le opzioni descritte nelle tre righe precedenti. Potete aggiungere al percorso tutte le fasi necessarie.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scegli cosa accade quando l'approvazione viene rifiutata</p> </td> 
      <td> <p>Selezionare l'azione che si desidera eseguire se l'elemento di lavoro viene rifiutato in una qualsiasi fase del percorso:</p> 
       <ul> 
       <li><b>Crea un problema</b>: (disponibile solo per i processi di approvazione del progetto e dell'attività) viene creato un problema nel progetto o nell'attività in cui è in esecuzione il processo di approvazione. La risorsa assegnata predefinita all'attività, o il proprietario del progetto, è assegnato al problema. Per impostazione predefinita, il nome del problema creato è <b>Approvazione rifiutata (&lt;Nome progetto o attività&gt;)</b>. Si tratta di un problema di rifiuto, immesso sotto l’attività o il progetto, a seconda del processo di approvazione in cui si è verificato il rifiuto.</li> 
       <li> <p><b>Imposta stato su</b>: scegliere una delle opzioni seguenti:</p> 
       <ul> 
       <li><b>Stato precedente</b>: il progetto, l'attività o il problema rifiutato torna allo stato precedente allo stato che attiva il processo di approvazione.</li> 
       <li><p><b>Qualsiasi altro stato nell'elenco</b>: l'oggetto rifiutato passa allo stato scelto, ad esempio In sospeso. È possibile scegliere uno degli stati predefiniti o uno degli stati personalizzati aggiunti al sistema Workfront.</p>
       <p>Se si seleziona uno stato associato a un processo di approvazione come stato di rifiuto, l'oggetto rifiutato si sposta sullo stato selezionato e verrà contrassegnato come "In attesa di approvazione".</p> 
       <p> Ad esempio, selezionando In sospeso con lo stato In sospeso associato a un processo di approvazione, l'oggetto rifiutato passa allo stato "In sospeso - In attesa di approvazione" e richiede l'approvazione.</p>

   </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic su **Aggiungi percorso** per aggiungere un altro percorso al processo di approvazione, facendo riferimento all&#39;elenco di opzioni del passaggio precedente.

   Il nuovo percorso deve essere associato a un altro stato. Il percorso viene attivato quando l’elemento viene aggiornato per mostrare questo stato. Non è possibile avere due percorsi per lo stesso stato.

1. Fai clic su **Salva**.
1. Dopo aver creato il processo di approvazione, continuare con una delle operazioni seguenti:

   * Associa il processo di approvazione a progetti, attività o problemi specifici in tutto il sistema, come descritto in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Al di fuori di Workfront, avvisa gli utenti che il processo di approvazione è disponibile per l&#39;associazione ai loro progetti, attività o problemi, come descritto in [Associa un processo di approvazione nuovo o esistente a lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Crea un altro processo di approvazione che viene attivato se questo processo di approvazione viene rifiutato e l&#39;articolo assume un altro stato. In questo modo è possibile collegare tra loro i processi di approvazione.

Per informazioni sulla modifica di un processo di approvazione, vedere [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Associazione di un processo di approvazione a un elemento di lavoro

Quando si desidera creare un processo di approvazione per un elemento di lavoro (progetto, attività o problema), è necessario

1. Crea prima il processo di approvazione
1. Creare l’elemento di lavoro
1. Associa il processo di approvazione all&#39;elemento di lavoro

Per istruzioni sull&#39;associazione di un processo di approvazione a un elemento di lavoro, vedere [Associare un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Qualsiasi utente di Workfront con autorizzazioni di gestione per un progetto, un’attività o un problema può creare processi di approvazione a utente singolo da utilizzare solo sull’oggetto in cui viene creato. Per ulteriori informazioni, vedere [Associa un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Consentire agli utenti di modificare i processi di approvazione globali per un singolo elemento di lavoro

Per impostazione predefinita, gli utenti che hanno autorizzazioni di gestione su progetti, attività e problemi possono creare processi di approvazione per singolo utilizzo. Per informazioni sull&#39;aggiunta di processi di approvazione a utente singolo a progetti, attività e problemi, vedere la sezione [Associare un processo di approvazione a utente singolo a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) nell&#39;articolo [Associare un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Gli utenti possono inoltre modificare le impostazioni di un processo di approvazione globale associato a un elemento di lavoro. Queste modifiche interessano solo il progetto, l&#39;attività o il problema associato al processo di approvazione a livello di sistema. Per ulteriori informazioni, vedere la sezione [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) nell&#39;articolo [Associare un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).

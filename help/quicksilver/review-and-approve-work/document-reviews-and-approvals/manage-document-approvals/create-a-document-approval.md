---
product-area: documents
navigation-topic: approvals
title: Creare un flusso di lavoro di approvazione documento
description: Puoi richiedere l’approvazione di altri utenti per un documento in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 2231
ht-degree: 2%

---

# Creare un flusso di lavoro di approvazione documento

Puoi richiedere l’approvazione di un documento in Adobe Workfront ad altri utenti o team, oppure chiedere loro di rivedere un documento senza doverlo approvare.

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedere gli articoli elencati in [Approvazioni di lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td>  
   <td>
   <p>Collaboratore o successiva</p>
   <p>Revisione o successiva</p>
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard e calendari, documenti</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

## Create an approval workflow in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)

-->

## Creare un flusso di lavoro di approvazione nell’area documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

### Creare un flusso di lavoro di approvazione di base

Per creare un flusso di lavoro di approvazione in una sola fase:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Selezionare la versione del documento per cui si desidera creare un&#39;approvazione nel menu a discesa versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Compila i seguenti dettagli:

   <table>
   <tr>
   <td><strong>Utilizzare un modello di approvazione (facoltativo)</strong></td>
   <td>Seleziona un modello dal menu a discesa. Se il modello ha un percorso e una fase, viene applicato in modalità Base. Se il modello ha più di una fase o più percorsi, la finestra di dialogo passa automaticamente alla modalità Avanzata e qualsiasi input immesso in modalità Base viene sostituito dal contenuto del modello.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.</td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (facoltativo)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Scadenza il (facoltativo)</strong></td>
   <td>Imposta una data di scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della data di scadenza specificata.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi messaggio personalizzato (facoltativo)</strong></td>
   <td>Digitare un messaggio nella casella di testo <strong>Aggiungi messaggio personalizzato</strong>. Il messaggio viene visualizzato nella notifica e-mail di approvazione e nella scheda Approvazioni in Workfront.
   <p>Nota: se modifichi un messaggio personalizzato dopo la creazione del flusso di lavoro di approvazione, a tutti i partecipanti esistenti viene inviata una notifica e-mail aggiornata. Se aggiungi un partecipante in un secondo momento, il messaggio personalizzato viene incluso nella notifica e-mail.</p>
   </td>
   </tr>
   </table>

1. Fai clic su **Richiedi approvazione**.

   ![Richiedi l&#39;approvazione in modalità elementare](assets/request-approval-basic.jpeg)

### Creare un flusso di lavoro di approvazione avanzato

La modalità avanzata supporta più stadi e percorsi paralleli. Ogni percorso viene eseguito in modo indipendente e contiene uno o più stadi sequenziali. Quando vengono prese tutte le decisioni necessarie in una fase, inizia la fase successiva in tale percorso, la fase precedente viene bloccata e i revisori e gli approvatori della nuova fase ricevono una notifica e-mail.

Una decisione &quot;Lavoro necessario&quot; interrompe il percorso su ma non influisce sul flusso di lavoro di approvazione su altri percorsi. Puoi configurare fino a 30 percorsi e 100 stadi in totale.

Per creare un flusso di lavoro di approvazione avanzato:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fare clic sul documento necessario per aprire il pannello Riepilogo documento per tale documento.

1. Selezionare la versione del documento per cui si desidera creare un&#39;approvazione nel menu a discesa versione. La versione più recente è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**.

1. Nella parte superiore destra della finestra di dialogo **Richiedi approvazione**, fai clic su **Vai a pagina avanzata**. Qualsiasi input immesso in modalità Base viene mantenuto e applicato a **Percorso 1**, **Stadio 1**.

   >[!TIP]
   >
   >Durante la creazione dell&#39;approvazione, puoi tornare alla modalità Base facendo clic su **Vai alla modalità Base** in alto a destra. Dopo aver fatto clic su **Richiedi approvazione**, l&#39;opzione **Vai a base** non è più disponibile.

1. Inserire i dettagli per la fase 1 del percorso 1:

   <table>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Le fasi sono denominate <em>Fase 1</em>, <em>Fase 2</em> e così via per impostazione predefinita. Rinomina la fase in modo che sia più descrittiva, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.<p>Nota: un revisore o un approvatore può essere assegnato a una sola fase aperta alla volta sulla stessa risorsa. Se più stadi paralleli sono aperti contemporaneamente, la stessa persona non può essere aggiunta a più di uno.</p></td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (facoltativo)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Scadenza il (facoltativo)</strong></td>
   <td>La prima fase di ogni percorso supporta una data di scadenza assoluta. Ogni fase successiva del percorso supporta una data di scadenza relativa, ovvero il numero di giorni a partire dal momento in cui si apre la fase. Gli utenti e i team ricevono una notifica via e-mail 72 ore e quindi 24 ore prima della data di scadenza.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi messaggio personalizzato (facoltativo)</strong></td>
   <td>Digitare un messaggio nella casella di testo <strong>Aggiungi messaggio personalizzato</strong>. Il messaggio viene visualizzato nella notifica e-mail di approvazione e nella scheda Approvazioni in Workfront.<p>Quando si aggiunge una seconda fase, <strong>Mostra questo messaggio in tutte le fasi</strong> è selezionato per impostazione predefinita. Lascia selezionata questa opzione per utilizzare lo stesso messaggio in ogni fase. Per utilizzare un messaggio diverso per ogni fase, deselezionare <strong>Mostra il messaggio in tutte le fasi</strong>, quindi digitare il messaggio specifico per la fase nella casella di testo <strong>Aggiungi messaggio personalizzato</strong> di ogni fase.</p></td>
   </tr>
   </table>

1. (Facoltativo) Fai clic su **Aggiungi fase** per aggiungere un&#39;altra fase al percorso. Le fasi di un percorso vengono eseguite in sequenza nell&#39;ordine in cui sono elencate. È possibile riordinare gli stadi all&#39;interno di un tracciato, ma non è possibile spostare uno stadio da un tracciato all&#39;altro. Ogni percorso può avere un numero diverso di stadi.

1. (Facoltativo) In **Percorsi paralleli**, fai clic su **Aggiungi percorso** per aggiungere un altro percorso. Il nuovo percorso inizia con una fase vuota e diventa il percorso selezionato. Per rinominare un percorso, passa il puntatore sull&#39;etichetta del percorso, fai clic sull&#39;icona della matita, quindi digita un nuovo nome.

1. (Facoltativo) Per rimuovere un percorso, passa il cursore sull’etichetta del percorso e fai clic sull’icona del cestino. Impossibile rimuovere **Percorso 1** e riordinare i percorsi. Altri percorsi possono essere rimossi solo se nessuna fase all&#39;interno del percorso è bloccata o completata.

   ![Modalità avanzata con percorsi paralleli](assets/request-approval-parallel-paths.jpeg)

1. (Facoltativo) Per cancellare tutti i percorsi e gli stadi e ricominciare, fai clic su **Reimposta** in alto a destra.

1. Fai clic su **Richiedi approvazione**.


<!--

## Create an approval workflow in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)
   
-->

## Creare un flusso di lavoro di approvazione nella nuova area Documenti

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Per impostazione predefinita, la finestra di dialogo **Richiedi approvazione** si apre in modalità **Base**. La modalità di base è una singola fase con un set di approvatori o revisori. Passa alla modalità **Avanzate** per configurare approvazioni in più fasi o percorsi paralleli.

### Creare un flusso di lavoro di approvazione di base

Per creare un flusso di lavoro di approvazione in una sola fase:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Compila i seguenti dettagli:

   <table>
   <tr>
   <td><strong>Utilizzare un modello di approvazione (facoltativo)</strong></td>
   <td>Il campo dei modelli è compresso per impostazione predefinita. Fai clic sul campo per espanderlo, quindi seleziona un modello dal menu a discesa. Se il modello ha un percorso e una fase, viene applicato in modalità Base. Se il modello ha più di una fase o più percorsi, la finestra di dialogo passa automaticamente alla modalità Avanzata e qualsiasi input immesso in modalità Base viene sostituito dal contenuto del modello.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.</td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (facoltativo)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Scadenza il (facoltativo)</strong></td>
   <td>Imposta una data di scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della data di scadenza specificata.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi messaggio personalizzato (facoltativo)</strong></td>
   <td>Digitare un messaggio nella casella di testo <strong>Aggiungi messaggio personalizzato</strong>. Il messaggio viene visualizzato nella notifica e-mail di approvazione e nella scheda Approvazioni in Workfront.</td>
   </tr>
   </table>

1. Fai clic su **Richiedi approvazione**.

   ![Richiedi l&#39;approvazione in modalità elementare](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* La finestra di dialogo **Richiedi approvazione** si apre in modalità Base ogni volta, indipendentemente dalla sessione precedente.
>* Se modifichi un messaggio personalizzato dopo la creazione del flusso di lavoro di approvazione, a tutti i partecipanti esistenti viene inviata una notifica e-mail aggiornata. Se aggiungi un partecipante in un secondo momento, il messaggio personalizzato viene incluso nella notifica e-mail.
>* Dopo aver salvato un’approvazione, non puoi ripristinarla alla modalità Base. È possibile passare da un&#39;approvazione in corso all&#39;approvazione di base all&#39;approvazione avanzata, a condizione che l&#39;approvazione non sia bloccata o completata.

### Creare un flusso di lavoro di approvazione avanzato

La modalità avanzata supporta i percorsi paralleli. Ogni percorso viene eseguito in modo indipendente e contiene uno o più stadi sequenziali. Quando vengono prese tutte le decisioni necessarie in una fase, inizia la fase successiva in tale percorso, la fase precedente viene bloccata e i revisori e gli approvatori della nuova fase ricevono una notifica e-mail.

Una decisione &quot;Lavoro necessario&quot; interrompe il percorso su ma non influisce sul flusso di lavoro di approvazione su altri percorsi. Puoi configurare fino a 30 percorsi e 100 stadi in totale.

Per creare un flusso di lavoro di approvazione avanzato:

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fai clic su **Crea flusso di lavoro**.

1. Nella parte superiore destra della finestra di dialogo **Richiedi approvazione**, fai clic su **Vai a pagina avanzata**. Qualsiasi input immesso in modalità Base viene mantenuto e applicato a **Percorso 1**, **Stadio 1**.

   >[!TIP]
   >
   >Durante la creazione dell&#39;approvazione, puoi tornare alla modalità Base facendo clic su **Vai alla modalità Base** in alto a destra. Dopo aver fatto clic su **Richiedi approvazione**, l&#39;opzione **Vai a base** non è più disponibile.

1. Inserire i dettagli per la fase 1 del percorso 1:

   <table>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Le fasi sono denominate <em>Fase 1</em>, <em>Fase 2</em> e così via per impostazione predefinita. Rinomina la fase in modo che sia più descrittiva, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.<p>Nota: un revisore o un approvatore può essere assegnato a una sola fase aperta alla volta sulla stessa risorsa. Se più stadi paralleli sono aperti contemporaneamente, la stessa persona non può essere aggiunta a più di uno.</p></td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (facoltativo)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Scadenza il (facoltativo)</strong></td>
   <td>La prima fase di ogni percorso supporta una data di scadenza assoluta. Ogni fase successiva del percorso supporta una data di scadenza relativa, ovvero il numero di giorni a partire dal momento in cui si apre la fase. Gli utenti e i team ricevono una notifica via e-mail 72 ore e quindi 24 ore prima della data di scadenza.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi messaggio personalizzato (facoltativo)</strong></td>
   <td>Digitare un messaggio nella casella di testo <strong>Aggiungi messaggio personalizzato</strong>. Il messaggio viene visualizzato nella notifica e-mail di approvazione e nella scheda Approvazioni in Workfront.<p>Quando si aggiunge una seconda fase, <strong>Mostra questo messaggio in tutte le fasi</strong> è selezionato per impostazione predefinita. Lascia selezionata questa opzione per utilizzare lo stesso messaggio in ogni fase. Per utilizzare un messaggio diverso per ogni fase, deselezionare <strong>Mostra il messaggio in tutte le fasi</strong>, quindi digitare il messaggio specifico per la fase nella casella di testo <strong>Aggiungi messaggio personalizzato</strong> di ogni fase.</p></td>
   </tr>
   </table>

1. (Facoltativo) Fai clic su **Aggiungi fase** per aggiungere un&#39;altra fase al percorso. Le fasi di un percorso vengono eseguite in sequenza nell&#39;ordine in cui sono elencate. È possibile riordinare gli stadi all&#39;interno di un tracciato, ma non è possibile spostare uno stadio da un tracciato all&#39;altro. Ogni percorso può avere un numero diverso di stadi.


1. (Facoltativo) In **Percorsi paralleli**, fai clic su **Aggiungi percorso** per aggiungere un altro percorso. Il nuovo percorso inizia con una fase vuota e diventa il percorso selezionato. Per rinominare un percorso, passa il puntatore sull&#39;etichetta del percorso, fai clic sull&#39;icona della matita, quindi digita un nuovo nome.

1. (Facoltativo) Per rimuovere un percorso, passa il cursore sull’etichetta del percorso e fai clic sull’icona del cestino. Impossibile rimuovere **Percorso 1** e riordinare i percorsi. Altri percorsi possono essere rimossi solo se nessuna fase all&#39;interno del percorso è bloccata o completata.

   ![Modalità avanzata con percorsi paralleli](assets/request-approval-advanced.jpeg)

1. (Facoltativo) Per cancellare tutti i percorsi e gli stadi e ricominciare, fai clic su **Reimposta** in alto a destra.

1. Fai clic su **Richiedi approvazione**.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
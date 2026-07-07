---
product-area: documents
navigation-topic: approvals
title: Creare un modello di flusso di lavoro di approvazione per i documenti
description: Puoi creare modelli di approvazione per semplificare il processo di approvazione.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5e9318366f0dff85591a5d5a752920027f5c9b0e
workflow-type: tm+mt
source-wordcount: 895
ht-degree: 5%

---

# Creare un modello di flusso di lavoro di approvazione per i documenti

{{highlighted-preview}}

Nell’area Configurazione di Workfront, gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili. Una volta creati, i modelli di approvazione possono essere applicati alle risorse nell’area Documenti di un oggetto.
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
   <td><p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Piano</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un modello di approvazione in produzione

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Revisione e approvazione** > **Modelli di approvazione**.
1. Fai clic su **Nuovo modello** sul lato destro della pagina.

1. Compila i seguenti dettagli:

   <table>
     <tr>
   <td><strong>Nome modello</strong></td>
   <td>Aggiungi un nome modello. </td>
   </tr>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Aggiungete un nome di fase. È possibile modificare il nome in modo che sia più descrittivo, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. Se si dispone solo di revisori, questi riceveranno una notifica e avranno la possibilità di completare la revisione, ma non sarà necessaria o presa alcuna decisione.</td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (opzionale)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Giornate di lavoro fino alla data di scadenza</strong></td>
   <td>Scegli quanti giorni lavorativi mancano alla scadenza dell’approvazione dopo l’attivazione di una fase.</td>
   </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altre fasi in base alle esigenze.

   >[!NOTE]
   >
   >Se aggiungi più fasi, il flusso di lavoro di approvazione procede nell’ordine in cui sono elencate. Quando tutte le decisioni necessarie vengono prese, inizia la fase successiva e la fase precedente viene bloccata.

   ![Dettagli documento](assets/new-stage.png)

1. Fai clic su **Salva**.

Una volta creato, il modello può essere applicato ai documenti nell&#39;area Documenti di un oggetto per avviare il processo formale di revisione e approvazione in Workfront.

<div class="preview">

## Creare un modello di approvazione in Anteprima

La finestra di dialogo del modello di approvazione si apre sempre in modalità Avanzata. Non esiste una modalità di base per i modelli. Puoi configurare fino a 30 percorsi paralleli in un modello, per un totale di 100 stadi. Ogni percorso viene eseguito in modo indipendente e può contenere uno o più stadi sequenziali.

Per creare un modello di approvazione:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Revisione e approvazione** > **Modelli di approvazione**.

1. Fai clic su **Nuovo modello** sul lato destro della pagina.

1. Aggiungi un **nome modello**.

1. Inserire i dettagli per la fase 1 del percorso 1:

   <table>
   <tr>
   <td><strong>Nome fase</strong></td>
   <td>Le fasi sono denominate <em>Fase 1</em>, <em>Fase 2</em> e così via per impostazione predefinita. Rinomina la fase in modo che sia più descrittiva, ad esempio <em>Revisione iniziale</em> o <em>Approvazione finale</em>.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi nomi o e-mail (facoltativo)</strong></td>
   <td>Inizia a digitare il nome di un utente o team da aggiungere come approvatore o revisore. I partecipanti sono facoltativi nei modelli. È possibile aggiungerli quando il modello viene applicato a un documento.<p>Nota: un revisore o un approvatore può essere assegnato a una sola fase aperta alla volta sulla stessa risorsa. Se più stadi paralleli sono aperti contemporaneamente, la stessa persona non può essere aggiunta a più di uno.</p></td>
   </tr>
   <tr>
   <td><strong>È necessaria una sola decisione (facoltativo)</strong></td>
   <td>La prima persona che prende una decisione completa la fase.</td>
   </tr>
   <tr>
   <td><strong>Giorni lavorativi fino alla data di scadenza (facoltativo)</strong></td>
   <td>Scegliere il numero di giorni lavorativi necessari per il completamento della fase dopo l'apertura. La prima fase di ogni percorso supporta anche una data di scadenza assoluta. Ogni fase successiva del percorso supporta solo una data di scadenza relativa.</td>
   </tr>
   <tr>
   <td><strong>Aggiungi messaggio personalizzato (facoltativo)</strong></td>
   <td>Digitare un messaggio nella casella di testo <strong>Aggiungi messaggio personalizzato</strong>. Quando il modello viene applicato a un documento, il messaggio viene visualizzato nella notifica e-mail di approvazione e nella scheda Approvazioni di Workfront.<p>Quando si aggiunge una seconda fase, <strong>Mostra questo messaggio in tutte le fasi</strong> è selezionato per impostazione predefinita. Lascia selezionata questa opzione per utilizzare lo stesso messaggio in ogni fase. Per utilizzare un messaggio diverso per ogni fase, deselezionare <strong>Mostra il messaggio in tutte le fasi</strong>, quindi digitare il messaggio specifico per la fase nella casella di testo <strong>Aggiungi messaggio personalizzato</strong> di ogni fase.</p></td>
   </tr>
   </table>

   ![aggiungi una fase](assets/add-stage.png)

1. (Facoltativo) Fai clic su **Aggiungi fase** per aggiungere un&#39;altra fase al percorso. Le fasi di un percorso vengono eseguite in sequenza nell&#39;ordine in cui sono elencate. Quando vengono prese tutte le decisioni necessarie in una fase, inizia la fase successiva di quel percorso e la fase precedente viene bloccata. È possibile riordinare gli stadi all&#39;interno di un tracciato, ma non è possibile spostare uno stadio da un tracciato all&#39;altro. Ogni percorso può avere un numero diverso di stadi.

1. (Facoltativo) In **Percorsi paralleli**, fai clic su **Aggiungi percorso** per aggiungere un altro percorso. Il nuovo percorso inizia con una fase vuota e diventa il percorso selezionato. Impossibile riordinare i percorsi.

   ![aggiungi percorsi paralleli](assets/add-path.png)

1. (Facoltativo) Per rinominare un percorso, passa il cursore sull’etichetta del percorso, fai clic sull’icona della matita, quindi digita un nuovo nome. Per rimuovere un percorso, passa il cursore sull’etichetta del percorso e fai clic sull’icona del cestino. **Il percorso 1** non può essere rimosso e gli altri percorsi possono essere rimossi solo se nessuna fase all&#39;interno del percorso è bloccata o completata.

1. (Facoltativo) Per cancellare tutti i percorsi e gli stadi e ricominciare da capo, fai clic su **Reimposta** in alto a destra.

1. Fai clic su **Salva**.

Una volta creato, il modello può essere applicato ai documenti nell&#39;area Documenti di un oggetto per avviare il processo formale di revisione e approvazione in Workfront.

</div>



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->

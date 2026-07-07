---
product-area: documents
navigation-topic: approvals
title: Caricare una nuova versione del documento e richiedere un’approvazione
description: Puoi caricare una nuova versione del documento e richiedere l’approvazione di altri utenti in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 82530b9b87f6865ec294adcdc601443ee48dcbcf
workflow-type: tm+mt
source-wordcount: 1196
ht-degree: 5%

---

# Caricare una nuova versione del documento e richiedere un’approvazione

{{highlighted-preview}}

Se un documento è contrassegnato come &quot;Da lavorare&quot; in una revisione precedente, è possibile caricare una nuova versione nel documento originale e avviare un altro ciclo di approvazioni. Dopo aver caricato una nuova versione del documento, le versioni precedenti vengono bloccate.

Se il nome del file della nuova versione è diverso da quello della versione precedente, Workfront visualizza il documento con il nome più recente.

Quando si aggiunge una nuova versione a un documento con approvazioni in sospeso, l’approvazione della versione precedente viene visualizzata come &quot;Ritirata&quot;. Il precedente processo di approvazione si chiude, anche se alcuni partecipanti non hanno ancora preso una decisione.

Se la versione più recente del documento viene eliminata, le versioni precedenti rimangono bloccate. Se devi modificare una versione precedente, devi sbloccarla manualmente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire le approvazioni utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> <p>Richiedente o successiva</p>
   <p>Collaboratore o successiva</p>
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Modifica l'accesso all'oggetto associato al documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Usa il trascinamento della selezione per aggiungere una nuova versione nell’area dei documenti legacy in Produzione

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.


Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront.

È possibile aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nella pagina Dettagli documento.

Per aggiungere una nuova versione:

1. Passare al documento in Workfront.
1. Trascinare il nuovo file sopra il documento precedente. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo documento. Qui puoi vedere il numero di versione nella parte superiore del pannello.


1. Scorri verso il basso fino alla sezione **Approvazioni**.

1. Fai clic su **Crea flusso di lavoro**, quindi compila i seguenti dettagli:

   <table>
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
   <td><strong>Data di scadenza (facoltativo)</strong></td>
   <td>Imposta una data di scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della data di scadenza specificata.</td>
   </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altre fasi in base alle esigenze.

   >[!NOTE]
   >
   >Se aggiungi più fasi, il flusso di lavoro di approvazione procede nell’ordine in cui sono elencate. Quando tutte le decisioni necessarie vengono prese, inizia la fase successiva e la fase precedente viene bloccata.



1. (Facoltativo) Per aggiungere un modello di approvazione esistente, seleziona un modello dalla parte sinistra della finestra di dialogo.

   >[!TIP]
   >
   >   Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, vedere [Creare un modello di workflow di approvazione per i documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Dopo aver aggiunto tutte le fasi e i partecipanti necessari, fai clic su **Richiedi approvazione**.

   Il flusso di lavoro di approvazione viene avviato e gli approvatori ricevono una notifica che indica che la loro approvazione è necessaria per la nuova versione del documento. La versione precedente del documento è bloccata e tutte le approvazioni in sospeso relative alla versione precedente vengono ritirate.

   ![richiedi approvazione
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

<div class="preview">

## Usa il trascinamento della selezione per aggiungere una nuova versione nell’area dei documenti legacy in Anteprima

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione cloud Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.

Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront. È possibile aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nella pagina Dettagli documento.

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per aggiungere una nuova versione e richiedere l’approvazione:

1. Passare al documento in Workfront.

1. Trascinare il nuovo file sopra il documento precedente. Workfront crea automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo documento. Il numero di versione viene visualizzato nella parte superiore del pannello.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Fai clic su **Richiedi approvazione**.

   Il flusso di lavoro di approvazione viene avviato e gli approvatori ricevono una notifica che indica che la loro approvazione è necessaria per la nuova versione del documento. La versione precedente del documento è bloccata e tutte le approvazioni in sospeso relative alla versione precedente vengono ritirate.

## Trascinare la selezione per aggiungere una nuova versione nell&#39;area Nuovi documenti di Anteprima

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.

Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront. È possibile aggiungere un flusso di lavoro di approvazione alla nuova versione del documento.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

Per impostazione predefinita, la finestra di dialogo Richiedi approvazione si apre in modalità Base per l’approvazione in una sola fase. Passa alla modalità avanzata per configurare approvazioni in più fasi o percorsi paralleli.

Per aggiungere una nuova versione e richiedere l’approvazione:

1. Passare al documento in Workfront.

1. Trascinare il nuovo file sopra il documento precedente. Workfront crea automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo. La versione più recente del documento è selezionata per impostazione predefinita.

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**. La finestra di dialogo **Richiedi approvazione** si apre in modalità Base.

1. Configura il flusso di lavoro di approvazione. Per le descrizioni dei campi, l&#39;attivazione della modalità avanzata e il flusso dei percorsi paralleli, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Fai clic su **Richiedi approvazione**.

   Il flusso di lavoro di approvazione viene avviato e gli approvatori ricevono una notifica che indica che la loro approvazione è necessaria per la nuova versione del documento. La versione precedente del documento è bloccata e tutte le approvazioni in sospeso relative alla versione precedente vengono ritirate.

</div>

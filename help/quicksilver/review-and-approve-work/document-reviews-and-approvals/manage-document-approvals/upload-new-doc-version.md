---
product-area: documents
navigation-topic: approvals
title: Caricare una nuova versione del documento e richiedere un’approvazione
description: Puoi caricare una nuova versione del documento e richiedere l’approvazione di altri utenti in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 10%

---

# Caricare una nuova versione del documento e richiedere un’approvazione

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
   <td> <p>Qualsiasi</p> </td> 
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



## Usa il trascinamento della selezione per aggiungere una nuova versione nell’area dei documenti legacy

Se l&#39;organizzazione utilizza l&#39;archiviazione Workfront, quando si accede ai documenti in Workfront verrà visualizzata l&#39;area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Archiviazione Workfront e archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

>[!NOTE]
>
>Il trascinamento della selezione non funziona con Internet Explorer.


Se è necessario eseguire un altro ciclo di revisione e approvazione su un documento, è possibile creare una nuova versione del documento in Workfront.

È possibile aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nella pagina Dettagli documento.

Per aggiungere una nuova versione:

1. Passare al documento in Workfront.
1. Trascinare il nuovo file sopra il documento precedente. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionare il documento per aprire il pannello Riepilogo documento. Qui puoi vedere il numero di versione nella parte superiore del pannello.
   ![Aprire la pagina dei dettagli del documento](assets/open-doc-details.png)


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

   ![richiede l&#39;approvazione](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

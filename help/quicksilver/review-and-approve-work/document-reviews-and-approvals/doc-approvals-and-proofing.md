---
product-area: documents
navigation-topic: approvals
title: Utilizzare insieme approvazioni unificate e bozze
description: Puoi utilizzare le Approvazioni unificate con la verifica.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1723'
ht-degree: 1%

---

# Utilizzare insieme approvazioni unificate e bozze

Approvazioni unificate in Workfront introduce una nuova serie di funzioni per facilitare la revisione e l’approvazione dei documenti. È possibile utilizzare un flusso di lavoro Approvazioni unificate con il visualizzatore di bozze esistente per aggiungere commenti e markup ai documenti in revisione.

Esistono alcune differenze chiave nel flusso di lavoro quando si utilizzano insieme le approvazioni unificate e la verifica:

* I partecipanti vengono visualizzati nel riepilogo del documento, non nel flusso di lavoro di verifica.

* I dettagli Inviato, Aperto, Commento, Decisione (SOCD) nell’elenco dei documenti sono correlati alle verifiche e non riflettono lo stato della decisione del documento.

## Utilizzare insieme le approvazioni e le prove unificate nell&#39;ambiente di produzione

### Caricare un documento e creare una bozza

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.
Oppure
Trascinare il documento nell&#39;elenco dei documenti.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento e seleziona **Bozza semplice**. È necessario creare una bozza semplice perché non utilizzerai il flusso di lavoro di bozza per le approvazioni.

Gli utenti assegnati come partecipanti possono utilizzare il visualizzatore di bozze per aggiungere commenti e markup al documento. Passare alla sezione successiva per scoprire come aggiungere partecipanti di revisione.

### Aprire il documento Riepilogo e assegnare i partecipanti

È possibile assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Non è necessario contrassegnare la revisione come completata per far avanzare il documento nel processo di approvazione.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.

Per assegnare i partecipanti:

1. Seleziona il documento caricato e apri il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. Scegli un modello di approvazione esistente (facoltativo). Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, vedere [Creare un modello di workflow di approvazione per i documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fare clic sul pulsante Approvatore e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, fare clic sul pulsante Revisore e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

### Crea una nuova versione in base alle esigenze

Se hai bisogno di un altro ciclo di revisione e approvazione, puoi creare una nuova versione della bozza e aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nel Riepilogo del documento.

Per aggiungere una nuova versione:

1. Trascinare e rilasciare il nuovo file sopra il documento precedente in Workfront. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionarlo e fare clic su **Crea bozza** > **Bozza semplice**.

1. Selezionare nuovamente il documento e aprire il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. Scegli un modello di approvazione esistente (facoltativo). Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, vedere [Creare un modello di workflow di approvazione per i documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fare clic sul pulsante Approvatore e iniziare a digitare il nome di un utente o di un team oppure scegliere un approvatore della versione precedente.

1. Per aggiungere un revisore, fare clic sul pulsante Revisore e iniziare a digitare il nome di un utente o di un team, scegliere un revisore della versione precedente.

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

<!-- add info about reusing previous participants once released -->


### Verifica la bozza e prendi una decisione

Il documento non passa a uno stato approvato finché tutti gli approvatori assegnati non scelgono &quot;approvato&quot;.

Per rivedere e approvare un documento:

1. Vai alla notifica e-mail di revisione e fai clic su **Vai alla revisione**.

1. Una volta in Workfront, fai clic su **Vai alla bozza**.

1. Rivedi il contenuto e aggiungi eventuali commenti o markup. Per ulteriori informazioni sull&#39;utilizzo del visualizzatore di bozze, vedere [Rivedere le bozze in Adobe Workfront: article index](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Scegli una delle seguenti decisioni:

   * **Approva**: il documento non necessita di modifiche ed è pronto per l&#39;uso.
   * **Approva con modifiche**: il documento richiede modifiche ed è pronto per l&#39;uso una volta apportate. Non è necessaria un&#39;ulteriore approvazione.
   * **Lavoro necessario**: il documento richiede modifiche e non è pronto per l&#39;uso. Dopo aver apportato le modifiche specificate, il documento deve essere caricato come nuova versione e superare un altro ciclo di approvazioni. Per ulteriori informazioni sul caricamento di una nuova versione, vedere [Creare una nuova versione in base alle esigenze](#create-a-new-version-as-needed) in questo articolo.

Una volta presa una decisione, il proprietario del documento riceve una notifica tramite e-mail.


<div class="preview">


## Utilizzare insieme le approvazioni e le prove unificate nell’ambiente di anteprima

### Caricare un documento e creare una bozza

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.
Oppure
Trascinare il documento nell&#39;elenco dei documenti.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento e seleziona **Bozza semplice**. È necessario creare una bozza semplice perché non utilizzerai il flusso di lavoro di bozza per le approvazioni.

Gli utenti assegnati come partecipanti possono utilizzare il visualizzatore di bozze per aggiungere commenti e markup al documento. Passare alla sezione successiva per scoprire come aggiungere partecipanti di revisione.

### Aprire il documento Riepilogo e assegnare i partecipanti

È possibile assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Non è necessario contrassegnare la revisione come completata per far avanzare il documento nel processo di approvazione.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.

Per assegnare i partecipanti:

1. Seleziona il documento caricato e apri il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**.


1. Compila i seguenti dettagli:

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

   ![nuova fase](assets/new-stage.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fai clic su **Richiedi approvazioni**. I partecipanti vengono informati via e-mail.


### Crea una nuova versione in base alle esigenze

Se hai bisogno di un altro ciclo di revisione e approvazione, puoi creare una nuova versione della bozza e aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nel Riepilogo del documento.

Per aggiungere una nuova versione:

1. Trascinare e rilasciare il nuovo file sopra il documento precedente in Workfront. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionarlo e fare clic su **Crea bozza** > **Bozza semplice**.

1. Selezionare nuovamente il documento e aprire il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione **Approvazioni**, quindi fai clic su **Crea flusso di lavoro**.


1. Compila i seguenti dettagli:

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

   ![nuova fase](assets/new-stage.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fai clic su **Richiedi approvazioni**. I partecipanti vengono informati via e-mail.



### Verifica la bozza e prendi una decisione

Il documento non passa a uno stato approvato finché tutti gli approvatori assegnati non scelgono &quot;approvato&quot;.

Per rivedere e approvare un documento:

1. Vai alla notifica e-mail di revisione e fai clic su **Vai alla revisione**.

1. Una volta in Workfront, fai clic su **Vai alla bozza**.

1. Rivedi il contenuto e aggiungi eventuali commenti o markup. Per ulteriori informazioni sull&#39;utilizzo del visualizzatore di bozze, vedere [Rivedere le bozze in Adobe Workfront: article index](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Scegli una delle seguenti decisioni:

   * **Approva**: il documento non necessita di modifiche ed è pronto per l&#39;uso.
   * **Approva con modifiche**: il documento richiede modifiche ed è pronto per l&#39;uso una volta apportate. Non è necessaria un&#39;ulteriore approvazione.
   * **Lavoro necessario**: il documento richiede modifiche e non è pronto per l&#39;uso. Dopo aver apportato le modifiche specificate, il documento deve essere caricato come nuova versione e superare un altro ciclo di approvazioni. Per ulteriori informazioni sul caricamento di una nuova versione, vedere [Creare una nuova versione in base alle esigenze](#create-a-new-version-as-needed) in questo articolo.

Una volta presa una decisione, il proprietario del documento riceve una notifica tramite e-mail.

</div>
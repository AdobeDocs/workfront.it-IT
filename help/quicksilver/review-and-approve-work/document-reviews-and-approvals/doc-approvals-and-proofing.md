---
product-area: documents
navigation-topic: approvals
title: Utilizzare insieme approvazioni unificate e prove
description: Puoi utilizzare le Approvazioni unificate con la verifica.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Utilizzare insieme approvazioni unificate e prove

Approvazioni unificate in Workfront introduce una nuova serie di funzioni per facilitare la revisione e l’approvazione dei documenti. È possibile utilizzare un flusso di lavoro Approvazioni unificate con il visualizzatore di bozze esistente per aggiungere commenti e markup ai documenti in revisione.

Esistono alcune differenze chiave nel flusso di lavoro quando si utilizzano insieme le approvazioni unificate e la verifica:

* I partecipanti vengono visualizzati nel riepilogo del documento, non nel flusso di lavoro di verifica

* I dettagli Inviato, Aperto, Commento, Decisione (SOCD) nell’elenco dei documenti sono correlati alle verifiche e non riflettono lo stato della decisione del documento.

## Caricare un documento e creare una bozza

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.
Oppure
Trascinare il documento nell&#39;elenco dei documenti.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento e seleziona **Bozza semplice**. È necessario creare una bozza semplice perché non utilizzerai il flusso di lavoro di bozza per le approvazioni.

Gli utenti assegnati come partecipanti possono utilizzare il visualizzatore di bozze per aggiungere commenti e markup al documento. Passare alla sezione successiva per scoprire come aggiungere partecipanti di revisione.

## Aprire il documento Riepilogo e assegnare i partecipanti

È possibile assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Non è necessario contrassegnare la revisione come completata per far avanzare il documento nel processo di approvazione.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.

Per assegnare i partecipanti:

1. Seleziona il documento caricato e apri il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. Scegli un modello di approvazione esistente (facoltativo). Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, consulta [Creare un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fare clic sul pulsante Approvatore e iniziare a digitare il nome di un utente o di un team.

1. Per aggiungere un revisore, fare clic sul pulsante Revisore e iniziare a digitare il nome di un utente o di un team.

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

## Crea una nuova versione in base alle esigenze

Se hai bisogno di un altro ciclo di revisione e approvazione, puoi creare una nuova versione della bozza e aggiungere i partecipanti precedenti, nuovi partecipanti o una combinazione di entrambi. È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nel Riepilogo del documento.

Per aggiungere una nuova versione:

1. Trascinare e rilasciare il nuovo file sopra il documento precedente in Workfront. Viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, selezionarlo e fare clic su **Crea bozza** > **Bozza semplice**.

1. Selezionare nuovamente il documento e aprire il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. Scegli un modello di approvazione esistente (facoltativo). Gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili dall’area Configurazione. Per ulteriori informazioni, consulta [Creare un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Imposta una scadenza per l’approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e in seguito 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fare clic sul pulsante Approvatore e iniziare a digitare il nome di un utente o di un team oppure scegliere un approvatore della versione precedente.

1. Per aggiungere un revisore, fare clic sul pulsante Revisore e iniziare a digitare il nome di un utente o di un team, scegliere un revisore della versione precedente.

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

<!-- add info about reusing previous participants once released -->


## Verifica la bozza e prendi una decisione

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


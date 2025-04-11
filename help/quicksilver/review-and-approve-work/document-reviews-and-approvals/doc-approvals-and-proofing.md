---
product-area: documents
navigation-topic: approvals
title: Utilizzare le approvazioni unificate e le prove di prova insieme
description: Puoi utilizzare le approvazioni unificate con le correzioni.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 300de02b81bc6abc8be9bdceb2bd028b0c4aabfe
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Utilizzare le approvazioni unificate e le prove di prova insieme

Approvazioni unificate in Workfront introduce una nuova serie di funzionalità che consentono di esaminare e approvare i documenti. È possibile utilizzare un workflow Approvazioni unificate con il visualizzatore di correzione esistente per aggiungere commenti e markup ai documenti in revisione.

Esistono alcune differenze chiave nel workflow quando si utilizzano congiuntamente le approvazioni unificate e le prove:

* I pulsanti di decisione non vengono visualizzati nel visualizzatore di correzione

* I partecipanti sono mostrati nel riepilogo del documento, non nel workflow di correzione

* I dettagli di Inviato, Aperto, Commento, Decisione (SOCD) nell&#39;elenco dei documenti sono correlati alle correzioni e non riflettono lo stato decisionale del documento.

## Caricare un documento e creare una prova

1. Vai al progetto, all&#39;attività o al problema in cui desideri aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.
Oppure
Trascinare il documento nell&#39;elenco dei documenti.

   >[!NOTE]
   >
   >Se nel tuo profilo utente sono abilitati **Genera automaticamente delle bozze durante il caricamento dei documenti**, il sistema crea automaticamente una bozza semplice.

1. Passa il puntatore del mouse sul documento, quindi fai clic sul collegamento **Crea bozza** visualizzato sotto il nome del documento e seleziona **Bozza semplice**. È necessario creare una bozza semplice perché non utilizzerai il flusso di lavoro di bozza per le approvazioni.

Gli utenti assegnati come partecipanti possono utilizzare il visualizzatore di bozze per aggiungere commenti e markup al documento. Passare alla sezione successiva per scoprire come aggiungere partecipanti di revisione.

## Apri il riepilogo del documento e assegna i partecipanti

È possibile assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Non è necessario contrassegnare la revisione come completata per far avanzare il documento nel processo di approvazione.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.

Per assegnare i partecipanti:

1. Selezionare il documento caricato e aprire il documento Riepilogo.
   ![Apri riepilogo documento](assets/open-doc-summary.png)

1. Scorri verso il basso fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. (Facoltativo) Scegli un modello di approvazione esistente. Gli utenti con una licenza Standard possono creare modelli di approvazione utilizzabili dall&#39;area Configurazione. Per ulteriori informazioni, vedere [Crea un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Stabilisci una scadenza per l&#39;approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e poi 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fare clic sull&#39;pulsante Approvatore e iniziare a digitare un utente o team nome.

1. Per aggiungere un revisore, fare clic sull&#39;pulsante Revisore e iniziare a digitare un utente o team nome.

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

## Crea una nuova versione in base alle esigenze

Se hai bisogno di un altro ciclo di revisione e approvazione, puoi creare una nuova versione della bozza.  <!-- and add the previous participants, new participants, or a mix of both. --> È possibile visualizzare informazioni sulle versioni precedenti e sui partecipanti nel Riepilogo del documento.

Per aggiungere una nuova versione:

1. Trascinare e rilasciare il nuovo file sopra il documento precedente in Workfront. In questo modo viene creata automaticamente una nuova versione.

1. Al termine del caricamento del documento, seleziona il documento, quindi fai clic su **Crea prova** > **prova semplice**.

1. Selezionare nuovamente il documento e aprire il Riepilogo del documento.
   ![Apri riepilogo documenti](assets/open-doc-summary.png)

1. Scorri fino alla sezione Approvazioni, quindi fai clic su **Aggiungi**.

1. Scegli un modello di approvazione esistente (facoltativo). Gli utenti con una licenza Standard possono creare modelli di approvazione utilizzabili dall&#39;area Configurazione. Per ulteriori informazioni, vedere [Crea un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facoltativo) Stabilisci una scadenza per l&#39;approvazione. Gli utenti e i team ricevono una notifica via e-mail 72 ore e poi 24 ore prima della scadenza specificata.

1. Per aggiungere un approvatore, fai clic sul pulsante Approvatore e inizia a digitare un nome utente o team<span class="preview"> oppure scegli un approvatore della versione precedente.</span>

1. Per aggiungere un revisore, fare clic sull&#39;pulsante Revisore e iniziare a digitare un nome utente o team <span class="preview">oppure scegliere un revisore della versione precedente. </span>

   ![Aggiungi approvatori](assets/add-approvers.png)

1. Dopo aver aggiunto tutti i revisori e gli approvatori, fare clic su **Invia richiesta**. I partecipanti vengono informati via e-mail.

<!-- add info about reusing previous participants once released -->


## Verifica la bozza e prendi una decisione

Il documento non passa a uno stato approvato finché tutti gli approvatori assegnati non scelgono &quot;approvato&quot;.

Se un approvatore sceglie &quot;lavoro necessario&quot;, lo stato del documento cambia immediatamente in Lavoro necessario. Il documento dovrà essere rivisto e caricato come nuova versione con un nuovo flusso di lavoro di approvazione.

>[!IMPORTANT]
>
>I pulsanti di decisione del documento non vengono visualizzati nel visualizzatore di correzione. È necessario tornare alla pagina Riepilogo documento o Dettagli documento per prendere una decisione o contrassegnare la revisione completata.

Per esaminare e approvare un documento:

1. Vai all&#39;e-mail di notifica della recensione e fai clic su Vai alla **revisione**.

1. Una volta in Workfront, fai clic su **Vai alla prova**.

1. Rivedi il contenuto e aggiungi eventuali commenti o markup. Per ulteriori informazioni sull&#39;utilizzo del visualizzatore di bozze, vedere [Rivedere le bozze in Adobe Workfront: article index](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Al termine della revisione, chiudete la visualizzatore di correzione.

1. Se ti trovi nella pagina Dettagli documento, i pulsanti di decisione si trovano nell&#39;angolo in alto a destra dello schermo.

1. Scegli una delle seguenti decisioni:

   * **Approva**: il documento non necessita di modifiche ed è pronto per l&#39;uso.
   * **Approva con modifiche**: il documento necessita di modifiche ed è pronto per l&#39;uso una volta apportate. Non è richiesta un&#39;ulteriore approvazione.
   * **Ha bisogno di lavoro**: il documento necessita di modifiche e non è pronto per l&#39;uso. Una volta apportate le modifiche specificate, il documento deve essere caricato come nuova versione e passare attraverso un altro ciclo di approvazioni. Per ulteriori informazioni sul caricamento di una nuova versione, consultate [Crea una nuova versione in base alle esigenze](#create-a-new-version-as-needed) in questo articolo.

Una volta presa una decisione, il documento proprietario viene notificato via e-mail.

---
product-area: projects
navigation-topic: approvals
title: Approvazione del lavoro
description: Approvazione del lavoro
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Approvazione del lavoro

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Se si è impostati come approvatore, è necessario verificare regolarmente il lavoro in attesa di approvazione.

Per informazioni sulla creazione dei processi di approvazione, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Per informazioni sull&#39;associazione delle approvazioni al lavoro in Workfront, vedere [Associare un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o accesso successivo agli oggetti associati alle approvazioni</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti associati alle approvazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Individuare le approvazioni in Adobe Workfront

Puoi visualizzare e gestire le approvazioni in varie aree di Workfront.

Per ulteriori informazioni sulla visualizzazione degli elementi in attesa di approvazione o degli elementi inviati personalmente per l&#39;approvazione, vedere [Visualizza approvazioni](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Approva lavoro dalla sezione Home

1. Fai clic sull&#39;icona **Home** ![](assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >   
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro della pagina, quindi fai clic su **Home**.

1. Fai clic sul menu a discesa **Filtro**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Seleziona **Approvazioni**.\
   Vengono visualizzati tutti gli elementi di lavoro che richiedono l&#39;approvazione. 

   >[!NOTE]
   >
   >Le approvazioni assegnate a Ruoli o Gruppi non vengono visualizzate nella Home. Le approvazioni assegnate ai team vengono visualizzate nel raggruppamento Richiesta team in Work List (Elenco di lavoro).

1. (Facoltativo) Modificare l&#39;ordine di visualizzazione delle approvazioni, come descritto nella sezione &quot;Raggruppa e ordina per data, progetto o priorità&quot; nell&#39;articolo [Visualizzare gli elementi nell&#39;elenco di lavoro nell&#39;area Home](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Seleziona l’elemento in cui desideri prendere una decisione di approvazione.

   ![](assets/task-approval-home-350x127.png)

1. Fai clic su una delle opzioni disponibili quando prendi una decisione di approvazione nel pannello a destra. Le seguenti opzioni vengono visualizzate nell&#39;angolo superiore destro della pagina, a seconda del tipo di elemento che si sta approvando:

   * **Progetti:** Fai clic su **Approva** o **Rifiuta**.

   * **Attività:** Fai clic su **Approva** o **Rifiuta**.

   * **Problemi:** Fai clic su **Approva** o **Rifiuta**.

   * **Schede orario:** Fare clic su **Approva** o **Rifiuta**.

   * **Documenti:** Fare clic su **Approva**, **Rifiuta** o **Modifiche**.\
      Considera quanto segue durante la visualizzazione  approvazioni:

      * Le approvazioni delle bozze vengono visualizzate qui quando un utente condivide una bozza con te, come descritto nella sezione &quot;Condividi un collegamento alla bozza&quot; nell&#39;articolo [Condividi una bozza in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Le approvazioni delle bozze vengono visualizzate nell’area Home solo se l’ambiente Workfront è integrato con un account Workfront Proof Premium. Se non è possibile utilizzare gli strumenti di correzione come descritto qui, contattare l&#39;amministratore di Workfront.
      * Ricevi una notifica in-app con la quale ti viene notificata l’approvazione della verifica.\
        Per ulteriori informazioni sulle notifiche in-app, vedere [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * Il nome dell’utente che ha richiesto l’approvazione viene visualizzato accanto all’immagine miniatura nell’area Home, con il testo seguente:\
        &quot;*L&#39;utente A* richiede la tua approvazione per...&quot;

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        Se il nome utente non è disponibile, viene visualizzato il testo seguente:\
        &quot;È pronta una nuova versione di una bozza&quot;
      * Per prendere una decisione di approvazione sulla bozza, fai clic su **Vai alla bozza**, fai clic su **Termina revisione**, quindi fai clic su una delle opzioni disponibili. Le opzioni disponibili per l&#39;approvazione di una bozza sono: **Approvato**, **Approvato con modifiche**, **Modifiche richieste** e **Non pertinente**.

      * Dopo aver preso una decisione sulla bozza, la bozza rimane nella scheda Approvazioni personali con il testo &quot;Presa di decisione&quot; fino a quando non fai clic sul pulsante **Aggiorna** o non aggiorni la pagina del browser.

        Per informazioni sulla revisione di una bozza, vedi [Verifica delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **Accesso:** Selezionare il livello di accesso da concedere nel menu a discesa **Cambia accesso**, quindi fare clic su **Concedi accesso**. In alternativa, fare clic su **Ignora**.

## Approvare il lavoro direttamente da un progetto, attività o problema

Quando un progetto, un’attività o un problema è in attesa di approvazione, è possibile approvare o rifiutare l’approvazione direttamente dal progetto, dall’attività o dal problema. Puoi anche visualizzare i dettagli relativi al processo di approvazione.

Per approvare il lavoro direttamente da un progetto, attività o problema:

1. Vai al progetto, all’attività o al problema che richiede la tua approvazione.

   Le informazioni sull&#39;approvazione relative al processo di approvazione corrente di un progetto, attività o problema vengono visualizzate nell&#39;intestazione dell&#39;elemento.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Sono disponibili le seguenti informazioni sull’approvazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td>Lo stato corrente del progetto, dell’attività o del problema. Lo stato corrente dell'elemento in attesa di approvazione. Lo stato viene approvato dopo ogni fase del processo di approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fasi di approvazione</td> 
      <td>Le fasi del processo di approvazione. <br>La fase corrente in attesa di approvazione viene visualizzata come In sospeso. Gli stadi che sono già stati approvati vengono visualizzati come Approvati, mentre quelli che non sono ancora stati approvati vengono visualizzati come Non avviato.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **Approva** o **Rifiuta**, a seconda che si desideri approvare o rifiutare il processo di approvazione.\
   La fase di approvazione in attesa di approvazione viene ora approvata e il processo di approvazione passa alla fase successiva. Lo stato viene approvato dopo che tutte le fasi sono state approvate.

## Approvare un documento direttamente da un documento 

1. Passare all&#39;area documenti contenente il documento che richiede l&#39;approvazione.
1. Seleziona il documento, quindi fai clic su **Approva**, **Modifiche** o **Rifiuta**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Facoltativo) Se è stata generata una bozza per il documento, è possibile approvare il documento all&#39;interno dell&#39;interfaccia di correzione, come descritto in [Approvare un documento da una bozza](#approve-a-document-from-a-proof).

## Approvare un documento da un messaggio e-mail di notifica dell’approvazione

A seconda delle impostazioni di notifica, è possibile che vengano inviate e-mail di notifica relative ai documenti per i quali altri utenti necessitano di una decisione di approvazione. Quando ricevi un&#39;e-mail contenente un pulsante **Decidi per l&#39;approvazione**, puoi avviare il processo di approvazione direttamente dall&#39;e-mail:

1. Dall&#39;e-mail, fai clic su **Decisione di approvazione** per aprire la pagina Dettagli documento per la bozza.
1. Per rivedere il documento, eseguire una delle operazioni seguenti:

   * Visualizzare i metadati relativi al documento.
   * Se è stata creata una bozza per la revisione del documento con commenti e commenti, fare clic su **Apri bozza** ![](assets/open-proof-icon-qs.png) nell&#39;angolo superiore destro e rivedere la bozza.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Per informazioni sulla revisione delle bozze, vedere [Verifica delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Fai clic su un&#39;opzione **Decisione** nell&#39;angolo superiore destro per approvare, approvare con modifiche o rifiutare il documento.

## Approvare un documento da una bozza {#approve-a-document-from-a-proof}

È possibile approvare un documento nel visualizzatore di bozze. Per ulteriori informazioni, vedere [Decidere su una bozza nel visualizzatore di bozze](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) nell&#39;articolo [Decidere su una bozza nel visualizzatore di bozze](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

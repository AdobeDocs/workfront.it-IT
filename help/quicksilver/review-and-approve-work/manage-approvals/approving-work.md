---
product-area: projects
navigation-topic: approvals
title: Approvazione del lavoro
description: Approvazione del lavoro
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Approvazione del lavoro

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Se sei impostato come approvatore, devi verificare regolarmente quale lavoro è in attesa di approvazione.

Per informazioni sulla creazione dei processi di approvazione, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Per informazioni sull&#39;associazione delle approvazioni con il lavoro in Workfront, vedi [Associa un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzazione o accesso superiore agli oggetti associati alle approvazioni</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti associati alle approvazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Individuare le approvazioni in Adobe Workfront

Puoi visualizzare e gestire le approvazioni in diverse aree di Workfront.

Per ulteriori informazioni sulla visualizzazione degli elementi in attesa di approvazione o degli articoli inviati per l&#39;approvazione, consulta [Visualizza approvazioni](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Approvare i lavori dall&#39;area Home

1. Fai clic sul pulsante **Pagina principale** icona ![](assets/home-icon-30x29.png) nell’angolo in alto a sinistra di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nell’ambiente:
   >
   >   
   >* Sostituiscilo con un&#39;immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con una pagina diversa. In questo caso, fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) nell’angolo superiore destro della pagina, quindi fai clic su **Pagina principale**.


1. Fai clic sul pulsante **Filtro** menu a discesa.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Seleziona **Approvazioni**.\
   Vengono visualizzati tutti gli elementi di lavoro che richiedono l&#39;approvazione. 

   >[!NOTE]
   >
   >Le approvazioni assegnate a Ruoli lavoro o Gruppi non vengono visualizzate nella home. Le approvazioni assegnate ai team vengono visualizzate nel raggruppamento di richieste team nell&#39;elenco di lavoro.

1. (Facoltativo) Modificare l&#39;ordine in cui vengono visualizzate le approvazioni, come descritto nella sezione &quot;Raggruppa e ordina per data, progetto o priorità&quot; nell&#39;articolo [Visualizza gli elementi nell&#39;elenco di lavoro nell&#39;area Home](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Selezionare l&#39;elemento in cui si desidera prendere una decisione di approvazione.

   ![](assets/task-approval-home-350x127.png)

1. Fai clic su una delle opzioni disponibili quando prendi una decisione di approvazione nel pannello a destra. Le seguenti opzioni vengono visualizzate nell’angolo superiore destro della pagina, a seconda del tipo di elemento che si sta approvando:

   * **Progetti:** Fai clic su **Approva** o **Rifiuta**.

   * **Attività:** Fai clic su **Approva** o **Rifiuta** .

   * **Problemi:** Fai clic su **Approva** o **Rifiuta** .

   * **Fogli orari:** Fai clic su **Approva** o **Rifiuta** .

   * **Documenti:** Fai clic su **Approva**, **Rifiuta** oppure **Modifiche**.\
       Quando visualizzi le approvazioni, considera quanto segue:

      * Le approvazioni delle prove vengono visualizzate qui quando un utente condivide con te una bozza, come descritto nella sezione &quot;Condividi un link di prova&quot; nell’articolo [Condividere una bozza in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Le approvazioni di correzione vengono visualizzate nell&#39;area Home solo se l&#39;ambiente Workfront è integrato con un account Workfront Proof Premium. Se non è possibile utilizzare la correzione come descritto qui, contatta il tuo amministratore Workfront.
      * Ricevi una notifica in-app che ti informa dell’approvazione della correzione.\
         Per ulteriori informazioni sulle notifiche in-app, vedi [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * Il nome dell’utente che ha richiesto l’approvazione viene visualizzato accanto all’immagine miniatura nell’area Home, con il seguente testo:\
         &quot;*Utente A* Vorrei la tua approvazione su...&quot;

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         Se il nome utente non è disponibile, viene visualizzato il testo seguente:\
         &quot;È pronta una nuova versione di una bozza da visualizzare&quot;
      * Per prendere una decisione di approvazione sulla bozza, fai clic su **Vai a prova**, fai clic su **Termina revisione**, quindi fai clic su una delle opzioni disponibili. Le opzioni disponibili per l’approvazione di una bozza sono: **Approvato**, **Approvato con modifiche**, **Modifiche richieste** e **Non pertinente**.

      * Dopo aver preso una decisione sulla bozza, la bozza rimane nella scheda Approvazioni personali con il testo &quot;Decisione presa&quot; fino a quando non si fa clic sul **Aggiorna** o fino ad aggiornare la pagina del browser.

         Per informazioni sulla revisione di una bozza, vedi [Revisione delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **Accesso:** Seleziona il livello di accesso da concedere nella **Modifica accesso** menu a discesa, quindi fai clic su **Accesso concesso**. Oppure, fai clic su **Ignora**.


## Approvare il lavoro direttamente da un progetto, un&#39;attività o un problema

Quando un progetto, un&#39;attività o un problema è in attesa di approvazione, è possibile approvare o rifiutare l&#39;approvazione direttamente dal progetto, dall&#39;attività o dal problema. Puoi anche visualizzare i dettagli relativi al processo di approvazione.

Per approvare il lavoro direttamente da un progetto, un&#39;attività o un problema:

1. Passa al progetto, all&#39;attività o al problema che richiede l&#39;approvazione dell&#39;utente.

   Le informazioni sull&#39;approvazione relative al processo di approvazione corrente di un progetto, un&#39;attività o un problema vengono visualizzate nell&#39;intestazione dell&#39;elemento.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Sono disponibili le seguenti informazioni sull’omologazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td>Lo stato corrente del progetto, dell'attività o del problema. Si tratta dello stato corrente dell'elemento in attesa dell'approvazione. Lo stato viene approvato dopo l’approvazione di ogni fase del processo di approvazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fasi di approvazione</td> 
      <td>Le fasi del processo di approvazione. <br>La fase corrente in attesa di approvazione viene visualizzata come In sospeso . Gli stadi già approvati vengono visualizzati come Approvati ; le fasi non ancora approvate vengono visualizzate come Non avviate .</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Approva** o **Rifiuta**, a seconda che si desideri approvare o rifiutare il processo di approvazione.\
   La fase di approvazione in attesa di approvazione viene ora approvata e il processo di approvazione passa alla fase successiva. Lo stato viene approvato dopo l&#39;approvazione di tutte le fasi.

## Approvare un documento direttamente da un documento 

1. Passare all&#39;area documenti contenente il documento che richiede l&#39;approvazione dell&#39;utente.
1. Selezionare il documento, quindi fare clic su **Approva**, **Modifiche** oppure **Rifiuta**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Facoltativo) Se è stata generata una bozza per il documento, è possibile approvare il documento all’interno dell’interfaccia di correzione, come descritto in [Approvare un documento da una bozza](#approve-a-document-from-a-proof).

## Approvare un documento da un&#39;e-mail di notifica di approvazione

A seconda delle impostazioni di notifica, puoi ricevere e-mail di notifica sui documenti per i quali altri utenti devono prendere una decisione di approvazione. Quando ricevi un’e-mail contenente un **Decisioni di approvazione** Puoi avviare il processo di approvazione direttamente dall’e-mail:

1. Dal messaggio e-mail, fai clic su **Decisioni di approvazione** per aprire la pagina Dettagli documento per la bozza .
1. Effettuare una delle seguenti operazioni per rivedere il documento:

   * Visualizzare i metadati del documento.
   * Se è stata creata una bozza per la revisione del documento con commenti e markup, fare clic su **Prova aperta** ![](assets/open-proof-icon-qs.png) nell’angolo in alto a destra e controlla la bozza.

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      Per informazioni sulla revisione delle bozze, consulta [Revisione delle bozze in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Fai clic su **Decisione** in alto a destra per approvare, approvare con modifiche o rifiutare il documento.

## Approvare un documento da una bozza {#approve-a-document-from-a-proof}

È possibile approvare un documento all’interno del visualizzatore di correzione. Per ulteriori informazioni, consulta [Prendere una decisione su una bozza nel visualizzatore di correzione](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) nell&#39;articolo [Prendere una decisione su una bozza nel visualizzatore di correzione](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

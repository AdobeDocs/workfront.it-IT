---
product-area: projects
navigation-topic: approvals
title: Approvazione del lavoro
description: Approvazione del lavoro
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 7366e3dd37b686a3566ca6d39e28eb6762c6d1ff
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# Approvazione del lavoro

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Se si è impostati come approvatore, è necessario verificare regolarmente il lavoro in attesa di approvazione.

Per informazioni sulla creazione dei processi di approvazione, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Per informazioni sull&#39;associazione delle approvazioni al lavoro in Workfront, vedere [Associare un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Individuare le approvazioni in Adobe Workfront

Puoi visualizzare e gestire le approvazioni in varie aree di Workfront.

Per ulteriori informazioni sulla visualizzazione degli elementi in attesa di approvazione o degli elementi inviati personalmente per l&#39;approvazione, vedere [Visualizza approvazioni](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Approva lavoro dalla sezione Home

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere il widget **Le mie approvazioni**.
1. (Condizionale) Fai clic sul menu a discesa **Filtro**, quindi seleziona **Tutti** per visualizzare le approvazioni assegnate e delegate all&#39;utente.

   >[!NOTE]
   >
   >Le approvazioni assegnate a Ruoli o Gruppi non vengono visualizzate nella Home. Le approvazioni assegnate ai team vengono visualizzate nel widget Approvazioni personali per ogni membro del team.


1. Seleziona l’elemento in cui desideri prendere una decisione di approvazione.

   ![](assets/my-approvals-widget.png)

1. Fai clic su una delle opzioni disponibili quando prendi una decisione di approvazione nel pannello a destra. Le seguenti opzioni vengono visualizzate nell&#39;angolo superiore destro della pagina, a seconda del tipo di elemento che si sta approvando:

   <table>
   <tr>
      <td>
      <p><strong>Accesso</strong></p>
      </td>
      <td>
      <p><strong>Elementi di lavoro</strong></p>
      </td>
      <td>
      <p><strong>Documenti</strong></p>
      </td>
      <td>
      <p><strong>Bozze</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Concedi</li>
      <li>Ignora</li>
      </ul>
      Se necessario, è possibile regolare il livello di accesso nel menu a discesa <b>Modifica accesso</b>.
      </td>
      <td>
         <ul>
         <li>Approvazione</li>
         <li>Rifiuta</li>
         </ul>
      Per lasciare un commento associato alla decisione, fai clic sul menu a discesa nel pulsante di decisione.
      </td>
      <td>
   Assegnato come approvatore
         <ul>
         <li>Approvazione</li>
         <li>Approva con modifiche</li>
         <li>Azioni da intraprendere</li>
         </ul>
   Assegnato come revisore
         <ul>
         <li>Completa la revisione</li>
         </ul>
      Le opzioni di questa colonna si applicano solo alle nuove approvazioni di documenti. Le approvazioni di documenti legacy vengono visualizzate come le approvazioni di elementi di lavoro. 
      </td>
      <td>
         <ul>
         <li>Vai alla bozza</li>
         </ul>
         La decisione viene presa nel visualizzatore bozze. Per informazioni sulla revisione di una bozza, vedi <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Verifica delle bozze in Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Dopo aver preso una decisione, l&#39;approvazione viene rimossa dal widget Approvazione personale.


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

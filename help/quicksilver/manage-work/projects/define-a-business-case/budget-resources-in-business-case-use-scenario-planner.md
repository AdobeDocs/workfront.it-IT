---
navigation-topic: business-case-and-scorecards
title: Risorse di budget nel caso aziendale utilizzando il Planner scenario
description: Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli di lavoro necessari per completare il lavoro in un progetto quando si crea il caso aziendale.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Risorse di budget nel caso aziendale utilizzando il Planner scenario

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli di lavoro necessari per completare il lavoro in un progetto quando si crea il caso aziendale.

Per ulteriori informazioni sulla creazione di un business case, vedi [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Le informazioni sul ruolo del lavoro per l&#39;iniziativa collegata al progetto inserito nel Planner scenario a livello di sistema sono visibili nell&#39;area Budget risorse del business case del progetto quando si pubblica l&#39;iniziativa. Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

È inoltre possibile creare un budget per le risorse nel business case utilizzando il Resource Planner. Per ulteriori informazioni, consulta quanto segue:

* [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>È consigliabile decidere se utilizzare il Planner risorse o il Planner scenario quando si inizia a lavorare a un progetto. Il passaggio frequente tra i due durante la durata del progetto può creare incongruenze nel modo in cui si preventivano le risorse per il progetto.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Aziende o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per Adobe Workfront Scenario Planner per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere Workfront Scenario Planner, consulta <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare il planner dello scenario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi: </p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
     <li> <p>Pianificazione scenario </p> </li> 
    </ul> <p>Per informazioni sull'accesso necessario alle risorse di budget, consulta anche <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Accesso necessario alle risorse di budget in Adobe Workfront</a>.</p> <p>Nota: Se non hai ancora accesso, chiedi al tuo amministratore Adobe Workfront se impostano ulteriori restrizioni nel tuo livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Creare un piano utilizzando il Planner scenario.

   Per informazioni, consulta [Creare e modificare i piani nel planner dello scenario](../../../scenario-planner/create-and-edit-plans.md).

* Crea un&#39;iniziativa sul piano e collegalo a un progetto.

   Assicurati di indicare le informazioni sui ruoli di lavoro richiesti per l&#39;iniziativa e di aggiornare il progetto collegato con queste informazioni.

   Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare e modificare le iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importare progetti in piani nel planner scenario](../../../scenario-planner/import-projects-to-plans.md)
   * [Aggiornare o creare progetti pubblicando iniziative nel Planner scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

* Anche se questi non sono prerequisiti, si consiglia anche quanto segue:

   * Assegnare le attività del progetto ai ruoli di lavoro iscritti in budget nel Planner scenario.
   * Indicare il numero di ore pianificate per le attività del progetto.

      Questo consente di comprendere la quantità di lavoro che un&#39;attività potrebbe dover completare, il che aiuta nella decisione di quanto tempo le risorse devono essere preventivate per completare l&#39;attività.

      Per informazioni sull&#39;associazione delle attività con l&#39;orario pianificato, vedere [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Risorse di budget nel caso aziendale utilizzando il Planner scenario per progetti collegati a iniziative

>[!IMPORTANT]
È possibile eseguire il budget delle risorse per un periodo di 15 anni. Se si finanziano risorse per un progetto con una durata superiore a 15 anni, le informazioni di budget potrebbero non essere precise.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Passa al progetto per il quale desideri preventivare le risorse.

   >[!TIP]
   Si tratta di un progetto collegato a un&#39;iniziativa in Scenario Planner la cui iniziativa collegata è stata pubblicata almeno una volta.

1. Fai clic su **Business case** nel pannello a sinistra.
1. (Condizionale) Nel **Budget risorse** eseguire una delle operazioni seguenti:

   * Se hai appena pubblicato informazioni dal Planner scenario, seleziona Planner scenario nel **Scegliere le ore da utilizzare per calcolare il costo del lavoro in budget del progetto** nell&#39;area Resource Budgeting, quindi fare clic su **Scegli**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Se il Planner risorse è stato selezionato in precedenza per le risorse di budget per il progetto, fare clic su **Modifica** > **Pianificazione scenario** > **Scegli**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront utilizza le ore del ruolo di lavoro richieste dall&#39;iniziativa collegata per calcolare il costo del lavoro in budget e le ore previste del progetto. Questa è l’opzione consigliata. Il costo viene visualizzato nel Business Case nella valuta del progetto.

      <!--drafted for Budgeted Hours:
   <span class="preview">Quando copi un progetto e selezioni di copiare le ore previste nel nuovo progetto, le ore previste nel budget utilizzando il planner scenario non vengono copiate nel nuovo progetto. Vengono copiate solo le ore inserite in budget nel Planner risorse. Per ulteriori informazioni, consulta [Copiare un progetto](../manage-projects/copy-project.md)</span>
-->

   >[!IMPORTANT]
   >
   >Quando si utilizza il Planner scenario per preventivare le risorse del progetto, il costo del lavoro a budget viene visualizzato nelle seguenti aree di Workfront:
   >
   >* Area Budget risorse del Business Case
   >* La pianificazione dello scenario a livello di sistema come costo delle persone dell&#39;iniziativa collegata al progetto. Per ulteriori informazioni, consulta [Creare e modificare le iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Facoltativo) Fai clic su **Visualizza in planner scenario** aprire il piano che contiene l&#39;iniziativa collegata al progetto. Verrà visualizzata la finestra di pianificazione dello scenario in una nuova scheda del browser.
1. (Facoltativo) Aggiorna le informazioni sull&#39;iniziativa. Per ulteriori informazioni, consulta [Creare e modificare le iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >È necessario pubblicare l&#39;iniziativa dopo ogni modifica per l&#39;area Resource Budgeting del progetto da aggiornare.

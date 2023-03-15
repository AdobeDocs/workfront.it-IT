---
navigation-topic: business-case-and-scorecards
title: Risorse di budget nel Business Case utilizzando il Resource Planner
description: Come parte della pianificazione delle risorse, è possibile utilizzare il Planner risorse a livello di progetto per creare il budget dei ruoli di lavoro necessari per completare il lavoro in un progetto quando si crea il caso aziendale.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# Risorse di budget nel Business Case utilizzando il Resource Planner

Come parte della pianificazione delle risorse, è possibile utilizzare il Planner risorse a livello di progetto per creare il budget dei ruoli di lavoro necessari per completare il lavoro in un progetto quando si crea il caso aziendale.

Per ulteriori informazioni sulla creazione di un business case, vedi [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Le informazioni immesse nel Planner risorse a livello di progetto sono visibili anche nel Planner risorse a livello di sistema. Anche il contrario è vero. Per informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

È inoltre possibile preventivare le risorse nel business case utilizzando Adobe Workfront Scenario Planner. Per ulteriori informazioni, consulta [Risorse di budget nel caso aziendale utilizzando il Planner scenario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a>*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>*</td> 
   <td> <p>Revisione o superiore</p> <p>Importante: Per modificare le informazioni di budget delle risorse, è necessario disporre di una licenza Plan. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi: </p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
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

* Soddisfa tutti i prerequisiti per la pianificazione delle risorse in Adobe Workfront. Per informazioni, consulta [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associa pool di risorse al progetto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Non è possibile assegnare risorse di budget a problemi nel Business Case. È possibile eseguire il budget in planner risorse a livello di sistema. Per ulteriori informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Anche se questo non è un prerequisito, ti consigliamo anche di indicare Orari pianificati per le attività sul progetto. Questo ti aiuta a capire la quantità di lavoro che un&#39;attività potrebbe dover completare, il che aiuta con la decisione di molto tempo le risorse devono essere preventivate per completare l&#39;attività. Per informazioni sull&#39;associazione delle attività con l&#39;orario pianificato, vedere [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Applicare i pool di risorse a un progetto e alle risorse di budget nel Business Case

>[!IMPORTANT]
È possibile eseguire il budget delle risorse per un periodo di 15 anni. Se si finanziano risorse per un progetto con una durata superiore a 15 anni, le informazioni di budget potrebbero non essere precise.

Per applicare i pool di risorse e le risorse del progetto di budget nel Business Case per un progetto senza pool di risorse:

1. Passa al progetto per il quale desideri preventivare le risorse.
1. Fai clic su **Business case** nel pannello a sinistra.
1. (Condizionale) Se l&#39;azienda non dispone di una licenza per Workfront Scenario Planner, fai clic su **Modifica budget risorse** in **Budget risorse** , quindi continua con il passaggio 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Facoltativo e condizionale) Se le informazioni sul progetto sono state pubblicate da un&#39;iniziativa nel Planner scenario, effettuare una delle seguenti operazioni:

   * Seleziona il Planner risorse nel **Scegliere le ore da utilizzare per calcolare il costo del lavoro in budget del progetto** campo , quindi fai clic su **Scegli > Modifica budget risorse**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Se è stato selezionato Planner scenario per le risorse di budget per il progetto, fare clic su **Modifica** > **Modifica budget risorse**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   In questo modo viene utilizzato l&#39;orario previsto del progetto per calcolare il costo del lavoro a budget per il progetto.

   Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   È consigliabile decidere se utilizzare il Planner risorse o il Planner scenario quando si inizia a lavorare a un progetto. Il passaggio frequente tra i due durante la durata del progetto può creare incongruenze nel modo in cui si preventivano le risorse per il progetto.

1. In **Seleziona pool di risorse** campo , specifica uno o più **Pool di risorse**.

   È necessario specificare solo i pool di risorse compilati con utenti attivi.

   >[!TIP]
   Se il progetto è già associato ai pool di risorse, viene visualizzato il Planner risorse per impostazione predefinita. Per aggiungere altri pool di risorse al progetto, modifica il progetto. Per informazioni sulla modifica di un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Applica**.

   Viene visualizzato il Planner risorse per il progetto selezionato.

   Per impostazione predefinita, i primi 20 ruoli di lavoro associati a questo progetto sono elencati in ordine alfabetico nella sezione Resource Budgeting. 

   Per ulteriori informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Facoltativo e condizionale) Espandi i ruoli di lavoro per visualizzare gli utenti associati ad essi.

   >[!NOTE]
   Gli utenti attivi vengono visualizzati sotto i ruoli di lavoro associati solo se soddisfano i seguenti criteri:
   * Appartengono a uno dei pool di risorse del progetto.
   * Hanno assegnato loro delle ore a budget.
   * Sono associati a uno dei ruoli di lavoro del progetto.


    

1. Fai clic su **Oggi** per tornare all&#39;attuale calendario.
1. (Facoltativo) Fai clic su **Settimana**, **Mese** o **Trimestre** per visualizzare le informazioni relative al progetto in diversi intervalli di tempo.
1. (Facoltativo) Fai clic sul pulsante **Ore** menu a discesa e seleziona **Ore**,**FTE** oppure **Costo** per modificare la modalità di visualizzazione delle informazioni nel Planner risorse. Le ore vengono visualizzate per impostazione predefinita.

1. (Facoltativo) Fai clic su **Esporta** per esportare il planner risorse in un file Excel.

   >[!NOTE]
   Puoi esportare dati per un massimo di 12 periodi di tempo alla volta.

1. (Facoltativo) Fai clic sul pulsante **Schermo intero** icona ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) per visualizzare il planner risorse in modalità a schermo intero.

1. Aggiorna **BDG** Campo (Ore in budget) con valori Ora, FTE o Costo per gli utenti, i ruoli o il progetto, eseguendo una delle operazioni seguenti:

   * Stimare manualmente la quantità di valori Ore, FTE o Costo per ruoli, utenti o progetto.

      Oppure

   * Fai clic sul pulsante **Opzioni** icona per il progetto o i ruoli del processo e selezionare un&#39;opzione per eseguire automaticamente il budget delle ore per ruoli, utenti o progetto.
   Per ulteriori informazioni sull&#39;impostazione del budget nella visualizzazione Progetto del Planner risorse, vedere [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   È possibile calcolare il budget di ore, FTE o costi per le risorse per qualsiasi intervallo di tempo visualizzato nell&#39;area Resource Budgeting, indipendentemente dalla timeline del progetto. Ad esempio, se desideri indicare che le risorse potrebbero non essere disponibili durante la cronologia del progetto (dove sono associate all’orario pianificato), ma potrebbero essere disponibili in un altro momento, puoi farlo inserendole nel budget per i frame di tempo in cui l’ora pianificata è zero, se questo è il momento in cui diventano disponibili per il lavoro.

1. (Facoltativo) Per capire se è possibile spostare gli orari, gli FTE o i costi preventivati in un altro intervallo di tempo, fai clic sul pulsante **Opzioni** icona, quindi **Adeguamento date budget**.

   Per ulteriori informazioni sulla regolazione delle date in budget, consulta [Adeguare le date di budget nel Planner risorse](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Fai clic su **Salva**.

   Se i tassi di costo per ora sono associati ai ruoli di lavoro, l&#39;impostazione del budget delle risorse nell&#39;area di budget risorse calcola il **Costo manodopera a budget** del progetto. Il costo del lavoro a budget viene visualizzato nell&#39;area Budget risorse del Business Case e nel sintetico del Business Case.

   >[!TIP]
   Il costo viene visualizzato nel Business Case nella valuta del progetto.

   Le informazioni di budget specificate nel Business Case vengono visualizzate anche nel Resource Planner.

   Quando copi un progetto, puoi anche copiare le ore previste nel nuovo progetto. Vengono copiate solo le ore inserite in budget nel Planner risorse. Per ulteriori informazioni, consulta [Copiare un progetto](../manage-projects/copy-project.md).

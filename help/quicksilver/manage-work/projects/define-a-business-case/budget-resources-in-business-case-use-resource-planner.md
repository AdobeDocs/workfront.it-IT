---
navigation-topic: business-case-and-scorecards
title: Preventivare le risorse nel Business Case utilizzando la Programmazione delle risorse
description: Come parte della pianificazione delle risorse, è possibile utilizzare la Pianificazione risorse a livello di progetto per preventivare i ruoli necessari per il completamento del lavoro in un progetto quando si crea il caso di business.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f1d235a21dcf939570d4d93f08f31865eab42803
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 0%

---

# Preventivare le risorse nel Business Case utilizzando la Programmazione delle risorse

<!--Audited: 01/2025-->

Come parte della pianificazione delle risorse, è possibile utilizzare la Pianificazione risorse a livello di progetto per preventivare i ruoli necessari per il completamento del lavoro in un progetto quando si crea il caso di business.

Per ulteriori informazioni sulla creazione di un caso di business, vedere [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Le informazioni immesse nella Programmazione risorse a livello di progetto sono visibili anche nella Programmazione risorse a livello di sistema. Anche il contrario è vero. Per informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Puoi anche preventivare le risorse nel caso di business utilizzando Adobe Workfront Scenario Planner. Per ulteriori informazioni, vedere [Risorse budget nel caso di business utilizzando la Pianificazione scenario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Prime o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Chiaro o superiore</p>
   <p>Corrente: revisione o versione successiva</p>

<p><b>IMPORTANTE:</b></p> 
   <p>Nuovo: è necessario disporre di una licenza Standard per modificare le informazioni di budgeting delle risorse. </p> 
   <p>Corrente: è necessario disporre di una licenza Pianificazione per modificare le informazioni di budgeting delle risorse. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a: </p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Soddisfa tutti i prerequisiti per la pianificazione delle risorse in Adobe Workfront. Per informazioni, vedere [Panoramica di Programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associa i gruppi di risorse al progetto.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >Non è possibile preventivare le risorse assegnate ai problemi nel Business Case. È possibile preventivarli nella programmazione delle risorse a livello di sistema. Per ulteriori informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Anche se questo non è un prerequisito, ti consigliamo anche di indicare le Ore pianificate per le attività sul progetto. In questo modo è possibile comprendere la quantità di lavoro che un&#39;attività potrebbe dover completare, il che consente di decidere in merito alla quantità di tempo a cui le risorse devono essere preventivate per completare l&#39;attività. Per informazioni sull&#39;associazione delle attività alle ore pianificate, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Applicare gruppi di risorse a un progetto e risorse preventivo nel Business Case

>[!IMPORTANT]
>
>È possibile preventivare le risorse per un periodo di 15 anni. Se si preventivano le risorse per un progetto con una durata superiore a 15 anni, le informazioni di definizione del budget potrebbero non essere accurate.

Per applicare i gruppi di risorse e le risorse del progetto di budget nel Business Case per un progetto senza gruppo di risorse:

1. Vai al progetto per il quale vuoi preventivare le risorse.
1. Fai clic su **Business Case** nel pannello a sinistra.
1. (Condizionale) Se la società non dispone di una licenza per Workfront Scenario Planner, fai clic su **Modifica budget risorse** nella sezione **Budget risorse**, quindi continua con il passaggio 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Facoltativo e condizionale) Se le informazioni sul progetto sono state pubblicate da un&#39;iniziativa nella Pianificazione scenario, effettuate una delle seguenti operazioni:

   * Selezionare Pianificazione risorse nel campo **Scegliere le ore da utilizzare per calcolare il costo manodopera preventivato del progetto**, quindi fare clic su **Scegli > Modifica budget risorse**.

     ![Caso di business in Pianificazione risorse](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Se la Pianificazione scenario è stata selezionata per la definizione del budget delle risorse per il progetto, fare clic su **Modifica** > **Modifica budget risorse**.

     ![Caso di business in Scenario Planner](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   In questo modo vengono utilizzate le ore preventivate del progetto per calcolare il costo manodopera preventivato per il progetto.

   La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   >
   >È consigliabile decidere se utilizzare la Programmazione risorse o la Pianificazione scenario quando si inizia a lavorare su un progetto. Il passaggio frequente tra le due opzioni durante il ciclo di vita del progetto può creare incongruenze nel modo in cui vengono preventivate le risorse per il progetto.

1. Nel campo **Seleziona pool di risorse**, specificare uno o più **pool di risorse**.

   È necessario specificare solo i gruppi di risorse popolati con utenti attivi.

   >[!TIP]
   >
   >Se il progetto è già associato ai gruppi di risorse, per impostazione predefinita viene visualizzato Pianificazione risorse. Per aggiungere altri gruppi di risorse al progetto, modifica il progetto. Per informazioni sulla modifica di un progetto, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fare clic su **Applica**.

   Viene visualizzata la Programmazione delle risorse per il progetto selezionato.

   Per impostazione predefinita, i primi 20 ruoli associati a questo progetto sono elencati in ordine alfabetico nella sezione Budget risorse. 

   Per ulteriori informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Facoltativo e condizionale) Espandere i ruoli per visualizzare gli utenti associati.

   >[!NOTE]
   >
   >Gli utenti attivi vengono visualizzati nelle mansioni loro associate solo se soddisfano i seguenti criteri:
   >
   >   
   >   
   >   * Appartengono a uno dei Pool di Risorse del progetto.
   >   * Sono state assegnate ore preventivate.
   >   * Sono associati a una delle mansioni del progetto.
   >   
   >

    

1. Fai clic su **Oggi** per tornare all&#39;intervallo di tempo odierno.
1. (Facoltativo) Fai clic su **Settimana**, **Mese** o **Trimestre** per visualizzare le informazioni per il progetto in diversi intervalli di tempo.
1. (Facoltativo) Fai clic sul menu a discesa **Ore** e seleziona **Ore**,**FTE** o **Costo** per modificare la modalità di visualizzazione delle informazioni nella Programmazione delle risorse. Le ore vengono visualizzate per impostazione predefinita.

1. (Facoltativo) Fai clic su **Esporta** per esportare la Programmazione delle risorse in un file Excel.

   >[!NOTE]
   >
   >Puoi esportare dati per un massimo di 12 periodi di tempo alla volta.

1. (Facoltativo) Fai clic sull&#39;icona **Schermo intero** ![schermo intero_RP_in_BC.png](assets/full-screen-rp-in-bc.png) per visualizzare la Programmazione delle risorse in modalità a schermo intero.

1. Aggiornare il campo **BDG** (Ore preventivate) con i valori di Ora, FTE o Costo per gli utenti, i ruoli o il progetto eseguendo una delle operazioni seguenti:

   * Stimare manualmente la quantità di ore, FTE o valori di costo per ruoli, utenti o progetto.

     Oppure

   * Fai clic sull&#39;icona **Opzioni** per il progetto o le mansioni e seleziona un&#39;opzione per preventivare automaticamente le ore per ruoli, utenti o progetto.

   Per ulteriori informazioni sull&#39;impostazione del budget nella visualizzazione Progetto della Programmazione delle risorse, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   >
   >È possibile preventivare ore, FTE o costi per le risorse per qualsiasi intervallo di tempo visualizzato nell&#39;area Budget risorse, indipendentemente dalla sequenza temporale del progetto. Ad esempio, se vuoi indicare che le risorse potrebbero non essere disponibili durante la timeline del progetto (dove sono associate alle ore pianificate), ma potrebbero essere disponibili in un altro momento, puoi preventivarle per intervalli di tempo in cui le ore pianificate sono zero, se questo è il momento in cui diventano disponibili per lavorare.

1. (Facoltativo) Per capire se è possibile spostare le ore, gli FTE o i costi preventivati in un altro intervallo di tempo, fai clic sull&#39;icona **Opzioni**, quindi **Adegua date budget**.

   Per ulteriori informazioni sull&#39;adeguamento delle date preventivate, vedere [Adeguare le date preventivate in Pianificazione risorse](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Fai clic su **Salva**.

   Se alle mansioni sono associate tariffe Costo orario, la definizione del budget delle risorse nell&#39;area Budget risorse calcola il **Costo manodopera preventivato** del progetto. Il Costo manodopera preventivato viene visualizzato nell&#39;area Budget risorse del Business Case e nel Sintetico Business Case.

   >[!TIP]
   >
   >Nel Business Case, il costo viene visualizzato nella valuta del progetto.

   Le informazioni di budget specificate nel Business Case vengono visualizzate anche nella Programmazione delle risorse.

   Quando copi un progetto, puoi anche copiare le ore preventivate nel nuovo progetto. Vengono copiate solo le ore preventivate nella Programmazione delle risorse. Per ulteriori informazioni, vedere [Copiare un progetto](../manage-projects/copy-project.md).

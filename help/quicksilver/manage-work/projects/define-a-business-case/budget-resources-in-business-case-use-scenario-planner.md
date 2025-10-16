---
navigation-topic: business-case-and-scorecards
title: Preventivare le risorse nel Business Case utilizzando la Pianificazione scenario
description: Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli necessari per il completamento del lavoro in un progetto al momento della creazione del business case.
author: Becky
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: fa0b4322b9f7c1d506cf194645c7ae50ad8c0f0b
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 1%

---

# Preventivare le risorse nel Business Case utilizzando la Pianificazione scenario

<!--Audited: 06/2025-->

Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli necessari per il completamento del lavoro in un progetto al momento della creazione del business case.

Per ulteriori informazioni sulla creazione di un caso di business, vedere [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Le informazioni sulla mansione per l&#39;iniziativa collegata al progetto immesse nella Programmazione scenario a livello di sistema sono visibili nell&#39;area Budget risorse del business case del progetto quando si pubblica l&#39;iniziativa. La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

È inoltre possibile preventivare le risorse nel business case utilizzando la pianificazione risorse. Per ulteriori informazioni vedi quanto segue:

* [Risorse budget nel caso di business](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>È consigliabile decidere se utilizzare la Programmazione risorse o la Pianificazione scenario quando si inizia a lavorare su un progetto. Il passaggio frequente tra le due opzioni durante il ciclo di vita del progetto può creare incongruenze nel modo in cui vengono preventivate le risorse per il progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td><p>Prime o versione successiva</p> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p>Chiaro o superiore 
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Prodotto</p></td> 
   <td><p>La Pianificazione scenario è inclusa nel piano Ultimate Workfront corrente.</p> 
   <p>Per i piani Workfront precedenti, è necessario acquistare una licenza per Adobe Workfront Scenario Planner, oltre alla licenza Workfront, per accedere alle funzionalità descritte in questo articolo.</p> <p>Per informazioni su come ottenere Workfront Scenario Planner, vedere <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td> <p>Modifica accesso a: </p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
     <li> <p>Pianificazione scenario </p> </li> 
    </ul> <p>Per informazioni sull'accesso necessario alle risorse del budget, vedere anche <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Accesso necessario alle risorse del budget in Adobe Workfront</a>.</p> <p>Nota: se ancora non disponi dell’accesso, chiedi all’amministratore di Adobe Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Gestire le autorizzazioni sul progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Creare un piano utilizzando la Pianificazione scenario.

  Per informazioni, vedere [Creare e modificare i piani nella Pianificazione scenario](../../../scenario-planner/create-and-edit-plans.md).

* Crea un’iniziativa sul piano e collegala a un progetto.

  Assicurati di indicare le informazioni sulle mansioni richieste per l’iniziativa e di aggiornare il progetto collegato con tali informazioni.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Crea e modifica iniziative nella Pianificazione scenario](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importa progetti nei piani nella Pianificazione scenario](../../../scenario-planner/import-projects-to-plans.md)
   * [Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

* Anche se questi non sono prerequisiti, consigliamo anche quanto segue:

   * Assegnare le attività del progetto alle mansioni preventivate nella Pianificazione scenario.
   * Indica il numero di ore pianificate per le attività del progetto.

     In questo modo è possibile comprendere la quantità di lavoro che un&#39;attività potrebbe dover completare, il che consente di decidere il tempo necessario per la pianificazione delle risorse per completare l&#39;attività.

     Per informazioni sull&#39;associazione delle attività alle ore pianificate, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Preventivare le risorse nel caso di business utilizzando Scenario Planner per i progetti collegati alle iniziative

>[!IMPORTANT]
>
>È possibile preventivare le risorse per un periodo di 15 anni. Se si preventivano le risorse per un progetto con una durata superiore a 15 anni, le informazioni di definizione del budget potrebbero non essere accurate.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. Vai al progetto per il quale vuoi preventivare le risorse.

   >[!TIP]
   >
   >Si tratta di un progetto collegato a un’iniziativa nella Pianificazione scenario la cui iniziativa collegata è stata pubblicata almeno una volta.

1. Fai clic su **Business Case** nel pannello a sinistra.
1. (Condizionale) Nella sezione **Budget risorse** eseguire una delle operazioni seguenti:

   * Se hai appena pubblicato le informazioni dalla Pianificazione scenario, seleziona Pianificazione scenario in **Scegli le ore da utilizzare per calcolare il costo della manodopera preventivato del progetto** nel campo Budget risorse, quindi fai clic su **Scegli**.

     <!--![Business case in Resource Planner with Choose button](assets/business-case-sp-selected-with-choose-button-350x121.png)-->

   * Se la Programmazione delle risorse è stata precedentemente selezionata per la definizione del budget delle risorse per il progetto, fare clic su **Modifica** > **Pianificazione scenario** > **Scegli**.

     ![Caso di business in Scenario Planner con pulsante Scegli](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront utilizza le ore ruolo richieste dall&#39;iniziativa collegata per calcolare il costo manodopera preventivato e le ore preventivate del progetto. Questa è l’opzione consigliata. Nel Business Case, il costo viene visualizzato nella valuta del progetto.

     Quando si copia un progetto e si seleziona di copiare le ore preventivate nel nuovo progetto, le ore preventivate utilizzando la Pianificazione scenario non vengono copiate nel nuovo progetto. Vengono copiate solo le ore preventivate nella Programmazione delle risorse. Per ulteriori informazioni, vedere [Copiare un progetto](../manage-projects/copy-project.md).

     >[!IMPORTANT]
     >
     >Quando si utilizza la Pianificazione scenario per preventivare le risorse per il progetto, il Costo manodopera preventivato viene visualizzato nelle seguenti aree di Workfront:
     >
     >   
     >   
     >   * Area Budget risorse del Business Case
     >   * Pianificazione scenario a livello di sistema come costo persone dell’iniziativa collegata al progetto. Per ulteriori informazioni, consulta [Creare e modificare iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).
     >   
     >

1. (Facoltativo) Fai clic su **Visualizza in Scenario Planner** per aprire il piano contenente l&#39;iniziativa collegata al progetto. Verrà aperta la finestra Pianificazione scenario in una nuova scheda del browser.
1. (Facoltativo) Aggiornare le informazioni sull’iniziativa. Per ulteriori informazioni, consulta [Creare e modificare iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >È necessario pubblicare l&#39;iniziativa dopo ogni modifica per l&#39;area Budget risorse del progetto da aggiornare.

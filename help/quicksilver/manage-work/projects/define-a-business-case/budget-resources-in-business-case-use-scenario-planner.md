---
navigation-topic: business-case-and-scorecards
title: Preventivare le risorse nel Business Case utilizzando la Pianificazione scenario
description: Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli necessari per il completamento del lavoro in un progetto al momento della creazione del business case.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Preventivare le risorse nel Business Case utilizzando la Pianificazione scenario

Come parte della pianificazione delle risorse, è possibile utilizzare Adobe Workfront Scenario Planner per preventivare i ruoli necessari per il completamento del lavoro in un progetto al momento della creazione del business case.

Per ulteriori informazioni sulla creazione di un caso di business, consulta [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Le informazioni sulla mansione per l&#39;iniziativa collegata al progetto immesse nella Programmazione scenario a livello di sistema sono visibili nell&#39;area Budget risorse del business case del progetto quando si pubblica l&#39;iniziativa. La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta [Panoramica sulla pianificazione degli scenari](../../../scenario-planner/scenario-planner-overview.md).

È inoltre possibile preventivare le risorse nel business case utilizzando la pianificazione risorse. Per ulteriori informazioni, vedi:

* [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>È consigliabile decidere se utilizzare la Programmazione risorse o la Pianificazione scenario quando si inizia a lavorare su un progetto. Il passaggio frequente tra le due opzioni durante il ciclo di vita del progetto può creare incongruenze nel modo in cui vengono preventivate le risorse per il progetto.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Business o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per Adobe Workfront Scenario Planner per accedere alle funzionalità descritte in questo articolo.</p> <p>Per informazioni su come ottenere Workfront Scenario Planner, consulta <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare la Pianificazione scenario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a: </p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Dati finanziari</p> </li> 
     <li> <p>Pianificazione scenario </p> </li> 
    </ul> <p>Per informazioni sull'accesso necessario alle risorse del budget, vedere anche <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Accesso necessario per preventivare le risorse in Adobe Workfront</a>.</p> <p>Nota: se ancora non disponi dell’accesso, chiedi all’amministratore di Adobe Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Creare un piano utilizzando la Pianificazione scenario.

   Per informazioni, consulta [Creare e modificare i piani nella Pianificazione scenario](../../../scenario-planner/create-and-edit-plans.md).

* Crea un’iniziativa sul piano e collegala a un progetto.

   Assicurati di indicare le informazioni sulle mansioni richieste per l’iniziativa e di aggiornare il progetto collegato con tali informazioni.

   Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare e modificare iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importare progetti nei piani nella Pianificazione scenario](../../../scenario-planner/import-projects-to-plans.md)
   * [Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

* Anche se questi non sono prerequisiti, consigliamo anche quanto segue:

   * Assegnare le attività del progetto alle mansioni preventivate nella Pianificazione scenario.
   * Indica il numero di ore pianificate per le attività del progetto.

      In questo modo è possibile comprendere la quantità di lavoro che un&#39;attività potrebbe dover completare, il che consente di decidere il tempo necessario per la pianificazione delle risorse per completare l&#39;attività.

      Per informazioni sull&#39;associazione delle attività alle ore pianificate, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Preventivare le risorse nel caso di business utilizzando Scenario Planner per i progetti collegati alle iniziative

>[!IMPORTANT]
È possibile preventivare le risorse per un periodo di 15 anni. Se si preventivano le risorse per un progetto con una durata superiore a 15 anni, le informazioni di definizione del budget potrebbero non essere accurate.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Vai al progetto per il quale vuoi preventivare le risorse.

   >[!TIP]
   Si tratta di un progetto collegato a un’iniziativa nella Pianificazione scenario la cui iniziativa collegata è stata pubblicata almeno una volta.

1. Clic **Business Case** nel pannello a sinistra.
1. (Condizionale) In **Budget risorse** eseguire una delle operazioni seguenti:

   * Se hai appena pubblicato informazioni da Pianificazione scenario, seleziona Pianificazione scenario in **Scegliere le ore da utilizzare per calcolare il costo manodopera preventivato del progetto** nell&#39;area Budget risorse, quindi fare clic su **Scegli**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Se la Pianificazione risorse è stata precedentemente selezionata per la definizione del budget delle risorse per il progetto, fare clic su **Cambia** > **Pianificazione scenario** > **Scegli**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront utilizza le ore ruolo richieste dall&#39;iniziativa collegata per calcolare il costo manodopera preventivato e le ore preventivate del progetto. Questa è l’opzione consigliata. Nel Business Case, il costo viene visualizzato nella valuta del progetto.

      Quando si copia un progetto e si seleziona di copiare le ore preventivate nel nuovo progetto, le ore preventivate utilizzando la Pianificazione scenario non vengono copiate nel nuovo progetto. Vengono copiate solo le ore preventivate nella Programmazione delle risorse. Per ulteriori informazioni, consulta [Copiare un progetto](../manage-projects/copy-project.md).

      >[!IMPORTANT]
      Quando si utilizza la Pianificazione scenario per preventivare le risorse per il progetto, il Costo manodopera preventivato viene visualizzato nelle seguenti aree di Workfront:
      * Area Budget risorse del Business Case
      * Pianificazione scenario a livello di sistema come costo persone dell’iniziativa collegata al progetto. Per ulteriori informazioni, consulta [Creare e modificare iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Facoltativo) Fai clic su **Visualizza in Pianificazione scenario** per aprire il piano contenente l’iniziativa collegata al progetto. Verrà aperta la finestra Pianificazione scenario in una nuova scheda del browser.
1. (Facoltativo) Aggiornare le informazioni sull’iniziativa. Per ulteriori informazioni, consulta [Creare e modificare iniziative in Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   È necessario pubblicare l&#39;iniziativa dopo ogni modifica per l&#39;area Budget risorse del progetto da aggiornare.

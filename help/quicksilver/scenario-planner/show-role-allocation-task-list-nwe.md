---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra allocazione ruoli per progetti e iniziative nell'elenco dei task
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che corrisponda. In questo modo si evita di sovrassegnarle o sottoutilizzarle.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Mostra assegnazione ruoli per progetti e iniziative nell&#39;elenco delle attività

<!--Audited: 07/2024-->

Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che corrisponda. In questo modo si evita di sovrassegnarle o sottoutilizzarle.

Questo articolo descrive come riconciliare le risorse utilizzando il pannello [!UICONTROL Allocazione ruoli] nell&#39;elenco delle attività di un progetto.

Per informazioni generali sulla riconciliazione delle risorse tra progetti e iniziative, inclusi i prerequisiti, vedere [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] pacchetto</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Se hai un pacchetto Workfront diverso, contatta il rappresentante Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Light] o versione successiva</p> 
   <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
    <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore ai progetti.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p> Visualizza o autorizzazioni superiori per un progetto.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sull&#39;accesso alla Pianificazione scenario, vedere [Accesso necessario per utilizzare la [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Per informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Mostra assegnazione ruoli per progetti e iniziative nell&#39;elenco delle attività

Se la società ha acquistato una licenza di [!DNL Workfront Scenario Planner], è possibile riconciliare le allocazioni di risorse tra l&#39;iniziativa e il progetto ad essa collegato nella sezione [!UICONTROL Attività] del progetto.

1. (Facoltativo) Un progetto deve essere connesso a un&#39;iniziativa utilizzando uno dei metodi descritti nella sezione [Mostra allocazione ruoli per progetti e iniziative nell&#39;elenco attività](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) di questo articolo.

   >[!IMPORTANT]
   >
   >Se apporti modifiche alle risorse dell’iniziativa, devi ripubblicare lo scenario a cui appartiene l’iniziativa per ottenere le informazioni più recenti sulle risorse dell’iniziativa da aggiornare sul progetto.

1. Vai al progetto in cui desideri rivedere l’allocazione delle mansioni per il progetto e per l’iniziativa associata.
1. Fai clic su **[!UICONTROL Attività]** nel pannello a sinistra.
1. Fai clic sull&#39;icona **[!UICONTROL Mostra allocazione ruoli]** ![Mostra allocazione ruoli](assets/show-role-allocation-icon.png) nell&#39;angolo superiore destro della barra degli strumenti.

   Viene visualizzato il pannello [!UICONTROL Allocazione ruoli].

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Rivedi le seguenti informazioni nell&#39;area **[!UICONTROL Totali progetto]** del pannello [!UICONTROL Allocazione ruoli]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ruolo]</td> 
      <td> <p>I nomi dei ruoli associati a uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>attività sul progetto</p> </li> 
        <li> <p>problemi relativi al progetto</p> </li> 
        <li> <p>iniziativa collegata al progetto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Il numero di ore richieste associate a ogni ruolo nell'iniziativa per la durata totale dell'iniziativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Lavoro Necessario]</td> 
      <td>Il numero di ore pianificate associate a ogni mansione nelle attività o nei problemi sul progetto per la durata totale del progetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Differenza tra le ore necessarie per l'iniziativa e le ore pianificate associate al lavoro sul progetto. [!DNL Workfront] calcola la varianza [!UICONTROL] utilizzando questa formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando le risorse sono pianificate per più ore rispetto a quelle richieste per l'iniziativa, la [!UICONTROL Variance] è negativa e viene visualizzata in rosso. Ciò significa che le risorse sono sovrassegnate. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Le ore pianificate del progetto non vengono visualizzate nei seguenti scenari:
   >
   >   
   >   
   >   * Quando le attività o i problemi non vengono assegnati a mansioni o agli utenti a cui sono associate delle mansioni.
   >   * Quando le attività o i problemi hanno una durata pari a zero.
   >   
   >



1. (Facoltativo) Se la colonna [!UICONTROL Varianza] indica che le risorse sono sovrassegnate, regola una delle seguenti opzioni:

   * Ridurre il numero di ore pianificate per una mansione che mostra le risorse sovrassegnate o aggiungere più risorse alle attività e distribuire più ore pianificate alle nuove risorse. È possibile aggiornare le assegnazioni o il numero di ore pianificate per le attività o i problemi durante la modifica. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Modifica attività](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifica problemi](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Per modificare attività e problemi è necessario disporre di autorizzazioni e diritti di accesso aggiuntivi.

   * Aumenta il numero di ore richieste per il ruolo che mostra la sovrassegnazione nell’iniziativa. Per ulteriori informazioni, vedere [Creare e modificare le iniziative in [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Per modificare i piani è necessario disporre di autorizzazioni e di accesso aggiuntivi.



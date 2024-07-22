---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra l’allocazione dei ruoli per progetti e iniziative nel Bilanciatore dei carichi di lavoro
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# Mostra allocazione ruoli per progetti e iniziative nel [!UICONTROL Bilanciatore dei carichi di lavoro]

<!--Audited: 07/2024-->

Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che corrisponda. In questo modo si evita di sovrassegnarle o sottoutilizzarle.

Questo articolo descrive come riconciliare le risorse utilizzando il pannello [!UICONTROL Allocazione ruoli] nel [!UICONTROL Bilanciatore dei carichi di lavoro] di un progetto.

Per informazioni generali sulla riconciliazione delle risorse tra progetti e iniziative, inclusi i prerequisiti, vedere [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <p>Corrente: [!UICONTROL Business] o versione successiva</p>
   <p>Nuovo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> 
   <p>Per i piani Workfront correnti: </p>
   <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni sull'accesso e sulle autorizzazioni per [!DNL Workfront Scenario Planner], vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a [!UICONTROL Projects]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] per un progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostra allocazione ruoli per progetti e iniziative nel [!UICONTROL Bilanciatore dei carichi di lavoro]

Se la società ha acquistato una licenza [!DNL Workfront Scenario Planner], è possibile riconciliare le allocazioni di risorse tra l&#39;iniziativa e il progetto ad essa collegato nel [!UICONTROL Bilanciatore dei carichi di lavoro] a livello di progetto.

1. (Condizionale) Collega un progetto a un’iniziativa utilizzando uno dei metodi descritti nei seguenti articoli:

   * [Importa i progetti nei piani in [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Aggiorna o crea progetti pubblicando iniziative in [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Se apporti modifiche alle risorse dell’iniziativa, devi ripubblicare lo scenario a cui appartiene l’iniziativa per ottenere le informazioni più recenti sulle risorse dell’iniziativa da aggiornare sul progetto.

1. Vai al progetto in cui desideri rivedere l’allocazione delle mansioni per il progetto e per l’iniziativa associata.
1. Fai clic su [!UICONTROL Bilanciatore dei carichi di lavoro] nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **[!UICONTROL Pianificazione]**, quindi su **[!UICONTROL Passa al Bilanciatore dei carichi di lavoro]**.

1. Esegui una delle operazioni seguenti:

   * Fai clic su **[!UICONTROL Mese]** per visualizzare il Bilanciatore dei carichi di lavoro per mese, fai clic sul menu a discesa accanto a un mese nella timeline ![](assets/drop-down-next-to-month-month-view-wb.png), quindi fai clic su **[!UICONTROL Altro]**.
   * Fai clic sull&#39;icona ![](assets/show-role-allocation-icon.png) **[!UICONTROL Mostra allocazione ruoli]** nell&#39;angolo superiore destro della barra degli strumenti.

   Viene visualizzato il pannello [!UICONTROL Allocazione ruoli].

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Anche se è possibile visualizzare il pannello [!UICONTROL Allocazione ruoli] anche se la tua organizzazione non ha acquistato una licenza di [!DNL Workfront Scenario Planner], non è possibile visualizzare informazioni sulle mansioni delle iniziative.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Rivedi le seguenti informazioni nell&#39;area **[!UICONTROL Totali progetto]** del pannello Allocazione ruoli:

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
   >   * Quando le attività o i problemi hanno una [!UICONTROL Durata] pari a zero.
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

1. (Facoltativo) Fai clic sull&#39;icona a discesa per espandere uno dei mesi nel pannello [!UICONTROL Allocazione ruoli] o nella timeline del [!UICONTROL Bilanciatore dei carichi di lavoro].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Lo stesso tipo di informazioni visualizzate nell&#39;area [!UICONTROL Totali progetto] viene visualizzato anche per ogni mese.

   >[!TIP]
   >
   >I mesi elencati nel pannello [!UICONTROL Allocazione ruoli] sono i mesi nella timeline visualizzati sullo schermo nel [!UICONTROL Bilanciatore dei carichi di lavoro]. Scorri avanti e indietro sulla timeline per visualizzare altri mesi.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->



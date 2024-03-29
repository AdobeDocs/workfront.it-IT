---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra l’allocazione dei ruoli per progetti e iniziative nel Bilanciatore dei carichi di lavoro
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Mostra l’allocazione dei ruoli per progetti e iniziative in [!UICONTROL Bilanciatore dei carichi di lavoro]

>[!IMPORTANT]
>
>La tua organizzazione deve acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] in modo da poter visualizzare le informazioni sull’iniziativa su un progetto. Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che corrisponda. In questo modo si evita di sovrassegnarle o sottoutilizzarle.

Questo articolo descrive come riconciliare le risorse utilizzando [!UICONTROL Allocazione mansioni] pannello in [!UICONTROL Bilanciatore dei carichi di lavoro] di un progetto

Per informazioni generali sulla riconciliazione delle risorse tra progetti e iniziative, inclusi i prerequisiti, consulta [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisiti di accesso

Devi effettuare le seguenti operazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o versione successiva</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alle funzionalità descritte in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva ai progetti </p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md">Accesso [!UICONTROL Request] a un piano in [!DNL Workfront Scenario Planner]</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un progetto, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Mostra l’allocazione dei ruoli per progetti e iniziative in [!UICONTROL Bilanciatore dei carichi di lavoro]

Se la tua azienda ha acquistato un [!DNL Workfront Scenario Planner] , è possibile riconciliare le allocazioni di risorse tra l&#39;iniziativa e il progetto ad essa collegato a livello di progetto [!UICONTROL Bilanciatore dei carichi di lavoro].

1. (Condizionale) Collega un progetto a un’iniziativa utilizzando uno dei metodi descritti nei seguenti articoli:

   * [Importa progetti nei piani in [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Aggiornare o creare progetti pubblicando iniziative in [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Se apporti modifiche alle risorse dell’iniziativa, devi ripubblicare lo scenario a cui appartiene l’iniziativa per ottenere le informazioni più recenti sulle risorse dell’iniziativa da aggiornare sul progetto.

1. Vai al progetto in cui desideri rivedere l’allocazione delle mansioni per il progetto e per l’iniziativa associata.
1. Clic [!UICONTROL Bilanciatore dei carichi di lavoro] nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **[!UICONTROL Pianificazione]**, quindi **[!UICONTROL Passa al Bilanciatore dei carichi di lavoro]**.

1. Esegui una delle operazioni seguenti:

   * Clic **[!UICONTROL Mese]** per visualizzare il Bilanciatore dei carichi di lavoro per mese, fai clic sul menu a discesa accanto a un mese nella timeline ![](assets/drop-down-next-to-month-month-view-wb.png), quindi fai clic su **[!UICONTROL Altro]**.
   * Fai clic su **[!UICONTROL Mostra allocazione ruoli]** icona ![](assets/show-role-allocation-icon.png) nell’angolo superiore destro della barra degli strumenti.

   Il [!UICONTROL Allocazione mansioni] viene visualizzato il pannello.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Anche se è possibile visualizzare [!UICONTROL Allocazione mansioni] anche se la tua organizzazione non ha acquistato un [!DNL Workfront Scenario Planner] licenza, non è possibile visualizzare informazioni sulle mansioni delle iniziative.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Rivedi le seguenti informazioni in **[!UICONTROL Totali progetto]** area del pannello Allocazione ruoli:

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
      <td> <p>Differenza tra le ore necessarie per l'iniziativa e le ore pianificate associate al lavoro sul progetto. [!DNL Workfront] Calcola la varianza di [!UICONTROL] utilizzando la formula seguente:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando le risorse sono pianificate per più ore rispetto a quelle richieste per l'iniziativa, la [!UICONTROL Variance] è negativa e viene visualizzata in rosso. Ciò significa che le risorse sono sovrassegnate. </p> </td> 
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
   >   * Quando le attività o i problemi hanno [!UICONTROL Durata] pari a zero.




1. (Facoltativo) Se [!UICONTROL Varianza] mostra che le risorse sono sovrassegnate, effettua una delle seguenti operazioni:

   * Ridurre il numero di ore pianificate per una mansione che mostra le risorse sovrassegnate o aggiungere più risorse alle attività e distribuire più ore pianificate alle nuove risorse. È possibile aggiornare le assegnazioni o il numero di ore pianificate per le attività o i problemi durante la modifica. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Modifica attività](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifica problemi](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Per modificare attività e problemi è necessario disporre di autorizzazioni e diritti di accesso aggiuntivi.

   * Aumenta il numero di ore richieste per il ruolo che mostra la sovrassegnazione nell’iniziativa. Per ulteriori informazioni, consulta [Creare e modificare le iniziative in [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Per modificare i piani è necessario disporre di autorizzazioni e di accesso aggiuntivi.


1. (Facoltativo) Fai clic sull’icona a discesa per espandere uno dei mesi nella [!UICONTROL Allocazione mansioni] nella timeline del [!UICONTROL Bilanciatore dei carichi di lavoro].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Lo stesso tipo di informazioni visualizzate nel [!UICONTROL Totali progetto] L&#39;area viene visualizzata anche per ogni mese.

   >[!TIP]
   >
   >I mesi elencati nel [!UICONTROL Allocazione mansioni] sono i mesi nella timeline visualizzati sullo schermo nel [!UICONTROL Bilanciatore dei carichi di lavoro]. Scorri avanti e indietro sulla timeline per visualizzare altri mesi.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->



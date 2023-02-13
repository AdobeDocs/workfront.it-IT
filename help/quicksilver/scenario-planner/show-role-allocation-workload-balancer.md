---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra l’allocazione dei ruoli per progetti e iniziative nel servizio di bilanciamento del carico di lavoro
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione affiancata per assicurarti che
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Mostrare la ripartizione dei ruoli per progetti e iniziative [!DNL Workload Balancer]

>[!IMPORTANT]
>
>La tua organizzazione deve acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per visualizzare le informazioni relative all’iniziativa su un progetto. Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione affiancata per garantirne la corrispondenza. In questo modo si evita la sovrallocazione o il sottoutilizzo dei fondi.

Questo articolo descrive come riconciliare le risorse utilizzando [!UICONTROL Assegnazione ruolo] pannello in [!UICONTROL Bilanciamento del carico di lavoro] di un progetto.

Per informazioni generali sulla riconciliazione delle risorse tra progetti e iniziative, compresi i prerequisiti, consulta [Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisiti di accesso

Devi seguire:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Visualizzazione progetti o accesso successivo </p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>[!UICONTROL View] o autorizzazioni successive al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md">Accesso a un piano in [!DNL Workfront Scenario Planner]</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un progetto, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Mostrare la ripartizione dei ruoli per progetti e iniziative [!DNL Workload Balancer]

Se la tua azienda ha acquistato un [!DNL Workfront Scenario Planner] licenza, puoi riconciliare le allocazioni di risorse tra l&#39;iniziativa e il progetto ad essa collegato a livello di progetto [!DNL Workload Balancer].

1. (Condizionale) Collega un progetto a un’iniziativa utilizzando uno dei metodi descritti nei seguenti articoli:

   * [Importa progetti nei piani [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Se apporti modifiche alle risorse nell’iniziativa, devi ripubblicare lo scenario a cui appartiene l’iniziativa per aggiornare il progetto con le informazioni più recenti sulle risorse dell’iniziativa.

1. Vai al progetto in cui desideri esaminare l’allocazione dei ruoli di lavoro per il progetto e per l’iniziativa associata.
1. Fai clic su [!DNL Workload Balancer] nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **[!UICONTROL Pianificazione]**, quindi **[!UICONTROL Passa al bilanciamento del carico di lavoro]**.

1. Esegui una delle operazioni seguenti:

   * Fai clic su **[!UICONTROL Mese]** per visualizzare il servizio di bilanciamento del carico di lavoro per mese, fai clic sul menu a discesa accanto a un mese nella timeline ![](assets/drop-down-next-to-month-month-view-wb.png), quindi fai clic su **[!UICONTROL Altro]**.
   * Fai clic sul pulsante **[!UICONTROL Mostra allocazione ruolo]** icona ![](assets/show-role-allocation-icon.png) nell’angolo superiore destro della barra degli strumenti.

   La [!UICONTROL Assegnazione ruolo] viene visualizzato il pannello .

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Anche se è possibile visualizzare il [!UICONTROL Assegnazione ruolo] , anche se l’organizzazione non ha acquistato un [!DNL Workfront Scenario Planner] non è possibile visualizzare informazioni sui ruoli di lavoro delle iniziative.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Consulta le seguenti informazioni nella sezione **[!UICONTROL Totali progetto]** area del pannello Assegnazione ruoli:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ruolo processo]</td> 
      <td> <p>I nomi dei ruoli di lavoro associati a uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>compiti del progetto</p> </li> 
        <li> <p>questioni relative al progetto</p> </li> 
        <li> <p>iniziativa legata al progetto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Numero di ore richieste associate a ciascun ruolo di lavoro nell'iniziativa per la durata totale dell'iniziativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Orario pianificato]</td> 
      <td>Numero di ore pianificate associate a ciascun ruolo di lavoro nelle attività o nei problemi del progetto per la durata totale del progetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Differenza tra le ore richieste per l'iniziativa e le ore pianificate associate al lavoro sul progetto. [!DNL Workfront] calcola la [!UICONTROL Variance] utilizzando questa formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando le risorse vengono pianificate per più ore rispetto a quelle richieste nell’iniziativa, la [!UICONTROL Variance] è negativa e viene visualizzata in rosso. Ciò significa che le risorse sono sovrassegnate. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Le ore pianificate dal progetto non vengono visualizzate nei seguenti scenari:
   >
   >   
   >   
   >   * Quando attività o problemi non vengono assegnati a ruoli di lavoro o a utenti a cui è associato un ruolo di lavoro.
   >   * Quando attività o problemi hanno una [!UICONTROL Durata] pari a zero.




1. (Facoltativo) Se [!UICONTROL Varianza] mostra che le risorse sono sovrassegnate e regola una delle seguenti operazioni:

   * Riduci il numero di ore pianificate per un ruolo di lavoro che mostra sovrassegnate o aggiungi più risorse alle attività e distribuisci più ore pianificate alle nuove risorse. È possibile aggiornare le assegnazioni o il numero di ore pianificate per le attività o i problemi durante la loro modifica. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Modifica delle attività](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifica dei problemi](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Per modificare attività e problemi è necessario disporre di autorizzazioni e accesso aggiuntivi.

   * Aumenta il numero di ore necessarie per il ruolo che mostra la sovrallocazione dell&#39;iniziativa. Per ulteriori informazioni, consulta [Creare e modificare iniziative in [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Per modificare i piani è necessario disporre di ulteriori autorizzazioni e accesso.


1. (Facoltativo) Fai clic sull’icona a discesa per espandere uno dei mesi nel [!UICONTROL Assegnazione ruolo] o nella timeline [!UICONTROL Bilanciamento del carico di lavoro].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Lo stesso tipo di informazioni visualizzate nel [!UICONTROL Totali progetto] viene visualizzata anche per ogni mese.

   >[!TIP]
   >
   >I mesi elencati nel [!UICONTROL Assegnazione ruolo] i mesi nella timeline visualizzati sullo schermo nel [!UICONTROL Bilanciamento del carico di lavoro]. Scorri avanti e indietro nella timeline per visualizzare altri mesi.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->



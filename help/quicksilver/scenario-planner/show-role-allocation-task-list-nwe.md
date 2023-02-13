---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra l'allocazione dei ruoli per progetti e iniziative nell'elenco dei task
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione affiancata per garantirne la corrispondenza. In questo modo si evita la sovrallocazione o il sottoutilizzo dei fondi.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Mostra l&#39;allocazione dei ruoli per progetti e iniziative nell&#39;elenco dei task

>[!IMPORTANT]
>
>La tua organizzazione deve acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per visualizzare le informazioni relative all’iniziativa su un progetto. Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione affiancata per garantirne la corrispondenza. In questo modo si evita la sovrallocazione o il sottoutilizzo dei fondi.

Questo articolo descrive come riconciliare le risorse utilizzando [!UICONTROL Assegnazione ruolo] nell’elenco delle attività di un progetto.

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
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Visualizzazione progetti o accesso successivo </p> <p>Nota: Se non hai ancora accesso, chiedi al tuo amministratore [!UICONTROL Workfront] se impostano ulteriori restrizioni nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>[!UICONTROL View] o autorizzazioni successive al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un progetto, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Mostra l&#39;allocazione dei ruoli per progetti e iniziative nell&#39;elenco dei task

Se la tua azienda ha acquistato un [!DNL Workfront Scenario Planner] licenza, puoi riconciliare le allocazioni di risorse tra l&#39;iniziativa e il progetto ad essa collegato nel [!UICONTROL Attività] sezione del progetto.

1. (Condizionale) Collega un progetto a un’iniziativa utilizzando uno dei metodi descritti in [Mostra l&#39;allocazione dei ruoli per progetti e iniziative nell&#39;elenco dei task](#Connect) del presente articolo.

   >[!IMPORTANT]
   >
   >Se apporti modifiche alle risorse nell’iniziativa, devi ripubblicare lo scenario a cui appartiene l’iniziativa per aggiornare il progetto con le informazioni più recenti sulle risorse dell’iniziativa.

1. Vai al progetto in cui desideri esaminare l’allocazione dei ruoli di lavoro per il progetto e per l’iniziativa associata.
1. Fai clic su **[!UICONTROL Attività]** nel pannello a sinistra.
1. Fai clic sul pulsante **[!UICONTROL Mostra allocazione ruolo]** icona ![](assets/show-role-allocation-icon.png) nell’angolo superiore destro della barra degli strumenti.

   La [!UICONTROL Assegnazione ruolo] viene visualizzato il pannello .

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Consulta le seguenti informazioni nella sezione **[!UICONTROL Totali progetto]** area [!UICONTROL Assegnazione ruolo] pannello:

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
   >   * Quando attività o problemi hanno una durata pari a zero.




1. (Facoltativo) Se [!UICONTROL Varianza] mostra che le risorse sono sovrassegnate e regola una delle seguenti operazioni:

   * Riduci il numero di ore pianificate per un ruolo di lavoro che mostra sovrassegnate o aggiungi più risorse alle attività e distribuisci più ore pianificate alle nuove risorse. È possibile aggiornare le assegnazioni o il numero di ore pianificate per le attività o i problemi durante la loro modifica. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Modifica delle attività](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifica dei problemi](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Per modificare attività e problemi è necessario disporre di autorizzazioni e accesso aggiuntivi.

   * Aumenta il numero di ore necessarie per il ruolo che mostra la sovrallocazione sull&#39;iniziativa. Per ulteriori informazioni, consulta [Creare e modificare iniziative in [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Per modificare i piani è necessario disporre di ulteriori autorizzazioni e accesso.




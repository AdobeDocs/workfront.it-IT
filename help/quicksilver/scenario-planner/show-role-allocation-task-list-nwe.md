---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostra assegnazione ruoli per progetti e iniziative nell'elenco delle attività
description: Dopo aver collegato progetti e iniziative, puoi gestirne l’allocazione delle risorse in modo che corrisponda. In questo modo si evita di sovrassegnarle o sottoutilizzarle.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '676'
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
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per i nuovi piani Workfront Select o Workfront Prime. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso di visualizzazione o superiore ai progetti.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p> Visualizza o autorizzazioni superiori per un progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
      <td> <p>Differenza tra le ore necessarie per l'iniziativa e le ore pianificate associate al lavoro sul progetto. [!DNL Workfront] calcola la varianza  utilizzando questa formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Quando le risorse sono pianificate per più ore rispetto a quelle richieste per l'iniziativa, la [!UICONTROL Variance] è negativa e viene visualizzata in rosso. Ciò significa che le risorse sono sovrassegnate. </p> </td> 
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



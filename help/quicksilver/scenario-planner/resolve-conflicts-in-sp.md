---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Risolvere i conflitti di iniziativa nella Pianificazione scenario
description: Quando le iniziative sono in conflitto tra loro, competono per le stesse risorse. Le risorse disponibili per uno scenario non sono sufficienti per coprire tutte le risorse necessarie per tutte le iniziative dello scenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '2164'
ht-degree: 0%

---

# Risolvi conflitti di iniziativa in [!DNL Scenario Planner]

Quando le iniziative sono in conflitto tra loro, competono per le stesse risorse. Le risorse disponibili per uno scenario non sono sufficienti per coprire tutte le risorse necessarie per tutte le iniziative dello scenario.

Ciò può verificarsi in uno qualsiasi dei seguenti casi:

* Il numero di ruoli richiesti per l&#39;iniziativa è maggiore del numero di ruoli preventivati per il piano.
* I costi dell&#39;iniziativa sono superiori all&#39;importo di bilancio disponibile per il piano.

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
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica sulla risoluzione dei conflitti

* Per conflitto si intende anche una sovrassegnazione delle mansioni o del budget di uno scenario.
* Quando [!DNL Workfront] rileva un conflitto, la barra corrispondente al mese in conflitto durante la durata dell&#39;iniziativa viene visualizzata in rosso. Ciò può verificarsi in uno qualsiasi dei seguenti casi:

   * Il numero di ruoli richiesti mensilmente per un&#39;iniziativa è maggiore del numero di ruoli preventivati per il piano dopo che tutte le iniziative precedenti hanno utilizzato le risorse preventivate per il piano.
   * I costi mensili dell&#39;iniziativa sono superiori al bilancio disponibile per il piano dopo che tutte le iniziative precedenti hanno utilizzato il bilancio del piano per coprire i costi.

>[!TIP]
>
>Per impostazione predefinita, [!DNL Scenario Planner] presuppone che sia stato preventivato per 0 mansioni e $0 o l&#39;equivalente di $0 nella valuta del sistema per uno scenario, a meno che non sia stato specificato diversamente. Il numero di mansioni indica il numero di FTE (equivalenti a tempo pieno) o di ore preventivate per la mansione.
>
>Per tutti i calcoli in Scenario Planner, Workfront utilizza il seguente valore: 1 FTE = 8 ore.
>
>Per informazioni sull&#39;aggiornamento dei ruoli disponibili per un piano e un budget, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* È possibile risolvere un conflitto eseguendo una delle operazioni seguenti:

   * Aggiunta automatica delle risorse richieste mancanti dalle iniziative sullo scenario. Questo articolo descrive come risolvere i conflitti utilizzando questa opzione.
   * Adeguare le risorse mansione e budget per lo scenario modificando il piano. Per ulteriori informazioni, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Risolvere i conflitti tra iniziative

1. Passare a un piano per il quale si desidera risolvere i conflitti.

   Per informazioni sulla creazione dei piani, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Per informazioni sulla creazione delle iniziative, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facoltativo) Dal menu a discesa **[!DNL Initial scenario]**, selezionare lo scenario che si desidera esaminare.

   >[!TIP]
   >
   >Un piano può avere diversi scenari. Esaminando i conflitti del piano, [!DNL Workfront] fa riferimento alle risorse attualmente disponibili nello scenario selezionato e a quelle necessarie per le iniziative dello scenario. Per informazioni sugli scenari, vedere [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Verificare che **[!UICONTROL Mostra conflitti]** sia abilitato. È attivata per impostazione predefinita.

   ![](assets/show-scenarios-toggle-on.png)

   La prima iniziativa in conflitto visualizza in rosso i mesi con conflitti e accanto al nome dell’iniziativa viene visualizzata un’icona di avviso.

   Lo sfondo di tutte le iniziative che iniziano con la prima in conflitto viene visualizzato in rosso sul grafico del piano.

   Quando un&#39;iniziativa presenta un conflitto, significa che il numero di mansioni per almeno una mansione specifica, i costi sostenuti o entrambi superano il numero di mansioni o il budget definito per il piano per un mese specifico.

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Effettuare una delle seguenti operazioni per ulteriori informazioni sui conflitti che potrebbero esistere:

   * Passa il cursore del mouse sull’icona di avviso accanto al nome dell’iniziativa per capire se disponi di una mansione o di un conflitto di budget.

     ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     A seconda che si siano sovrassegnate le mansioni o i costi sovrastimati per l’iniziativa, è possibile che venga visualizzata una delle seguenti opzioni quando si passa il puntatore sull’icona di avviso:

      * Mostra dettagli conflitto mansioni
      * Mostra dettagli conflitto budget
      * Mostra dettagli mansione e budget

   * Quando visualizzi il piano per mese, passa il cursore su un mese nella sequenza temporale del piano per visualizzare le risorse richieste per quel mese e se i conflitti per il mese sono relativi alle persone o ai costi.

     ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Esamina le seguenti informazioni mensili a livello di piano:

      * Il numero di ruoli disponibili, richiesti e sovrassegnati per il mese per tutte le iniziative pianificate per quel mese
      * I costi disponibili, richiesti e sovrassegnati per il mese per tutte le iniziative pianificate per quel mese

        >[!TIP]
        >
        >I costi [!UICONTROL Available] sono il budget dello scenario per quel mese.

   * Passa il cursore del mouse sulla barra rossa di un’iniziativa per un mese, in modo da visualizzare la casella delle informazioni aggiuntive sul conflitto che si verifica in quel mese.

     ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     Rivedi i campi seguenti nella casella delle informazioni aggiuntive a livello di iniziativa:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Mese in cui si verifica il conflitto</td> 
        <td>Viene visualizzato nel titolo della casella Informazioni aggiuntive.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Nome dell’iniziativa</td> 
        <td>Viene visualizzato nel titolo della casella Informazioni aggiuntive.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Ruoli]</td> 
        <td> <p>I ruoli associati a questa iniziativa che sono sovrassegnati per il mese selezionato. Nelle colonne seguenti vengono visualizzate le informazioni per ogni mansione richiesta per il mese selezionato e in conflitto con il numero di mansioni disponibili per quel mese:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponibile]</strong>: numero di ogni mansione disponibile nello scenario per il mese selezionato.</p> </li> 
          <li> <p><strong>[!UICONTROL Richiesto]</strong>: numero di ogni mansione richiesta per l'iniziativa per il mese selezionato.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Sovrassegnato]:</strong> Differenza tra il numero richiesto nell'iniziativa e il numero disponibile nello scenario. </p> </li> 
         </ul> <p>Suggerimento: a volte il numero di ruoli [!UICONTROL Available] corrisponde o è superiore al numero di ruoli [!UICONTROL Required], ma [!DNL Scenario Planner] mostra ancora una sovrassegnazione. Ciò significa che esistono iniziative di livello superiore che hanno già utilizzato i ruoli disponibili nel piano per lo stesso mese. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Costi</td> 
        <td> <p>I costi dell'iniziativa per il mese selezionato. Nelle colonne seguenti vengono visualizzate le informazioni relative ai costi necessari e al budget disponibile del mese selezionato:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponibile]</strong>: Budget disponibile dal piano per il mese selezionato.</p> </li> 
          <li> <p><strong>[!UICONTROL Richiesto]</strong>: i costi associati a questa iniziativa per il mese selezionato.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Sovrassegnato]:</strong> Differenza tra i costi dell'iniziativa e il budget disponibile nel piano. </p> </li> 
         </ul> <p>Suggerimento: a volte i costi di [!UICONTROL Available] corrispondono o sono superiori al costo [!UICONTROL Required] dell'iniziativa per il mese selezionato e [!DNL Scenario Planner] mostra ancora una sovrassegnazione dei costi. Ciò significa che esistono iniziative di livello superiore che utilizzano già il budget disponibile sul piano per lo stesso mese. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Per aprire il pannello dei dettagli dell’iniziativa e visualizzare ulteriori informazioni su dove si verificano i conflitti e per risolverli, effettua una delle seguenti operazioni:

   * Fai clic sull’icona di avviso accanto al nome dell’iniziativa.
   * Fai clic sulla barra di un’iniziativa.
   * Fai clic sull&#39;icona **[!UICONTROL Altro]** ![](assets/more-icon.png) a destra del nome dell&#39;iniziativa, quindi fai clic su **[!UICONTROL Modifica]**.

     Il pannello dei dettagli dell’iniziativa viene visualizzato a destra.

     Quando non disponi di un numero sufficiente di persone o di budget per l’iniziativa, accanto alle sezioni seguenti viene visualizzata un’icona di avviso rossa:

   * [!UICONTROL Ruoli richiesti]
   * [!UICONTROL Costi]

1. (Condizionale) Per le iniziative che presentano conflitti di mansioni, vai alla sezione **[!UICONTROL Mansioni richieste]** per visualizzare tutte le mansioni richieste per l&#39;iniziativa. Identifica i ruoli che potrebbero essere sovrassegnati. Esamina il numero di FTE o di ore necessarie per ogni mansione per ogni mese dell’iniziativa. La casella con il numero FTE o ore per i mesi con sovrassegnazioni viene visualizzata in rosso.

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto ai mesi nella timeline dell’iniziativa per visualizzare quali mesi aggiuntivi visualizzano i conflitti di mansioni.

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Facoltativo) Fare clic su **[!UICONTROL Mostra dettagli]** sotto la mansione che visualizza un conflitto per vedere dove appaiono i conflitti ed evidenziare i mesi in conflitto nell&#39;area grafico del piano. Vengono visualizzate informazioni aggiuntive per ogni mansione.

   Per ogni mansione vengono visualizzati i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponibile]</td> 
      <td> <p>Il numero di mansioni disponibili dal piano per ogni mese. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL allocato in precedenza]</td> 
      <td>Il numero di mansioni già allocate dal budget del piano a iniziative di livello superiore per un mese specifico. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL sovrassegnato]</td> 
      <td> <p>Anche la differenza tra il numero di ruoli richiesti nell’iniziativa e il numero disponibile nel piano dopo iniziative di livello superiore ha utilizzato alcuni dei ruoli. Workfront calcola il numero di ruoli di lavoro [!UICONTROL Sovrassegnato] utilizzando la formula seguente:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Nel grafico del piano, i mesi in cui vengono allocate le mansioni visualizzano il nome e il numero di mansioni necessarie per ogni iniziativa in cui sono necessarie. È necessario selezionare la visualizzazione [!UICONTROL Mese] per visualizzare il nome delle mansioni

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Per risolvere i conflitti di mansioni, eseguire una delle operazioni seguenti:

   * Regola manualmente il numero di ruoli per ogni mese dell’iniziativa su un numero inferiore.
   * Passa il puntatore del mouse sul nome della mansione e fai clic sull&#39;icona **[!UICONTROL elimina]** ![](assets/delete.png) per rimuovere la mansione dall&#39;iniziativa.
   * Seleziona **[!UICONTROL Aggiungi ruoli alle risorse disponibili dello scenario]**, quindi fai clic su **[!UICONTROL Applica]**.

     Questo aggiunge il numero mancante di FTE o di ore per la mansione al campo [!UICONTROL Available] dello scenario.

     >[!NOTE]
     >
     >I ruoli aggiunti per risolvere i conflitti modificano i ruoli [!UICONTROL Disponibili] per lo scenario selezionato e non per tutti gli scenari del piano.

     Viene visualizzata una freccia verde rivolta verso l&#39;alto ![](assets/upward-green-arrow.png) per il mese nella sequenza temporale del piano per indicare che sono state aggiunte più risorse al piano in quel mese. È necessario selezionare la visualizzazione [!UICONTROL Mese] per visualizzare questo indicatore.

   * (Facoltativo) Chiudi il pannello dei dettagli e assegna all’iniziativa una priorità più alta per ricevere prima le risorse di budget dal piano, se possibile. Per informazioni sull&#39;aggiornamento della priorità dell&#39;iniziativa, vedere [Aggiornare le priorità dell&#39;iniziativa in Pianificazione scenario](../scenario-planner/prioritize-initiatives.md).

1. (Facoltativo) Fai clic su **[!UICONTROL Nascondi dettagli]** per chiudere la casella dei dettagli aggiuntivi, quindi fai clic su **[!UICONTROL Applica]** per salvare le modifiche apportate alle mansioni.

1. (Condizionale) Per le iniziative che presentano conflitti di costi, vai alla sezione **[!UICONTROL Costi]** nel pannello dei dettagli dell&#39;iniziativa per esaminare i costi per ogni mese della durata dell&#39;iniziativa. Identifica i mesi che potrebbero non avere abbastanza soldi nel budget del piano per coprire i costi per l&#39;iniziativa selezionata. La casella con il budget disponibile insufficiente viene visualizzata in rosso.
1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto ai mesi nella timeline dell’iniziativa per visualizzare i mesi aggiuntivi con budget insufficiente a coprire i costi.

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. (Facoltativo) Fare clic su **[!UICONTROL Mostra dettagli]** sotto le informazioni sui costi per visualizzare la posizione del conflitto ed evidenziare i mesi in conflitto nel grafico del piano. Per ogni tipo di costo vengono visualizzati i seguenti campi aggiuntivi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponibile]</td> 
      <td> <p>I costi disponibili nel budget del piano per ogni mese. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL allocato in precedenza]</td> 
      <td>Importo già assegnato dal bilancio del piano a iniziative di livello superiore. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL sovrassegnato]</td> 
      <td> <p>Anche la differenza mensile tra i costi necessari per l'iniziativa e l'importo di denaro disponibile dal bilancio del piano dopo iniziative di livello superiore ha utilizzato parte del bilancio disponibile. [!DNL Workfront] calcola il numero di costi sovrassegnati utilizzando la seguente formula:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] calcola i costi richiesti per l'iniziativa corrente per ogni mese utilizzando la formula seguente:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Nel grafico del piano, i mesi in cui i costi sono insufficienti visualizzano il nome e il numero di ruoli ancora necessari per l’iniziativa. Per visualizzare gli importi dei costi è necessario selezionare la vista Mese.

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Se al momento della creazione del piano hai disabilitato l&#39;impostazione [!UICONTROL Includi costo persone] per la casella [!UICONTROL Budget] del piano, la riga [!UICONTROL Costi persone] non viene visualizzata per alcuna iniziativa in nessuno scenario. In questo caso, Workfront non prende in considerazione i costi delle persone nei calcoli per determinare i conflitti di costi. Per informazioni sulla creazione di un piano, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Per risolvere i conflitti di costi, effettuare una delle seguenti operazioni:

   * Regola manualmente il numero di [!UICONTROL Costi fissi] per ogni mese dell&#39;iniziativa su un numero inferiore.
   * Nella sezione **[!UICONTROL Ruoli richiesti]**, regolare manualmente il numero di ruoli per il mese con un budget Costi persone, se possibile. Questo riduce il numero di costi delle persone.

     >[!TIP]
     >
     >Non è possibile regolare manualmente i costi delle persone.

   * Seleziona **[!UICONTROL Aggiungi importo al budget dello scenario]**, quindi fai clic su **[!UICONTROL Applica]**.

     Questo aggiunge l&#39;importo insufficiente al budget dello scenario per i mesi in cui mancava, aggiornando anche il budget complessivo dello scenario.

     >[!NOTE]
     >
     >L&#39;importo aggiunto per risolvere i conflitti di costo modifica il budget per lo scenario selezionato e non per tutti gli scenari del piano.

   * (Facoltativo) Chiudi il pannello dei dettagli e assegna all’iniziativa una priorità più alta per ricevere prima le risorse di budget dal piano, se possibile. Per informazioni sull&#39;aggiornamento della priorità dell&#39;iniziativa, vedere [Aggiornare le priorità dell&#39;iniziativa in [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Fare clic su **[!UICONTROL Applica]** quando si apportano modifiche alla sezione Costi.
1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.



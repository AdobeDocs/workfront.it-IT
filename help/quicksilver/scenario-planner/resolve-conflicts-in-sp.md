---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Risolvere i conflitti di iniziativa nel Planner scenario
description: Quando le iniziative sono in conflitto tra loro, competono per le stesse risorse. Le risorse disponibili per uno scenario non sono sufficienti a coprire tutte le risorse richieste da tutte le iniziative dello scenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '2183'
ht-degree: 0%

---

# Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]

Quando le iniziative sono in conflitto tra loro, competono per le stesse risorse. Le risorse disponibili per uno scenario non sono sufficienti a coprire tutte le risorse richieste da tutte le iniziative dello scenario.

Questo può accadere in uno dei seguenti casi:

* Il numero di ruoli di lavoro necessari per l&#39;iniziativa è maggiore del numero di ruoli preventivati per il piano.
* I costi dell&#39;iniziativa sono superiori all&#39;importo di bilancio disponibile per il piano.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td> <p>Modifica [!UICONTROL] o superiore al [!DNL Scenario Planner]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Panoramica sulla risoluzione dei conflitti

* Un conflitto è anche inteso come una sovrallocazione dei ruoli di lavoro o del budget di uno scenario.
* Quando [!DNL Workfront] rileva un conflitto. La barra corrispondente al mese in conflitto durante la durata dell&#39;iniziativa viene visualizzata in rosso. Questo può accadere in uno dei seguenti casi:

   * Il numero di ruoli di lavoro richiesti mensilmente per un&#39;iniziativa è maggiore del numero di ruoli iscritti in bilancio per il piano dopo che tutte le iniziative precedenti hanno utilizzato le risorse previste in budget per il piano.
   * I costi mensili dell&#39;iniziativa sono superiori al bilancio disponibile per il piano dopo che tutte le precedenti iniziative hanno utilizzato il bilancio del piano per coprire i loro costi.

>[!TIP]
>
>Per impostazione predefinita, la [!DNL Scenario Planner] presuppone che sia stato impostato il budget per 0 ruoli di lavoro e $0 o l&#39;equivalente di $0 nella valuta del sistema per uno scenario, a meno che non sia stato specificato diversamente. Il numero di ruoli di lavoro indica il numero di FTE (equivalenti a tempo pieno) o di ore in budget per il ruolo di lavoro.
>
>Per tutti i calcoli nel Planner scenario, Workfront utilizza il seguente valore: 1 ETP = 8 ore.
>
>Per informazioni sull&#39;aggiornamento dei ruoli disponibili per un piano e un budget, vedere [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* È possibile risolvere un conflitto eseguendo una delle operazioni seguenti:

   * Aggiunta automatica delle risorse necessarie mancanti dalle iniziative sullo scenario. Questo articolo descrive come risolvere i conflitti utilizzando questa opzione.
   * Adeguamento del ruolo di lavoro e delle risorse di budget per lo scenario, modificando il piano. Per ulteriori informazioni, consulta [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Risolvere i conflitti tra le iniziative

1. Passare a un piano per il quale si desidera risolvere i conflitti.

   Per informazioni sulla creazione dei piani, consulta [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Per informazioni sulla creazione di iniziative, consulta [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facoltativo) Dal **[!DNL Initial scenario]** dal menu a discesa, selezionare lo scenario da esaminare.

   >[!TIP]
   >
   >Un piano può avere diversi scenari. Quando si esaminano i conflitti del piano, [!DNL Workfront] fa riferimento alle risorse attualmente disponibili sullo scenario selezionato e a quelle necessarie sulle iniziative di tale scenario. Per informazioni sugli scenari, vedi [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Assicurati che **[!UICONTROL Mostra conflitti]** è abilitato. È attivata per impostazione predefinita.

   ![](assets/show-scenarios-toggle-on.png)

   La prima iniziativa in conflitto visualizza i mesi in cui sono presenti conflitti in rosso, mentre accanto al nome dell’iniziativa viene visualizzata un’icona di avviso.

   Lo sfondo di tutte le iniziative che iniziano con la prima in conflitto viene visualizzato in rosso sul grafico del piano.

   Quando un&#39;iniziativa visualizza un conflitto, significa che il numero di ruoli per almeno un ruolo specifico, i costi sostenuti o entrambi superano il numero di ruoli o il budget definito per il piano per un mese specifico.

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Effettua una delle seguenti operazioni per ulteriori informazioni sui conflitti esistenti:

   * Passa il puntatore sull’icona di avviso accanto al nome dell’iniziativa per capire se hai un ruolo o un conflitto di budget.

      ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

      A seconda che i ruoli di lavoro siano stati sovrapassegnati o che i costi dell’iniziativa siano stati sopravvalutati, quando passi il cursore sull’icona di avviso potrebbe essere visualizzata una delle seguenti opzioni:

      * Mostra dettagli conflitto mansioni
      * Mostra dettagli conflitto budget
      * Mostra dettagli su ruolo e budget
   * Quando si visualizza il piano per mese, passare il cursore del mouse sopra un mese nella timeline del piano per visualizzare le risorse necessarie per quel mese e se i conflitti relativi al mese sono relativi a persone o costi.

      ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

      Rivedi le seguenti informazioni mensili a livello di piano:

      * Numero di ruoli di lavoro disponibili, richiesti e sovrassegnati per il mese per tutte le iniziative pianificate per quel mese
      * I costi disponibili, richiesti e sovrassegnati per il mese per tutte le iniziative previste per quel mese

         >[!TIP]
         >
         >La [!UICONTROL Disponibile] i costi sono il budget dello scenario per quel mese.
   * Passa il cursore del mouse sulla barra rossa di un&#39;iniziativa per un mese per visualizzare la casella delle informazioni aggiuntive sul conflitto che si verifica in quel mese.

      ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

      Rivedi i seguenti campi nella casella delle informazioni aggiuntive a livello di iniziativa:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Mese in cui si verifica il conflitto</td> 
        <td>Viene visualizzato nel titolo della casella delle informazioni aggiuntive.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Nome dell'iniziativa</td> 
        <td>Viene visualizzato nel titolo della casella delle informazioni aggiuntive.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Ruoli processo]</td> 
        <td> <p>I ruoli di lavoro associati a questa iniziativa che sono sovrassegnati per il mese selezionato. Nelle colonne seguenti sono visualizzate le informazioni relative a ciascun ruolo di lavoro richiesto per il mese selezionato e in conflitto con il numero di ruoli di lavoro disponibili per tale mese:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponibile]</strong>: Il numero di ogni ruolo di lavoro disponibile dallo scenario per il mese selezionato.</p> </li> 
          <li> <p><strong>[!UICONTROL Obbligatorio]</strong>: Il numero di ogni ruolo di lavoro richiesto per l'iniziativa per il mese selezionato.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Sovrassegnata]:</strong> La differenza tra il numero richiesto nell'iniziativa e il numero disponibile nello scenario. </p> </li> 
         </ul> <p>Suggerimento: A volte, il numero di ruoli [!UICONTROL Available] corrisponde o è superiore al numero di ruoli [!UICONTROL Required], ma il [!DNL Scenario Planner] mostra ancora una sovrallocazione. Ciò significa che esistono iniziative di alto livello che hanno già utilizzato i ruoli di lavoro disponibili nel piano per lo stesso mese. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Costi</td> 
        <td> <p>I costi dell'iniziativa per il mese selezionato. Nelle colonne seguenti vengono visualizzate le informazioni relative ai costi necessari e al budget disponibile per il mese selezionato:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponibile]</strong>: Il budget disponibile dal piano per il mese selezionato .</p> </li> 
          <li> <p><strong>[!UICONTROL Obbligatorio]</strong>: I costi associati a questa iniziativa per il mese selezionato.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Sovrassegnata]:</strong> La differenza tra i costi dell'iniziativa e il bilancio disponibile dal piano. </p> </li> 
         </ul> <p>Suggerimento: A volte, i costi [!UICONTROL Available] corrispondono o sono superiori al costo [!UICONTROL Required] dell'iniziativa per il mese selezionato e il [!DNL Scenario Planner] mostra ancora una sovrallocazione dei costi. Ciò significa che vi sono iniziative di alto livello che utilizzano già il bilancio disponibile sul piano per lo stesso mese. </p> </td> 
       </tr> 
      </tbody> 
     </table>



1. Effettua una delle seguenti operazioni per aprire il pannello dei dettagli dell’iniziativa e visualizzare ulteriori informazioni su dove si verificano i conflitti e per risolverli:

   * Fai clic sull’icona di avviso accanto al nome dell’iniziativa.
   * Fai clic sulla barra di un&#39;iniziativa.
   * Fai clic sul pulsante **[!UICONTROL Altro]** icona ![](assets/more-icon.png) a destra del nome dell&#39;iniziativa, quindi fai clic su **[!UICONTROL Modifica]**.

      Il pannello dei dettagli dell&#39;iniziativa viene visualizzato a destra.

      Se non disponi di un numero sufficiente di persone o di budget per l’iniziativa, accanto alle sezioni seguenti viene visualizzata un’icona di avviso rossa:

   * [!UICONTROL Ruoli richiesti]
   * [!UICONTROL Costi]

1. (Condizionale) Per le iniziative che presentano conflitti di ruolo, passa alla sezione **[!UICONTROL Ruoli di lavoro richiesti]** per visualizzare tutti i ruoli di lavoro richiesti per l’iniziativa. Identificare i ruoli di lavoro che potrebbero essere sovrassegnati. Rivedi il numero di ETP o ore necessarie per ciascun ruolo di lavoro per ogni mese dell’iniziativa. La casella con il numero di ore o di tempo per i mesi con sovrassegnazioni viene visualizzata in un contorno rosso.

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto ai mesi nella timeline dell’iniziativa per visualizzare i mesi aggiuntivi in cui vengono visualizzati i conflitti tra ruoli di lavoro.

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Facoltativo) Fai clic su **[!UICONTROL Mostra dettagli]** sotto il ruolo job che visualizza un conflitto per vedere dove vengono visualizzati i conflitti e per evidenziare i mesi in conflitto nell&#39;area grafico del piano. Per ogni ruolo di lavoro vengono visualizzate informazioni aggiuntive.

   Per ciascun ruolo di lavoro vengono visualizzati i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponibile]</td> 
      <td> <p>Numero di ruoli di lavoro disponibili nel piano per ogni mese. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Assegnato in precedenza]</td> 
      <td>Numero di ruoli di lavoro già assegnati dal budget del piano a iniziative di livello superiore per un mese specifico. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sovrassegnata]</td> 
      <td> <p>Anche la differenza tra il numero di ruoli di lavoro richiesti nell'iniziativa e il numero disponibile nel piano dopo le iniziative di livello superiore ha utilizzato alcuni dei ruoli. Workfront calcola il numero di ruoli di lavoro [!UICONTROL Overallocate] utilizzando la seguente formula:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Nel grafico del piano, i mesi in cui i ruoli di lavoro sono allocati presentano il nome e il numero di ruoli necessari per ogni iniziativa in cui sono necessari. È necessario selezionare la [!UICONTROL Mese] visualizzare il nome dei ruoli del processo

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Per risolvere i conflitti relativi ai ruoli di lavoro, eseguire una delle operazioni seguenti:

   * Regola manualmente il numero di ruoli di lavoro per ogni mese dell’iniziativa con un numero inferiore.
   * Passa il puntatore del mouse sul nome del ruolo del lavoro e fai clic sul pulsante **[!UICONTROL delete] icona** ![](assets/delete.png) rimuovere il ruolo di lavoro dall&#39;iniziativa.
   * Seleziona **[!UICONTROL Aggiungi ruoli alle risorse disponibili dello scenario]**, quindi fai clic su **[!UICONTROL Applica]**.

      Questo aggiunge il numero mancante di FTE o ore di ruolo nello scenario [!UICONTROL Disponibile] campo .

      >[!NOTE]
      >
      >I ruoli aggiunti per risolvere i conflitti modificano la [!UICONTROL Disponibile] ruoli di lavoro per lo scenario selezionato e non per tutti gli scenari del piano.

      Una freccia verde verso l&#39;alto ![](assets/upward-green-arrow.png) viene visualizzato per il mese nella timeline del piano per indicare che sono state aggiunte ulteriori risorse al piano in quel mese. È necessario selezionare la [!UICONTROL Mese] visualizza questo indicatore.

   * (Condizionale) Chiudi il pannello dei dettagli e assegna all’iniziativa una priorità più elevata per ricevere prima risorse di bilancio dal piano, se possibile. Per informazioni sull&#39;aggiornamento della priorità dell&#39;iniziativa, vedi [Aggiornare le priorità dell&#39;iniziativa nel planner dello scenario](../scenario-planner/prioritize-initiatives.md).

1. (Facoltativo) Fai clic su **[!UICONTROL Nascondi dettagli]** per chiudere la casella dei dettagli aggiuntivi, fai clic su **[!UICONTROL Applica]** per salvare le modifiche apportate ai ruoli di lavoro.

1. (Condizionale) Per le iniziative che hanno conflitti di costi, vai al **[!UICONTROL Costi]** sezione del pannello dei dettagli dell&#39;iniziativa per esaminare i costi per ogni mese della durata dell&#39;iniziativa. Indicare quali mesi potrebbero non disporre di fondi sufficienti nel bilancio del piano per coprire i costi dell&#39;iniziativa selezionata. La casella con il budget disponibile insufficiente viene visualizzata in un contorno rosso.
1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto ai mesi nel calendario dell&#39;iniziativa per visualizzare i mesi aggiuntivi con budget insufficiente per coprire i costi.

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. (Facoltativo) Fai clic su **[!UICONTROL Mostra dettagli]** in informazioni sui costi per vedere dove appare il conflitto ed evidenziare i mesi in conflitto nel grafico del piano. Per ogni tipo di costo vengono visualizzati i seguenti campi aggiuntivi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponibile]</td> 
      <td> <p>I costi disponibili a titolo del bilancio del piano per ogni mese. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Assegnato in precedenza]</td> 
      <td>L'importo già assegnato dal bilancio del piano a iniziative di alto livello. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sovrassegnata]</td> 
      <td> <p>Anche la differenza mensile tra i costi necessari per l'iniziativa e l'importo disponibile a titolo del bilancio del piano dopo iniziative di alto livello ha utilizzato parte del bilancio disponibile. [!DNL Workfront] calcola il numero di costi sovrallocati utilizzando la formula seguente:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] calcola i costi richiesti per l'iniziativa corrente per ogni mese utilizzando la seguente formula:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Nel grafico del piano, i mesi in cui i costi sono insufficienti mostrano il nome e il numero di ruoli ancora necessari per l&#39;iniziativa. Selezionare la visualizzazione Mese per visualizzare gli importi dei costi.

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Se hai disabilitato [!UICONTROL Includi costi per le persone] impostazione del piano [!UICONTROL Bilancio] quando hai creato il piano, la [!UICONTROL Costi per le persone] In nessun caso, la linea non viene visualizzata per alcuna iniziativa. In questo caso, Workfront non inserisce i costi delle persone nei calcoli per determinare i conflitti di costi. Per informazioni sulla creazione di un piano, vedi [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Per risolvere i conflitti relativi ai costi, eseguire una delle operazioni seguenti:

   * Regolare manualmente il numero di [!UICONTROL Costi fissi] per ogni mese dell&#39;iniziativa a un numero inferiore.
   * In **[!UICONTROL Ruoli di lavoro richiesti]** Regola manualmente il numero di ruoli di lavoro per il mese con un budget per i costi delle persone, se possibile. Questo riduce il numero dei costi delle persone.

      >[!TIP]
      >
      >Non è possibile regolare manualmente i costi delle persone.

   * Seleziona **[!UICONTROL Aggiungi importo al budget dello scenario]**, quindi fai clic su **[!UICONTROL Applica]**.

      Questo aggiunge l&#39;importo insufficiente al bilancio dello scenario per i mesi in cui era mancante, il che aggiorna anche il bilancio dello scenario complessivo.

      >[!NOTE]
      >
      >L&#39;importo aggiunto per risolvere i conflitti di costo modifica il budget per lo scenario selezionato e non per tutti gli scenari del piano.

   * (Condizionale) Chiudi il pannello dei dettagli e assegna all’iniziativa una priorità più elevata per ricevere prima risorse di bilancio dal piano, se possibile. Per informazioni sull&#39;aggiornamento della priorità dell&#39;iniziativa, vedi [Aggiornare le priorità dell&#39;iniziativa [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Fai clic su **[!UICONTROL Applica]** quando apporti modifiche alla sezione Costi .
1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.



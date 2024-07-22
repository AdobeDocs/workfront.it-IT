---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creare e modificare iniziative in Scenario Planner
description: Quando utilizzi Adobe Workfront Scenario Planner, puoi creare iniziative in un piano che hai creato o che è stato condiviso con te. Creando iniziative è possibile mostrare in che modo le unità organizzative più piccole contribuiscono al completamento del piano. Ad esempio, se l'organizzazione ha un piano per i prossimi tre anni per espandersi in un nuovo mercato, è possibile creare iniziative all'interno di questo piano per ogni reparto per stimare il fabbisogno di risorse umane e di budget di ciascun reparto per realizzare questo piano.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 0%

---

# Crea e modifica iniziative in [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Quando si utilizza [!UICONTROL Adobe Workfront Scenario Planner], è possibile creare iniziative in un piano creato o condiviso con l&#39;utente. Creando iniziative è possibile mostrare in che modo le unità organizzative più piccole contribuiscono al completamento del piano. Ad esempio, se l&#39;organizzazione ha un piano per i prossimi tre anni per espandersi in un nuovo mercato, è possibile creare iniziative all&#39;interno di questo piano per ogni reparto per stimare il fabbisogno di risorse umane e di budget di ciascun reparto per realizzare questo piano.

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
   <td>Prodotto*</td> 
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

## Prerequisiti

È necessario creare un piano oppure un altro utente deve condividere un piano con l&#39;utente prima di poter creare un&#39;iniziativa all&#39;interno del piano. Per informazioni sulla creazione dei piani, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Per ulteriori informazioni sulle iniziative, vedere [Panoramica delle iniziative in [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Creare iniziative

Puoi creare iniziative nei seguenti modi:

* Da zero.
* Importando i progetti in un piano

  Per informazioni sull&#39;importazione di progetti come iniziative in un piano, vedere [Importare progetti in piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Copiando le iniziative esistenti.

  Per informazioni sulla copia delle iniziative, vedere [Copia iniziative in [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Per creare iniziative da zero:

{{step1-to-scenario-planner}}

1. Fare clic sul nome del piano per il quale si desidera creare un&#39;iniziativa.
1. Fai clic sull&#39;icona **+** a sinistra di **[!UICONTROL Nuova iniziativa]**

   Oppure

   Fai clic sul menu a discesa **[!UICONTROL Nuova iniziativa]** e seleziona **[!UICONTROL Nuova iniziativa]** o **[!UICONTROL Importa progetti].**

1. Digita un nome per l&#39;iniziativa nel campo **[!UICONTROL Iniziativa senza titolo]**, quindi premi Invio o fai clic in un altro punto della pagina.

   L’iniziativa viene visualizzata sulla timeline del piano, come una barra blu. Per impostazione predefinita, la durata di un’iniziativa è di un mese e inizia sempre dal primo mese del piano.

1. (Facoltativo) Per ridimensionare il pannello sinistro, trascinate la barra di separazione tra il pannello sinistro e la timeline.

1. (Facoltativo) Trascina la fine della barra dell’iniziativa per estenderne la durata a più di un mese e rilasciala nel punto in cui desideri che si trovi la fine del mese dell’iniziativa.
1. (Facoltativo e condizionale) Se la durata dell&#39;iniziativa è inferiore a quella del piano, trascinare e rilasciare la barra dell&#39;iniziativa in una posizione diversa sulla cronologia del piano, per spostarla in un altro intervallo di tempo.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Puoi selezionare una durata solo in mesi. La durata di un&#39;iniziativa creata da zero non può mai superare la durata del piano.

1. (Facoltativo) Dal menu a discesa **[!UICONTROL Mese]**, selezionare una delle opzioni seguenti per modificare la sequenza temporale del piano:

   | Opzione menu a discesa | Descrizione |
   |---|---|
   | [!UICONTROL Mese] | Visualizza la timeline per mese. Questa è l&#39;opzione predefinita per un piano annuale. |
   | [!UICONTROL Trimestre] | Visualizza la timeline per trimestre. Questa opzione è disponibile solo quando la [!UICONTROL durata] del piano è di 3 o 5 anni. Questa è l&#39;opzione predefinita per un piano triennale. |
   | [!UICONTROL Anno] | Visualizza la timeline per anno. Questa opzione è disponibile solo quando la [!UICONTROL durata] del piano è di 5 anni. Questa è l&#39;opzione predefinita per un piano quinquennale. |


1. (Facoltativo) Scorri da sinistra a destra per visualizzare l’intera durata dell’iniziativa.
1. (Facoltativo) Fai clic sulla riga dell&#39;indicatore **[!UICONTROL Oggi]** per tornare alla data corrente.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Se il piano è futuro o passato e non include la data corrente, l&#39;indicatore Oggi non viene visualizzato.

1. Fai clic sulla barra di un’iniziativa. Il pannello dei dettagli dell’iniziativa si apre a destra.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   Specifica o controlla le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Durata iniziativa</td> 
      <td>La durata dell’iniziativa in mesi. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Date di inizio e fine</td> 
      <td>Le date di inizio e di fine dell’iniziativa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sezione Ruoli richiesti </td> 
      <td> <p>Fare clic sul campo <strong>[!UICONTROL Inizia a digitare la mansione]</strong> e selezionare una mansione dall'elenco oppure iniziare a digitare il nome di una mansione <span>n attiva</span>. </p> <p><span>A seconda che il piano sia impostato per l'utilizzo di FTE o ore,</span> aggiungi il numero di mansioni necessarie per questa iniziativa in FTE <span><span>o ore</span></span><span> per ogni mese nell'iniziativa</span>. <span>Per impostazione predefinita vengono visualizzati i primi tre mesi dell'iniziativa.</span></p> <p><span>L'aggiornamento delle informazioni sulle mansioni per l'iniziativa comporta anche l'aggiornamento delle informazioni sulle mansioni richieste per il piano.</span> </p> <p>Per informazioni sulla configurazione del piano per l'utilizzo di FTE o ore, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani in [!DNL Scenario Planner]</a>. </p>
      <p><b>IMPORTANTE</b></p>  
      <p>Per tutti i calcoli in [!DNL Scenario Planner], [!DNL Workfront] utilizza il seguente valore: 1 FTE = 8 ore. </p>

   <p><b>SUGGERIMENTO</b></p>

   <ul> 
       <li> <p><span>Utilizzare la chiave [!UICONTROL Tab] per passare al mese successivo.</span> </p> </li> 
      <li> <p> Tutti i ruoli di lavoro <span>active</span> nel sistema sono elencati quando si fa clic su questo campo. </p> </li> 
       <li> <p>Vengono visualizzati per primi i ruoli già aggiunti ai ruoli disponibili del piano. Per informazioni sull'aggiunta di mansioni disponibili a un piano, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani nella Pianificazione scenario</a>. </p> </li> 
       <li> <p>[!DNL Workfront] ritiene che un equivalente a tempo pieno sia di 160 ore per un mese. </p> <p>Per tutti i calcoli in Scenario Planner, Workfront utilizza il seguente valore: 1 FTE = 8 ore. </p></li> 
      </ul> </p> <p>È possibile immettere un numero inferiore a 1 FTE o numeri decimali per FTE <span>o</span> <span>ore</span>. Ad esempio, un ruolo di consulente pari a 0,5 significherebbe che un consulente dedicherebbe metà del suo ETP (in genere 4 ore, dove 8 ore sono 1 ETP) a lavorare su questa iniziativa. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Sezione Costi</td> 
      <td> <p>I costi totali dell'iniziativa vengono visualizzati a destra della sezione [!UICONTROL Costs]. [!DNL Workfront] calcola i costi di un'iniziativa utilizzando la formula seguente:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Nel campo <strong>[!UICONTROL Costi fissi]</strong>, immetti manualmente una stima approssimativa dei costi previsti per completare l'iniziativa. Non dovrebbero essere inclusi i costi associati alle mansioni stimate per l'iniziativa.</p> <p><span>Immettere un importo per ogni mese dell'iniziativa spostandosi da un mese all'altro quando si utilizza il tasto TAB.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>A seconda che il piano sia impostato per l'utilizzo di FTE o ore, [!UICONTROL Workfront] utilizza le seguenti formule per calcolare il costo delle persone [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>Quando si utilizzano gli FTE: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, dove 160 è il numero totale di ore lavorative in un mese. </p> </li> 
         <li> <p style="font-weight: normal;">Quando si utilizzano le ore: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Per informazioni sull'impostazione del piano per l'utilizzo di ore o FTE, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani in Pianificazione scenario</a>.</p> </li> 
        </ul> 
        <p>I costi relativi alle persone vengono calcolati nella valuta di base selezionata nelle preferenze Tassi di cambio. Per informazioni sui tassi di cambio, vedere <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Impostare i tassi di cambio</a>.</p> 
        <p>L'aggiornamento delle informazioni sui costi per un'iniziativa aggiorna anche l'area [!UICONTROL Costs] per il piano. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Dopo aver definito la mansione e i valori di costo richiesti per l'iniziativa e aver modificato la durata dell'iniziativa, può verificarsi uno degli scenari seguenti:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Se si riduce l'iniziativa, [!DNL Workfront] rimuove dal piano la quantità di risorse richiesta e i costi associati al tempo di rimozione. Le mansioni rimangono nel piano, ma non hanno FTE richiesto o <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">ore</span>. Le risorse disponibili per il piano e il budget rimangono invariate.<br>Per informazioni aggiornate sul piano, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani in [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Se si rende l'iniziativa più lunga, è necessario specificare la quantità di mansioni e costi per i mesi appena aggiunti sull'iniziativa. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] sezione</td> 
      <td>Nella sezione <strong>[!DNL Net Value]</strong> immettere manualmente un importo approssimativo nel campo <strong>[!UICONTROL Planned Benefit]</strong>. Questo è ciò che, a vostro parere, il vantaggio di realizzare questa iniziativa sarà. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se hai già definito il numero di mansioni e il budget per il tuo piano, nonché il numero di mansioni e i costi dell&#39;iniziativa che stai modificando e di tutte le iniziative al di sopra di essa e tutti superano gli importi specificati per il piano, [!DNL Workfront] potrebbe scoprire che non hai abbastanza risorse per completare l&#39;iniziativa. [!DNL Workfront] contrassegna l&#39;iniziativa come conflitto quando tenta di ottenerla e la visualizza come barra rossa. Tutte le iniziative che seguono l&#39;iniziativa in conflitto vengono visualizzate in rosso. Potrebbe essere necessario adeguare alcune delle esigenze delle iniziative, a partire dalla prima con risorse insufficienti. Per informazioni sulla regolazione delle iniziative in conflitto, vedere [Risolvere i conflitti tra iniziative in  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Facoltativo) Passa il puntatore del mouse sul nome di una mansione, quindi fai clic sull&#39;icona **[!UICONTROL cestino]** ![](assets/delete.png) per rimuoverlo dall&#39;iniziativa.

1. (Condizionale) Se hai apportato modifiche all&#39;iniziativa, fai clic su **[!UICONTROL Applica]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Condizionale) Se non hai apportato modifiche, fai clic sull&#39;icona **X** in alto a destra nel pannello dei dettagli dell&#39;iniziativa per chiuderla.
1. (Facoltativo) Aggiorna la priorità delle iniziative.

   Per informazioni sull&#39;assegnazione delle priorità alle iniziative, vedere [Aggiornare le priorità delle iniziative nella Pianificazione scenario](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Le iniziative elencate per prime nell’elenco hanno una priorità più elevata e ottengono risorse prima di quelle elencate per prime nell’elenco.

1. Fare clic su **[!UICONTROL Salva piano]**.

   L’iniziativa è ora inclusa nel piano.

   Per informazioni sull&#39;eliminazione di iniziative da un piano, vedere [Eliminare iniziative in [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).

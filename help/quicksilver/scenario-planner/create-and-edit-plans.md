---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creare e modificare piani nella Pianificazione scenario
description: È possibile creare piani utilizzando Workfront Scenario Planner quando si assegna la priorità alla strategia di livello superiore della propria azienda. Per ulteriori informazioni sui piani, vedere Panoramica dei piani in Pianificazione scenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '2399'
ht-degree: 0%

---

# Crea e modifica piani in [!DNL Scenario Planner]

È possibile creare piani nell&#39;ambito dell&#39;utilizzo di [!DNL Workfront Scenario Planner], quando si assegna la priorità alla strategia di livello superiore della propria azienda. Per ulteriori informazioni sui piani, vedere [Panoramica dei piani in [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

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
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> </td> 
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
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Creare o modificare i piani

È possibile creare un piano da zero oppure modificare un piano esistente condiviso con l&#39;utente.

>[!NOTE]
>
>Dopo aver creato un piano, l&#39;utente viene considerato il creatore e il proprietario del piano. Quando un utente viene disattivato, il piano non ha alcun proprietario e non è visibile a nessuno a meno che non sia stato condiviso in precedenza con un collegamento.

In questo articolo viene descritto come creare un piano da zero o come modificarne uno esistente.

Per tutte le considerazioni sui piani, incluse le informazioni disponibili per un piano, vedere [Panoramica dei piani in [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Per informazioni sull&#39;eliminazione dei piani, vedere [Eliminare i piani in [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Per creare o modificare un piano:

{{step1-to-scenario-planner}}

Un elenco dei piani esistenti creati viene visualizzato in [!DNL Workfront Scenario Planner].

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Filtro]** ![Icona Filtro](assets/filter-icon-34x37.png)nell&#39;angolo superiore destro dell&#39;elenco dei piani e seleziona una delle seguenti opzioni:

   | Filtro | Descrizione |
   |---|---|
   | [!UICONTROL Tutti] | Visualizza tutti i piani creati o condivisi con l&#39;utente. |
   | [!UICONTROL I miei piani] | Visualizza i piani creati. |
   | [!UICONTROL Condiviso con me] | Visualizza i piani condivisi con l&#39;utente. |

   ![Pianifica le opzioni del menu a discesa dei filtri](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Ricerca]** ![Icona Ricerca](assets/search-icon.png) per digitare una parola chiave e individuare rapidamente un piano nell&#39;elenco.

1. Fare clic sul nome di un piano esistente per modificarlo e continuare con il passaggio 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Oppure

   Fare clic su **[!UICONTROL Nuovo piano]** nell&#39;angolo superiore sinistro per creare un piano e continuare con il passaggio 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![Pulsante Nuovo piano](assets/new-plan-button.png)

   Viene visualizzata la casella [!UICONTROL Nuovo piano].

   ![Nuova finestra del piano](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Condizionale) Quando si crea un piano, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Digitare un nome per il piano. Questo è un campo obbligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Importante: <span style="font-weight: normal;">Impossibile modificare le selezioni seguenti dopo la creazione e il salvataggio del piano.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Equivalente Tempo Pieno]) o [!UICONTROL Ore]</span> </td> 
      <td> <p><span>Selezionare una delle opzioni seguenti per indicare come si desidera stimare le informazioni sul ruolo per questo piano:</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. </span> predefinito </p> 
      <p><b>IMPORTANTE</b></p>  
      <p>Per tutti i calcoli in [!DNL Scenario Planner], [!DNL Workfront] utilizza il seguente valore: 1 FTE = 8 ore. </p> </li> 
      <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p><b>IMPORTANTE</b></p>

   L&#39;opzione selezionata in questo campo determina la modalità di visualizzazione delle informazioni sul ruolo per il piano, gli scenari del piano e le iniziative</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data di inizio]</td> 
      <td> <p>Selezionare il mese e l'anno in cui si desidera che inizi il piano. In questo campo è possibile selezionare solo mesi. [!DNL Workfront] presuppone che la data di inizio del piano sia il primo giorno del mese selezionato e che la data di fine sia l'ultimo giorno della fine del mese nella sua durata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duration]</td> 
      <td> <p>Dal menu a discesa, seleziona una delle seguenti durate:</p> 
       <ul> 
        <li>1 anno. Questa è la durata predefinita. </li> 
        <li>3 anni</li> 
        <li> <p>5 anni</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Condizionale) Fai clic su **[!UICONTROL Avanti]**.

   La sequenza temporale del piano viene visualizzata come **[!UICONTROL scenario iniziale]**.

   Per informazioni sulla creazione di scenari aggiuntivi, vedere [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facoltativo) Dal menu a discesa della timeline, selezionate una delle opzioni della tabella seguente per modificare la modalità di visualizzazione della timeline del piano.

   ![Menu a discesa Mese](assets/month-dropdown-with-all-options.png)

   | Opzione menu a discesa | Descrizione |
   |---|---|
   | [!UICONTROL Mese] | Visualizza la timeline per mese. Questa è l&#39;opzione predefinita e unica per un piano annuale. |
   | [!UICONTROL Trimestre] | Visualizza la timeline per trimestre. Questa opzione è disponibile solo quando la [!UICONTROL durata] del piano è di 3 o 5 anni. Questa è l&#39;opzione predefinita per un piano triennale. |
   | [!UICONTROL Anno] | Visualizza la timeline per anno. Questa opzione è disponibile solo quando la [!UICONTROL durata] del piano è di 5 anni. Questa è l&#39;opzione predefinita per un piano quinquennale. |

1. (Facoltativo) Scorri da sinistra a destra per visualizzare l’intera durata del piano.
1. (Facoltativo) Fai clic sulla riga dell&#39;indicatore **[!UICONTROL Oggi]** per tornare al giorno corrente.

   ![Indicatore oggi](assets/today-indicator-350x160.png)

1. Fare clic sulla casella **[!UICONTROL Ruoli]** nell&#39;intestazione del piano per aggiungere i ruoli disponibili per l&#39;esecuzione del piano.

   Vengono visualizzati i dettagli della casella [!UICONTROL Ruoli].

   >[!TIP]
   >
   >L&#39;unità di allocazione dei ruoli (FTE o ore) utilizzata da [!DNL Workfront] per questo piano viene visualizzata tra parentesi nel titolo della casella.

   ![Aggiunta di persone al piano](assets/adding-people-to-plan-350x206.png)

1. Fare clic sul campo **[!UICONTROL Inizia a digitare la mansione]** e selezionare una mansione dall&#39;elenco oppure iniziare a digitare il nome di una mansione attiva.

   Tutti i ruoli di lavoro attivi nel sistema vengono elencati quando si fa clic su questo campo.

   In questo modo il ruolo viene aggiunto alla colonna Ruoli.

1. Aggiorna o controlla le seguenti informazioni per la mansione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (per FTE) </p> <p role="rowheader">oppure </p> <p role="rowheader"><span>[!UICONTROL Totale disponibile] (per ore)</span> </p> </td> 
      <td> <p><span>A seconda che si sia scelto di utilizzare le ore o l'FTE per il piano, digitare</span> il numero di FTE dei ruoli <span>o le ore</span> disponibili per eseguire il lavoro sul piano nei campi seguenti: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Totale disponibile]</strong> (per ore): indicare il numero totale di ore per tutti i mesi durante la durata dello scenario. Per impostazione predefinita, [!DNL Workfront] divide il numero totale disponibile in parti uguali in tutti i mesi della durata dello scenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se si immettono 1200 ore per un Designer, questo significa che il Designer è disponibile per 100 ore per ogni mese durante la durata del piano, quando la durata del piano [!UICONTROL Duration] è di 1 anno. </p> </li> 
        <li> <p><b>[!UICONTROL Max available]</b> (per FTE): indicare il numero di FTE disponibili per ogni mese della mansione per la durata del piano. Per impostazione predefinita, <strong>Workfront</strong> assegna il numero [!UICONTROL Max available] a ogni mese della durata dello scenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se si immette 1 FTE per un consulente, questo significa che il consulente è disponibile per 1 FTE per ogni mese durante la durata del piano. </p> <p>È possibile immettere un numero inferiore a 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Un ruolo di consulente 0,5 significa che un consulente dedicherebbe metà del proprio FTE (in genere, 4 ore, dove 8 ore sono 1 FTE) al lavoro su questo piano. Per tutti i calcoli in Scenario Planner, Workfront utilizza il seguente valore: 1 FTE = 8 ore. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max obbligatorio] (per FTE)</p> <p role="rowheader">oppure </p> <p role="rowheader"><span>[!UICONTROL Totale richiesto] (per ore)</span> </p> </td> 
      <td> <p><span>A seconda che si sia scelto di utilizzare le ore o l'FTE per il piano, rivedere</span> il numero di FTE dei ruoli <span>o le ore</span> necessarie per completare le iniziative nello scenario. Esamina i campi seguenti:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total required]</strong> (per ore): numero totale di ore richieste per tutti i mesi durante la durata del piano.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (per FTE): numero massimo di FTE richiesti per uno qualsiasi dei mesi durante la durata del piano. </p> </li> 
       </ul> <p>Suggerimento: il numero <span>massimo</span> di FTE <span> o il numero totale di ore</span> richiesti per quella mansione viene visualizzato dopo l'inizio dell'aggiunta delle iniziative. Per informazioni sull'aggiunta di iniziative a un piano, vedere <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Creare e modificare le iniziative in [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tariffa oraria]</td> 
      <td> <p>Tariffa [!UICONTROL Cost Hour] per la mansione. La tariffa oraria viene visualizzata nella valuta del sistema. Per informazioni sulla configurazione dei tassi di cambio per il sistema, vedere <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Impostare i tassi di cambio</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Passa il puntatore del mouse sul nome di una mansione o fai clic sulla scheda dopo aver aggiornato le informazioni sul ruolo, quindi fai clic sull&#39;icona **[!UICONTROL cestino]** ![icona Elimina](assets/delete.png) per rimuoverlo dal piano.
1. Fare clic su **[!UICONTROL Distribuzione mansioni]**.

   Il pannello Distribuzione mansione viene visualizzato per tutti i mesi della durata dello scenario.

   ![Distribuzione mensile mansioni](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Digitare il nome di una mansione per aggiungerla al piano nel campo **[!UICONTROL Inizia a digitare la mansione]**, quindi fare clic su Invio quando viene visualizzato nell&#39;elenco. Questa operazione aggiunge la mansione alla colonna [!UICONTROL Ruoli].
1. Aggiorna o controlla le seguenti informazioni per ogni mese dello scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ruoli] (FTE o Ore)</td> 
      <td>Sia il ruolo disponibile per lo scenario che quelli necessari per le iniziative sullo scenario vengono visualizzati nel pannello Distribuzione ruolo. È indicato se le stime dei ruoli sono in FTE o in ore nell’intestazione della colonna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponibile] (max &lt;numero di FTE&gt;) </p> 
       <div> 
        <p>oppure</p> 
        <p>[!UICONTROL Disponibile] (totale &lt;numero di ore&gt;) </p> 
       </div> </td> 
      <td> <p><span>A seconda che si sia scelto di utilizzare le ore o l'FTE per il piano, rivedere o aggiornare</span> il numero mensile di FTE dei ruoli <span>o le ore</span> disponibili per lo scenario nei campi seguenti:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponibile] (max &lt;numero di FTE&gt;)</strong>: il numero tra parentesi indica il numero massimo di ruoli disponibili per uno qualsiasi dei mesi per lo scenario. Rivedi o aggiorna il numero di FTE per ogni mese dello scenario. La modifica dell’allocazione mensile potrebbe aggiornare il numero di FTE tra parentesi. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Disponibile] (totale &lt;numero di ore&gt;)</strong>: il numero tra parentesi indica il numero totale di ore disponibili per tutti i mesi dello scenario. Rivedi o aggiorna il numero di ore per ogni mese dello scenario. La modifica dell'allocazione mensile aggiorna il numero di ore tra parentesi.</span> </p> </li> 
       </ul> <p>L’aggiornamento manuale delle allocazioni mensili dei ruoli è un altro modo per risolvere i conflitti di ruoli tra le iniziative sullo scenario. </p> <p>Suggerimento   <p><span>Per aggiornare la disponibilità mensile dei ruoli per diversi mesi, digitare il numero di ore o FTE nel campo [!UICONTROL Available] di un mese, quindi trascinare l'angolo del campo sui mesi adiacenti per copiare lo stesso valore per ogni mese. Rilascialo per aggiornare tutti i mesi.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Obbligatorio] (max &lt;numero&gt;)</p> 
       <div> 
        <p role="rowheader">oppure</p> 
        <p role="rowheader">[!UICONTROL Obbligatorio] (totale &lt;numero&gt;)</p> 
       </div> </td> 
      <td> <p><span>A seconda che si sia scelto di utilizzare le ore o l'FTE per il piano, esaminare</span> il numero mensile di FTE dei ruoli o le ore richieste per lo scenario nei campi seguenti: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Obbligatorio] (max &lt;numero di FTE&gt;)</strong>: il numero tra parentesi indica il numero massimo di ruoli richiesti per uno qualsiasi dei mesi per lo scenario. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Richiesto] (totale &lt;numero di ore&gt;)</strong>: il numero tra parentesi indica il numero totale di ore richieste per tutti i mesi dello scenario.</span> </p> </li> 
       </ul> <p>Suggerimento: non è possibile modificare il numero richiesto di FTE <span>o ore</span> per la mansione. Questo numero viene popolato per lo scenario dopo che hai iniziato ad aggiungere iniziative e i relativi requisiti di mansione. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>Differenza mensile tra la quantità di mansioni richieste e disponibili per lo scenario. [!DNL Workfront] calcola la differenza per ogni mansione per ogni mese utilizzando la formula seguente:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in FTE o ore) </p> 
        <p>Suggerimento: quando la differenza visualizza un numero negativo, lo scenario richiede un numero di mansioni superiore a quello disponibile nel piano. Risorse sovrassegnate. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilization] %</td> 
      <td> 
       <div> 
        <p>La percentuale di utilizzo mostra il numero di ruoli disponibili effettivamente utilizzati (o richiesti) nelle iniziative dello scenario. </p> 
        <p>[!DNL Workfront] calcola l'utilizzo per ruolo al mese utilizzando la formula seguente: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>La percentuale di utilizzo potrebbe essere visualizzata nei colori seguenti, a seconda dell’allocazione delle risorse:</p> 
        <ul> 
         <li> <p><b>Verde</b>: i numeri di ruoli disponibili e richiesti corrispondono. Le risorse sono completamente assegnate e la percentuale di utilizzo è del 100%. </p> </li> 
         <li> <p><b>Rosso</b>: sono presenti più ruoli richiesti di quelli disponibili nel piano. Le risorse sono sovrassegnate e la percentuale di utilizzo è superiore al 100%.</p> </li> 
         <li> <p><b>Blu</b>: sono disponibili più mansioni di quante siano richieste. Le risorse sono sottoassegnate e la percentuale di utilizzo è inferiore al 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Applica]** per salvare la distribuzione mensile delle mansioni

   Oppure

   Fare clic su **[!UICONTROL Annulla]** per chiudere la lista di distribuzione dei ruoli e tornare allo scenario.

1. Fare clic sulla casella **[!UICONTROL Dati finanziari]** nell&#39;intestazione del piano per aggiungere il budget per il piano.

   Vengono visualizzati i dettagli della casella [!UICONTROL Financial].

   >[!TIP]
   >
   >La valuta utilizzata da [!DNL Workfront] per questo piano viene visualizzata tra parentesi nel titolo della casella.

1. Specifica il **[!UICONTROL budget annuale]**.

   >[!NOTE]
   >
   >Se il piano si estende su più anni, è necessario specificare un importo di budget per ogni anno.

1. Premi Invio per salvare il budget annuale, quindi [!UICONTROL Scheda] per passare all&#39;anno successivo.

   Il budget annuale viene distribuito automaticamente in parti uguali per ogni mese dell&#39;anno selezionato.

1. Fai clic su **[!UICONTROL Avanzate]** per visualizzare la distribuzione del budget mensile. I bilanci annuali e mensili sono sempre numeri arrotondati. Quando l&#39;importo del budget non può essere distribuito equamente a tutti i mesi entro un anno a causa di decimali, viene visualizzato un indicatore **[!UICONTROL Rimanente]** sotto la distribuzione del budget annuale.

   ![Collegamenti avanzati e rimanenti](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Adeguare manualmente i budget mensili per eliminare gli importi in eccesso.

   Quando il totale di tutti gli importi di budget mensili è maggiore del budget annuale, viene visualizzato un indicatore di avvertenza **[!UICONTROL Eccedente]** nella distribuzione del budget annuale. Adeguare manualmente gli importi di budget mensili finché non sono uguali o inferiori al budget disponibile per il piano.

   ![Avviso di superamento del budget](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Disattiva l&#39;impostazione **[!UICONTROL Includi costi persone]** per escludere i costi associati alle mansioni dal conteggio del costo complessivo del piano. I costi fissi vengono sempre conteggiati nel costo complessivo del piano. Questa impostazione è attivata per impostazione predefinita e influisce su tutti gli scenari del piano.
1. Fare clic in un punto qualsiasi all&#39;esterno della casella [!UICONTROL Financial] per chiuderla. Le informazioni immesse vengono salvate automaticamente.

   Ora puoi iniziare a creare le iniziative sul piano e aggiungere scenari.

1. (Consigliato) Fai clic su **[!UICONTROL Nuova iniziativa]** per aggiungere una nuova iniziativa.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Per informazioni sull&#39;aggiunta di iniziative, vedere l&#39;articolo [Creare e modificare le iniziative in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facoltativo) Creare una copia dello scenario esistente per creare uno scenario dello stesso piano. Per ulteriori informazioni sulla creazione e l&#39;utilizzo di più scenari, vedere [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Fare clic su **[!UICONTROL Salva piano]**.

   Il piano viene creato o aggiornato.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Preferiti]** ![Preferiti](assets/favorites-icon-small.png) a destra del nome del piano per aggiungere il piano all&#39;elenco dei preferiti.

1. (Facoltativo) Copiare l&#39;URL del piano e inviarlo a qualsiasi altro utente che potrebbe avere bisogno di rivederlo o aggiornarlo. Per poter visualizzare il piano, devono disporre di almeno l&#39;accesso [!UICONTROL Visualizzazione] nel proprio livello di accesso. Devono avere l&#39;accesso [!UICONTROL Modifica] per modificarlo. Se devono esaminare le informazioni finanziarie sul piano, ad esempio le informazioni su budget, costi e tassi di ruolo, devono avere accesso anche a [!UICONTROL Dati finanziari] nel proprio livello di accesso. Per informazioni sull&#39;accesso necessario per [!DNL Scenario Planner], vedere [Accesso necessario per utilizzare  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

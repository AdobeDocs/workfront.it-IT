---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creare e modificare i piani nel planner dello scenario
description: È possibile creare piani nell'ambito dell'utilizzo di Workfront Scenario Planner per assegnare una priorità alla strategia di livello superiore della tua azienda. Per ulteriori informazioni sui piani, vedere la panoramica dei piani in Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '2401'
ht-degree: 1%

---

# Crea e modifica piani in [!DNL Scenario Planner]

Puoi creare piani come parte dell&#39;utilizzo di [!DNL Workfront Scenario Planner], per assegnare la priorità alla strategia di livello superiore della tua azienda. Per ulteriori informazioni sui piani, consulta [Panoramica dei piani in [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!UICONTROL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurazioni a livello di accesso* </td> 
   <td> <p>Accesso o superiore a [!DNL Scenario Planner]</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>[!DNL Manage] autorizzazioni a un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare o modificare piani

Puoi creare un piano da zero o modificarne uno esistente condiviso con te.

>[!NOTE]
>
>Dopo aver creato un piano, si viene considerati il creatore e proprietario del piano. Quando un utente è disattivato, il piano non ha alcun proprietario e non è visibile a nessuno a meno che non sia stato precedentemente condiviso con un collegamento.

Questo articolo descrive come creare un piano da zero o modificarne uno esistente.

Per tutte le considerazioni sui piani, comprese le informazioni disponibili per un piano, vedi [Panoramica dei piani in [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Per informazioni sull&#39;eliminazione dei piani, vedere [Elimina i piani nel [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Per creare o modificare un piano:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Un elenco dei piani esistenti creati viene visualizzato in [!DNL Workfront Scenario Planner].

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Filtro]** icona ![](assets/filter-icon-34x37.png)nell&#39;angolo in alto a destra dell&#39;elenco dei piani e selezionare una delle seguenti opzioni:

   | Filtro | Descrizione |
   |---|---|
   | [!UICONTROL Tutti] | Visualizza tutti i piani creati o condivisi con te. |
   | [!UICONTROL I miei piani] | Visualizza i piani creati. |
   | [!UICONTROL Condivisi con me] | Visualizza i piani condivisi con te. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Ricerca]** icona ![](assets/search-icon.png) per digitare una parola chiave e individuare rapidamente un piano nell&#39;elenco.

1. Fare clic sul nome di un piano esistente per modificarlo e continuare con il passaggio 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Oppure

   Fai clic su **[!UICONTROL Nuovo piano]** nell’angolo in alto a sinistra per creare un piano e continuare con il passaggio 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   La [!UICONTROL Nuovo piano] viene visualizzata la casella .

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Condizionale) Quando crei un nuovo piano, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Digitare un nome per il piano. Questo è un campo obbligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Importante: <span style="font-weight: normal;">Non è possibile modificare le selezioni seguenti dopo aver creato e salvato il piano.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Full Time Equivalent]) o [!UICONTROL Hours]</span> </td> 
      <td> <p><span>Selezionare una delle opzioni seguenti per indicare come si desidera stimare le informazioni sul ruolo del lavoro per questo piano:</span> </p> 
       <ul> 
        <li> <p><span><strong>FTE</strong>. Questa è l'impostazione predefinita </span> </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>
         --> <p>Per tutti i calcoli nel [!DNL Scenario Planner], [!DNL Workfront] utilizza il seguente valore: 1 ETP = 8 ore. </p> </li> 
        <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p>Importante: <span>L'opzione selezionata qui determina il modo in cui vengono visualizzate le informazioni sul ruolo del lavoro per il piano, gli scenari del piano e le iniziative.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data di inizio]</td> 
      <td> <p>Selezionare il mese e l'anno in cui si desidera avviare il piano. In questo campo è possibile selezionare solo mesi. [!DNL Workfront] presuppone che la data di inizio del piano sia il primo giorno del mese selezionato e che la data di fine sia l’ultimo giorno della fine del mese nella sua durata. </p> </td> 
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

1. (Condizionale) Fai clic su **[!UICONTROL Successivo]**.

   La timeline del piano viene visualizzata come **[!UICONTROL Scenario iniziale]**.

   Per informazioni sulla creazione di scenari aggiuntivi, consulta [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facoltativo) Dal menu a discesa della timeline, seleziona una delle opzioni nella tabella seguente per modificare la modalità di visualizzazione della timeline del piano.

   ![](assets/month-dropdown-with-all-options.png)

   | Opzione del menu a discesa | Descrizione |
   |---|---|
   | [!UICONTROL Mese] | Visualizza la timeline per mese. Questa è l&#39;opzione predefinita e l&#39;unica opzione per un piano di un anno. |
   | [!UICONTROL Trimestre] | Visualizza la timeline per trimestre. Questa opzione è disponibile solo quando [!UICONTROL Durata] del piano è di 3 o 5 anni. Questa è l’opzione predefinita per un piano a 3 anni. |
   | [!UICONTROL Anno] | Visualizza la timeline per anno. Questa opzione è disponibile solo quando [!UICONTROL Durata] del piano è di 5 anni. Questa è l’opzione predefinita per un piano quinquennale. |

1. (Facoltativo) Scorri da sinistra a destra per visualizzare l’intera durata del piano.
1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Oggi]** linea dell&#39;indicatore per tornare al giorno corrente.

   ![](assets/today-indicator-350x160.png)

1. Fai clic sul pulsante **[!UICONTROL Ruoli processo]** nell&#39;intestazione del piano per aggiungere i ruoli di lavoro disponibili per l&#39;esecuzione del piano.

   I dettagli della [!UICONTROL Ruoli processo] visualizzazione delle caselle.

   >[!TIP]
   >
   >L’unità di allocazione del ruolo (FTE o ore) che [!DNL Workfront] gli utilizzi di questo piano vengono visualizzati tra parentesi nel titolo della casella.

   ![](assets/adding-people-to-plan-350x206.png)

1. Fai clic sul pulsante **[!UICONTROL Inizia a digitare il ruolo]** selezionare un ruolo dall&#39;elenco o iniziare a digitare il nome di un ruolo di processo attivo.

   Quando si fa clic su questo campo, vengono elencati tutti i ruoli di lavoro attivi nel sistema.

   Questo aggiunge il ruolo del processo alla colonna Ruoli processo.

1. Aggiornare o rivedere le seguenti informazioni per il ruolo del processo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (per FTE) </p> <p role="rowheader">oppure </p> <p role="rowheader"><span>[!UICONTROL Totale disponibile] (per ore)</span> </p> </td> 
      <td> <p><span>A seconda che sia stata selezionata l’opzione per l’utilizzo di ore o FTE per il piano, digitare</span> il numero di FTE per il ruolo di lavoro <span>o ore</span> disponibili per eseguire i lavori sul piano nei campi seguenti: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Totale disponibile]</strong> (per ore): Indicare il numero totale di ore per tutti i mesi durante la durata dello scenario. Per impostazione predefinita, [!DNL Workfront] divide in parti uguali il numero totale disponibile per tutti i mesi della durata dello scenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se si immettono 1200 ore per un Designer, ciò significa che Designer è disponibile per 100 ore al mese per ogni mese durante la durata del piano, quando il piano [!UICONTROL Duration] è di 1 anno. </p> </li> 
        <li> <p><b>[!UICONTROL Max available]</b> (per FTE): Indicare il numero di FTE per cui il ruolo di lavoro è disponibile per ogni mese durante la durata del piano. Per impostazione predefinita, <strong>Workfront</strong> assegna il numero [!UICONTROL Max available] a ogni mese nella durata dello scenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se si inserisce 1 ETP per un Consulente, ciò significa che il Consulente è disponibile per 1 ETP per ogni mese durante la durata del piano. </p> <p>È possibile immettere un numero inferiore a 1 ETP. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Un ruolo di consulente di 0.5 significherebbe che un consulente dedicherebbe metà del proprio ETP (tipicamente, 4 ore, dove 8 ore è 1 ETP) a lavorare su questo piano. Per tutti i calcoli nel Planner scenario, Workfront utilizza il seguente valore: 1 ETP = 8 ore. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max required] (per FTE)</p> <p role="rowheader">oppure </p> <p role="rowheader"><span>[!UICONTROL Totale richiesto] (per ore)</span> </p> </td> 
      <td> <p><span>A seconda che sia stato selezionato per utilizzare ore o FTE per il piano, rivedi</span> il numero di FTE per il ruolo di lavoro <span>o ore</span> necessari per completare le iniziative nello scenario. Esamina i campi seguenti:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Totale richiesto]</strong> (per ore): Numero totale di ore richieste per tutti i mesi durante la durata del piano.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (per FTE): Numero massimo di ETP richiesti per uno qualsiasi dei mesi durante la durata del piano. </p> </li> 
       </ul> <p>Suggerimento: La <span>massimo</span> numero di ETP <span>o il numero totale di ore</span> necessario per quel ruolo di lavoro viene visualizzato dopo aver iniziato ad aggiungere iniziative. Per informazioni sull’aggiunta di iniziative a un piano, consulta <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Creare e modificare iniziative in [!DNL Scenario Planner]</a>.</p> </td> 
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
      <td> <p>Questo è il tasso di [!UICONTROL Cost Hour] per il ruolo di lavoro. Il tasso orario viene visualizzato nella valuta del sistema. Per informazioni sull'impostazione dei tassi di cambio per il sistema, vedere <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Passa il puntatore del mouse sul nome di un ruolo di lavoro o fai clic sulla scheda dopo aver aggiornato le informazioni sul ruolo, quindi fai clic sul pulsante **[!UICONTROL icona cestino]** ![](assets/delete.png) per rimuoverlo dal piano.
1. Fai clic su **[!UICONTROL Distribuzione del ruolo del lavoro]**.

   Il pannello di distribuzione del ruolo di lavoro viene visualizzato per tutti i mesi nella durata dello scenario.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Digitare il nome di un ruolo di lavoro da aggiungere al piano nel **[!UICONTROL Inizia a digitare il campo del ruolo del lavoro]**, quindi fai clic su Invio quando viene visualizzato nell’elenco. Questo aggiunge il ruolo del lavoro al [!UICONTROL Ruoli processo] colonna.
1. Aggiorna o rivedi le seguenti informazioni per ogni mese dello scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ruoli processo] (FTE o ore)</td> 
      <td>Sia il ruolo di lavoro disponibile per lo scenario che quelli necessari per le iniziative sullo scenario vengono visualizzati nel pannello di distribuzione dei ruoli di lavoro. È presente un’indicazione che le stime dei ruoli di lavoro sono in FTE o ore nell’intestazione della colonna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponibile] (max &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>oppure</p> 
        <p>[!UICONTROL Disponibile] (totale) &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>A seconda che sia stato selezionato di utilizzare ore o FTE per il piano, rivedere o aggiornare</span> il numero mensile di FTE per i ruoli di lavoro <span>o ore</span> disponibile per lo scenario nei campi seguenti:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponibile] (max &lt;number of="" ftes=""&gt;)</strong>: Il numero tra parentesi indica il numero massimo di ruoli disponibili per uno qualsiasi dei mesi per lo scenario. Rivedi o aggiorna il numero di ETP per ogni mese dello scenario. La modifica dell’allocazione mensile potrebbe aggiornare il numero di ETP tra parentesi. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Disponibile] (totale) &lt;number of="" hours=""&gt;)</strong>: Il numero tra parentesi indica il numero totale di ore disponibili per tutti i mesi dello scenario. Rivedere o aggiornare il numero di ore per ogni mese dello scenario. La modifica dell’allocazione mensile aggiorna il numero di ore tra parentesi.</span> </p> </li> 
       </ul> <p>L'aggiornamento manuale delle allocazioni mensili dei ruoli di lavoro è un altro modo per risolvere i conflitti di ruolo tra le iniziative sullo scenario. </p> <p>Suggerimento:   <p><span>Per aggiornare la disponibilità del ruolo mensile per diversi mesi, digita il numero di ore o FTE nel campo [!UICONTROL Disponibile] di qualsiasi mese, quindi trascina l’angolo del campo sui mesi adiacenti per copiare lo stesso valore per ogni mese. Rilascia per aggiornare tutti i mesi.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Obbligatorio] (max &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">oppure</p> 
        <p role="rowheader">[!UICONTROL Obbligatorio] (totale) &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>A seconda che sia stato selezionato per utilizzare ore o FTE per il piano, rivedi</span> il numero mensile di FTE o ore dei ruoli di lavoro richiesti per lo scenario nei campi seguenti: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Obbligatorio] (max &lt;number of="" ftes=""&gt;)</strong>: Il numero tra parentesi indica il numero massimo di ruoli richiesti per uno qualsiasi dei mesi per lo scenario. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Obbligatorio] (totale) &lt;number of="" hours=""&gt;)</strong>: Il numero tra parentesi indica il numero totale di ore necessarie per tutti i mesi dello scenario.</span> </p> </li> 
       </ul> <p>Suggerimento: Non è possibile modificare il numero richiesto di FTE <span>o ore</span> per il ruolo di lavoro. Questo numero viene compilato per lo scenario dopo aver iniziato ad aggiungere iniziative e i relativi requisiti di ruolo del lavoro. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>Differenza mensile tra gli importi dei ruoli di lavoro richiesti e disponibili per lo scenario. [!DNL Workfront] calcola la differenza per ogni ruolo di lavoro per ogni mese utilizzando la seguente formula:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in ETP o ore) </p> 
        <p>Suggerimento: Quando la differenza visualizza un numero negativo, lo scenario richiede più ruoli di lavoro di quelli disponibili nel piano. Le risorse sono sovrassegnate. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilizzazione] %</td> 
      <td> 
       <div> 
        <p>La percentuale di utilizzo indica quanti dei ruoli di lavoro disponibili vengono effettivamente utilizzati (o richiesti) sulle iniziative nello scenario. </p> 
        <p>[!DNL Workfront] calcola l'utilizzo per ruolo di lavoro al mese utilizzando la seguente formula: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>La percentuale di utilizzo può essere visualizzata nei seguenti colori, a seconda dell’allocazione delle risorse:</p> 
        <ul> 
         <li> <p><b>Verde</b>: Il numero di ruoli di lavoro disponibili e richiesti corrisponde. Le risorse sono completamente assegnate e la percentuale di utilizzo è del 100%. </p> </li> 
         <li> <p><b>Rosso</b>: Ci sono più ruoli di lavoro richiesti di quelli disponibili nel piano. Le risorse sono sovrassegnate e la percentuale di utilizzo è superiore al 100%.</p> </li> 
         <li> <p><b>Blu</b>: Ci sono più ruoli di lavoro disponibili di quelli richiesti. Le risorse sono sottoassegnate e la percentuale di utilizzo è inferiore al 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Applica]** per salvare la distribuzione mensile dei ruoli di lavoro

   Oppure

   Fai clic su **[!UICONTROL Annulla]** per chiudere la lista di distribuzione dei ruoli di lavoro e tornare allo scenario.

1. Fai clic sul pulsante **[!UICONTROL Finanziario]** nell&#39;intestazione del piano, aggiungere il budget per questo piano.

   I dettagli della [!UICONTROL Finanziario] visualizzazione delle caselle.

   >[!TIP]
   >
   >La valuta che [!DNL Workfront] gli utilizzi di questo piano vengono visualizzati tra parentesi nel titolo della casella.

1. Specifica la **[!UICONTROL Bilancio annuale]**.

   >[!NOTE]
   >
   >Se il piano si estende per più anni, è necessario specificare un importo di budget per ogni anno.

1. Premere Invio per salvare il budget annuale, quindi [!UICONTROL Scheda] per passare all&#39;anno successivo.

   Il bilancio annuale viene automaticamente distribuito in modo uniforme per ogni mese dell&#39;anno selezionato.

1. Fai clic su **[!UICONTROL Avanzate]** per visualizzare la distribuzione mensile del budget. I bilanci annuali e mensili sono sempre arrotondati. Quando l&#39;importo di bilancio non può essere distribuito equamente a tutti i mesi entro un anno a causa dei decimali **[!UICONTROL Rimanente]** viene visualizzato sotto la distribuzione del budget annuale.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Adeguare manualmente i budget mensili per eliminare gli importi in eccesso.

   Quando il totale di tutti gli importi mensili del bilancio è superiore al bilancio annuale, **[!UICONTROL superiore]** l&#39;indicatore di avviso viene visualizzato sotto la distribuzione del budget annuale. Adeguare manualmente gli importi di budget mensili fino a quando non sono uguali o inferiori al budget disponibile per il piano.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Disattiva la **[!UICONTROL Includi costi per le persone]** impostazione per escludere i costi associati ai ruoli di lavoro dal conteggio verso il costo complessivo del piano. I costi fissi contano sempre per il costo complessivo del piano. Questa impostazione è abilitata per impostazione predefinita e interessa tutti gli scenari del piano.
1. Fai clic in un punto qualsiasi al di fuori del [!UICONTROL Finanziario] per chiuderlo. Le informazioni inserite vengono salvate automaticamente.

   Ora puoi iniziare a creare le iniziative sul piano e aggiungere scenari.

1. (Consigliato) Fai clic su **[!UICONTROL Nuova iniziativa]** aggiungere una nuova iniziativa.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Per informazioni sull’aggiunta di iniziative, consulta l’articolo [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facoltativo) Fare una copia dello scenario esistente per creare un nuovo scenario dello stesso piano. Per ulteriori informazioni sulla creazione e l’utilizzo di più scenari, consulta [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Fai clic su **[!UICONTROL Salva piano]**.

   Il piano viene creato o aggiornato.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Icona Preferiti]** ![](assets/favorites-icon-small.png) a destra del nome del piano per aggiungere il piano all&#39;elenco dei Preferiti.

1. (Facoltativo) Copia l’URL del piano e invialo a qualsiasi altro utente che potrebbe dover rivederlo o aggiornarlo. Devono avere almeno [!UICONTROL Visualizza] accesso al loro livello di accesso per poter visualizzare il piano. Devono avere [!UICONTROL Modifica] accedere per modificarlo. Se devono rivedere le informazioni finanziarie sul piano, come i budget, i costi e le informazioni sui tassi di ruolo del lavoro, devono avere accesso anche a [!UICONTROL Dati finanziari] nel livello di accesso. Per informazioni sull&#39;accesso necessario per [!DNL Scenario Planner], vedi [Accesso necessario per utilizzare [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Panoramica delle iniziative nel planner dello scenario
description: Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni sul planner scenario di Workfront, vedere Panoramica del planner scenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Panoramica delle iniziative in [!DNL Scenario Planner]

La [!DNL Scenario Planner] è disponibile solo nel nuovo [!DNL Adobe Workfront] esperienza e richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi [La [!DNL Scenario Planner] panoramica](../scenario-planner/scenario-planner-overview.md).
In qualità di business manager, puoi creare iniziative per i piani nel [!DNL Adobe Workfront Scenario Planner]. Per informazioni sulla creazione dei piani, consulta l’articolo [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Panoramica delle iniziative

Utilizzo della [!DNL Workfront Scenario Planner], puoi stimare e rivedere le seguenti informazioni per ogni iniziativa:

* Stimare il tipo e il numero di ruoli di lavoro che potrebbero essere necessari per completare l&#39;iniziativa. Questo aggiunge al conteggio del ruolo di lavoro obbligatorio per il piano e calcola i costi delle persone che è possibile esaminare per un&#39;iniziativa.
* Stimare i costi fissi associati al lavoro necessario per completare l&#39;iniziativa.
* Stimare il benefit pianificato che la tua azienda potrebbe ottenere al completamento dell&#39;iniziativa.

Per visualizzare informazioni sulle iniziative, puoi accedere a singole iniziative all’interno di un piano. Per informazioni sulla creazione e l’accesso alle iniziative, consulta l’articolo [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Considerazioni sulle iniziative

Quando crei iniziative, considera quanto segue:

* È necessario creare un piano prima di poter creare un&#39;iniziativa.
* Puoi creare iniziative da zero o importare progetti in un piano. I progetti diventano iniziative nell&#39;ambito del piano.

   Per informazioni sulla creazione di iniziative da zero, consulta [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Per informazioni sull&#39;importazione di progetti in un piano per la creazione di iniziative da progetti, vedere [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Le iniziative sono unità di pianificazione più piccole dei piani e sono create solo come parte di un piano.
* L&#39;iniziativa più breve può avere una durata di 1 mese. L&#39;iniziativa più lunga può avere una durata di 5 anni.
* Non si può lavorare effettivamente su un&#39;iniziativa. A livello di iniziativa, puoi definire le risorse necessarie e il costo che tali risorse dovranno sostenere, in modo da poter iniziare a eseguire una delle richieste del piano. Ad esempio, se la tua azienda prevede di espandere e acquisire un nuovo ufficio in una nuova posizione, il reparto potrebbe avere un&#39;iniziativa per installare l&#39;infrastruttura di rete per tale nuova posizione.
* Puoi creare più iniziative in un piano. Con ogni iniziativa, puoi delineare una strategia di alto livello per eseguire il lavoro nel tuo reparto.
* Puoi assegnare priorità alle iniziative all&#39;interno di un piano, per garantire che l&#39;iniziativa più importante riceva il maggior numero di risorse e di budget.
* Quando si creano iniziative all&#39;interno di un piano, tutti coloro che lo vedono possono anche visualizzare tutte le iniziative all&#39;interno del piano.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Puoi pubblicare le iniziative per creare progetti o per aggiornare i progetti ad essi collegati. Per informazioni sulle iniziative di pubblicazione, vedi [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informazioni finanziarie sulle iniziative

È possibile esaminare le informazioni finanziarie relative alle singole iniziative per capire come le iniziative si adattano al piano. Per informazioni sull&#39;accesso a un&#39;iniziativa, consulta l&#39;articolo [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Puoi visualizzare i seguenti indicatori finanziari su un&#39;iniziativa accedendo all&#39;interno di un piano:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importo totale costi]</td> 
   <td> <p style="font-weight: normal;">Si tratta di un calcolo del costo totale di un'iniziativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcola il valore dei costi totali di un'iniziativa utilizzando questa formula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costi Fissi]</td> 
   <td> <p><span style="font-weight: normal;">Questa è una voce manuale dove è possibile stimare <span>un importo mensile di Costi fissi per ogni mese dell'iniziativa.</span> Questo non include i costi associati ai ruoli aggiunti all’iniziativa che vengono acquisiti nel campo [!UICONTROL People Cost] .</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costi Persone]</td> 
   <td> <p style="font-weight: normal;">Si tratta di un calcolo totale dei costi associati ai ruoli dell'iniziativa per la durata dell'iniziativa. Questo numero dipende dal numero di ETP o ore stimate per un ruolo di lavoro per ogni mese dell’iniziativa. </p> 
     <p><b>SUGGERIMENTI</b>  
     <ul> 
      <li> <p>Il numero di ETP mensili per lo stesso ruolo di lavoro può essere diverso da mese a mese.</p> </li> 
      <li> <p>[!DNL Workfront] ritiene che in un mese vi siano 160 ore di lavoro. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcola i [!UICONTROL People Cost] di un'iniziativa utilizzando la seguente formula:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcola i costi mensili delle persone per ogni mese durante la durata dell'iniziativa utilizzando la seguente formula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>ESEMPIO</b></p>
      <p>Se si dispone di un'iniziativa della durata di 6 mesi che richiede 1 Designer con un tasso orario di $ 50 per 1 ETP al mese e un Web Designer con un tasso orario di $ 100 per 2 mesi dell'iniziativa, i costi delle persone dell'iniziativa vengono calcolati come segue:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vantaggio pianificato]</td> 
   <td>Questa è una voce manuale in cui puoi stimare il beneficio complessivo che il tuo reparto potrebbe trarre completando questa iniziativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importo valore netto]</td> 
   <td> <p style="font-weight: normal;">Questo rappresenta il valore della tua iniziativa quando si tiene conto dei costi complessivi e del beneficio previsto stimato sull'iniziativa. [!DNL Workfront] calcola il valore netto di un'iniziativa utilizzando la seguente formula:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Informazioni di iniziativa nelle relazioni

Puoi visualizzare le informazioni sull’iniziativa nei rapporti, come descritto nella tabella seguente. Queste informazioni sono disponibili nella tua istanza di Workfront solo quando la tua azienda ha acquistato una licenza di Workfront Scenario Planner .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo di rapporto</b></td> 
   <td><b>Informazioni sull'iniziativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Nome, durata, date di inizio e fine, Inserito da, ID, Data ultima pubblicazione*, Tutti i campi del progetto inclusi i campi personalizzati*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Tutte le informazioni dell'iniziativa elencate sopra, ID (Ruolo lavoro), Progetto*, Ora pianificata assegnazione progetto*, Ore del ruolo dell'iniziativa, Conteggio (Ruolo lavoro), Tutti i campi del progetto, compresi i campi personalizzati*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Tutte le informazioni dell'iniziativa elencate sopra*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Questi campi si popolano con le informazioni del progetto collegato all&#39;iniziativa, solo quando l&#39;iniziativa è stata creata da un progetto o è stata pubblicata a un progetto almeno una volta. Per informazioni sulle iniziative di pubblicazione, vedi [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Panoramica delle iniziative nella Pianificazione scenario
description: La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta Panoramica di Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Panoramica delle iniziative in [!DNL Scenario Planner]

In qualità di Business Manager, puoi creare iniziative per i piani in [!DNL Adobe Workfront Scenario Planner]. Per informazioni sulla creazione di piani, vedere l&#39;articolo [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Panoramica delle iniziative

Utilizzando [!DNL Workfront Scenario Planner], puoi stimare e rivedere le seguenti informazioni per ogni iniziativa:

* Stimare il tipo e il numero di mansioni che potrebbero essere necessarie per completare l&#39;iniziativa. In questo modo si aggiunge al conteggio dei ruoli richiesti per il piano e si calcolano i costi delle persone che è possibile esaminare per un&#39;iniziativa.
* Stimare i costi fissi associati al lavoro necessario per completare l&#39;iniziativa.
* Stimare il beneficio pianificato che la tua azienda potrebbe ottenere al termine dell’iniziativa.

Per visualizzare informazioni sulle iniziative, puoi accedere alle singole iniziative all’interno di un piano. Per informazioni sulla creazione e l&#39;accesso alle iniziative, vedere l&#39;articolo [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Considerazioni sulle iniziative

Quando crei iniziative, tieni presente quanto segue:

* È necessario creare un piano prima di poter creare un&#39;iniziativa.
* Puoi creare iniziative da zero oppure importare progetti in un piano. I progetti diventano iniziative nell&#39;ambito del piano.

  Per informazioni sulla creazione dell&#39;iniziativa da zero, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Per informazioni sull&#39;importazione di progetti in un piano per la creazione di iniziative da progetti, vedere [Importare progetti in piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Le iniziative sono unità di pianificazione più piccole rispetto ai piani e vengono create solo come parte di un piano.
* L’iniziativa più breve può avere una durata di 1 mese. L&#39;iniziativa più lunga può avere una durata di 5 anni.
* Non è possibile eseguire operazioni effettive su un&#39;iniziativa. A livello di iniziativa, è possibile definire quali risorse sono necessarie e il costo che tali risorse devono sostenere, in modo da poter iniziare a eseguire una delle domande del piano. Ad esempio, se l&#39;azienda prevede di espandere e acquisire un nuovo ufficio in una nuova posizione, il reparto potrebbe avere un&#39;iniziativa per installare l&#39;infrastruttura di rete per la nuova posizione.
* Puoi creare più iniziative in un piano. Con ogni iniziativa, puoi delineare una strategia di alto livello per portare a termine il lavoro nel tuo reparto.
* Puoi assegnare un ordine di priorità alle iniziative all’interno di un piano, in modo che l’iniziativa più importante riceva il budget e le risorse più importanti.
* Quando si creano iniziative all&#39;interno di un piano, tutti coloro che visualizzano tale piano possono visualizzare anche tutte le iniziative all&#39;interno del piano.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Puoi pubblicare le iniziative per creare progetti o per aggiornare i progetti ad essi collegati. Per informazioni sulla pubblicazione delle iniziative, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informazioni finanziarie sulle iniziative

È possibile esaminare le informazioni finanziarie relative alle singole iniziative per capire in che modo esse si adattano al piano. Per informazioni sull&#39;accesso a un&#39;iniziativa, vedere l&#39;articolo [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Per visualizzare i seguenti indicatori finanziari relativi a un&#39;iniziativa, è possibile accedervi all&#39;interno di un piano:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costi totali]</td> 
   <td> <p style="font-weight: normal;">Si tratta di un calcolo del costo totale di un'iniziativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcola il valore totale dei costi di un'iniziativa utilizzando la formula seguente:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costi Fissi]</td> 
   <td> <p><span style="font-weight: normal;">Questo è un inserimento manuale in cui è possibile stimare <span>un importo mensile di costi fissi per ogni mese dell'iniziativa.</span> Non sono inclusi i costi associati ai ruoli aggiunti all'iniziativa che vengono acquisiti nel campo [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costi Persone]</td> 
   <td> <p style="font-weight: normal;">Calcolo totale dei costi associati ai ruoli dell'iniziativa per la durata dell'iniziativa. Questo numero dipende dal numero di FTE o ore stimato per un ruolo per ogni mese dell’iniziativa. </p> 
     <p><b>SUGGERIMENTI</b>  
     <ul> 
      <li> <p>Il numero di FTE mensili per lo stesso ruolo può essere diverso da un mese all’altro.</p> </li> 
      <li> <p>[!DNL Workfront] ritiene che in un mese vi siano 160 ore lavorative. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcola i [!UICONTROL People Costs] di un'iniziativa utilizzando la formula seguente:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcola i costi mensili delle persone per ogni mese durante la durata dell'iniziativa utilizzando la formula seguente:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>ESEMPIO</b></p>
      <p>Se si dispone di un'iniziativa con una durata di 6 mesi che richiede 1 Designer con una tariffa oraria di 50 $ per 1 ETP ogni mese e un Designer Web con una tariffa oraria di 100 $ per 2 mesi dell'iniziativa, i costi delle persone dell'iniziativa vengono calcolati come segue:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>Si tratta di un inserimento manuale in cui è possibile stimare il beneficio complessivo che il reparto otterrebbe completando questa iniziativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valore Netto]</td> 
   <td> <p style="font-weight: normal;">Rappresenta il valore dell’iniziativa se si considerano i costi complessivi e il beneficio pianificato stimato sull’iniziativa. [!DNL Workfront] calcola il valore netto di un'iniziativa utilizzando la formula seguente:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## Informazioni sulle iniziative nei rapporti

Puoi visualizzare le informazioni sull’iniziativa nei rapporti, come descritto nella tabella seguente. Queste informazioni sono disponibili nella tua istanza di Workfront solo quando la tua azienda ha acquistato una licenza di Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo di rapporto</b></td> 
   <td><b>Informazioni iniziativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Nome, Durata, Date di inizio e fine, Immesso da, ID, Data ultima pubblicazione*, Tutti i campi del progetto, compresi i campi personalizzati*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Tutte le informazioni sull'iniziativa elencate in precedenza, ID (mansione), Progetto*, Ore pianificate assegnazione progetto*, Ore mansione iniziativa, Conteggio (mansione), Tutti i campi del progetto, inclusi i campi personalizzati*</td> 
  </tr> 
  <tr> 
   <td><p>Progetto *</p></td> 
   <td> <p>Tutte le informazioni sull'iniziativa elencate in precedenza*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Questi campi vengono compilati con le informazioni del progetto collegato all’iniziativa, solo quando l’iniziativa è stata creata da un progetto o è stata pubblicata in un progetto almeno una volta. Per informazioni sulla pubblicazione delle iniziative, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

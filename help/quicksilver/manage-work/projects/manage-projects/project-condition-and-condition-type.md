---
title: Panoramica del tipo di condizione e condizione del progetto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condizione del progetto è una rappresentazione visiva dell’avanzamento del progetto. Si tratta di una variabile segnalabile determinata dalla relazione tra le date previste, previste e stimate del progetto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Panoramica del tipo di condizione e condizione del progetto

La condizione del progetto è una rappresentazione visiva dell’avanzamento del progetto. Si tratta di una variabile segnalabile determinata dalla relazione tra le date previste, previste e stimate del progetto.

## Panoramica sulla condizione del progetto

Per comprendere la condizione di un progetto, considera quanto segue:

* In qualità di proprietario del progetto, puoi decidere se impostare manualmente o automaticamente la condizione di un progetto. La condizione di un progetto può essere impostata nei seguenti modi:

   * Manualmente, per gli utenti che hanno accesso a Gestione progetto e quando il Tipo di condizione del progetto è impostato su Manuale.
   * Automaticamente, da Adobe Workfront, quando il tipo di condizione del progetto è impostato su Stato di avanzamento. Lo stato di avanzamento del progetto è determinato dall’avanzamento delle attività del progetto. Per informazioni sullo stato di avanzamento del progetto, consulta [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   Per informazioni su come aggiornare il tipo di condizione del progetto, consulta [Imposta il tipo di condizione di un progetto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Quando Workfront può stimare automaticamente la condizione del progetto, si consiglia di utilizzare i predecessori per le attività in modo che l’avanzamento dell’attività rifletta l’avanzamento effettivo e lo stato di avanzamento del progetto.
* In qualità di proprietario del progetto, è possibile modificare il progetto per utilizzare un tipo di condizione manuale invece di utilizzare lo stato di avanzamento cambiando il tipo di condizione da Stato di avanzamento a Manuale.

   >[!NOTE]
   >
   >I progetti che si trovano in uno dei seguenti stati sono sempre contrassegnati come Su Target, indipendentemente dalle date delle attività e dal relativo avanzamento:
   >
   >* Idea
   >* Richiesto
   >* Approvato
   >* Rifiutato


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Aggiornamento della condizione del progetto da parte di Workfront in base allo stato di avanzamento

Quando il tipo di condizione del progetto è impostato su Manuale, è possibile determinare quale condizione del progetto è indipendente dallo stato di avanzamento del progetto.

Tuttavia, è consigliabile impostare il tipo di condizione del progetto su Stato di avanzamento in modo da avere un’indicazione chiara dell’effettivo avanzamento del progetto, in base all’avanzamento delle attività. Per informazioni sul modo in cui Workfront calcola lo stato di avanzamento dei progetti, consulta [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

In questo caso, i valori per la condizione di progetto possono essere:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Condizione del progetto</td> 
   <td>Stato di avanzamento del progetto</td> 
   <td>Indicatore di condizione Workfront</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Puntuale</td> 
   <td> <li>Quando lo stato di avanzamento del progetto è attivato, la condizione del progetto è <strong>Su Target</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>A Rischio</td> 
   <td>Stato di avanzamento del progetto <strong>Dietro</strong> o <strong>A rischio</strong>, la condizione del progetto è <strong>A rischio</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>In difficoltà</td> 
   <td>Stato di avanzamento del progetto <strong>In ritardo</strong>, la condizione del progetto è <strong>In problemi</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le condizioni possono essere personalizzate per il tuo ambiente, quindi potresti trovare più di tre opzioni per Condition nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli sopra elencati. Per informazioni sulla personalizzazione delle Condizioni in , consulta l’articolo [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapporto sulla condizione del progetto, sull’aggiornamento della condizione del progetto e sulla nota relativa all’ultima condizione

Nella visualizzazione di un rapporto sul progetto, puoi visualizzare i seguenti campi relativi alla condizione del progetto:

* **Condizione del progetto:** Mostra la condizione corrente del progetto.
* **Aggiornamento della condizione del progetto**: Mostra l’aggiornamento più recente fornito dal proprietario del progetto nel flusso di aggiornamento del progetto, insieme alla nuova condizione .\
   I commenti effettuati sugli aggiornamenti della condizione non vengono visualizzati nella **Aggiornamento delle condizioni** colonna; viene visualizzato solo l&#39;aggiornamento principale.

* **Ultima nota sulla condizione**: Visualizza l&#39;ultimo aggiornamento immesso in un oggetto dal proprietario dell&#39;oggetto. Questo campo è utile per visualizzare l&#39;attività o l&#39;interazione più recente del proprietario su un oggetto.\
   La **Ultima nota sulla condizione** Se il testo della nota dell’ultima nota di un oggetto è stato eliminato, la colonna è vuota. Quando una nuova nota viene inserita sull’oggetto, diventa l’ultima nota e viene visualizzata nuovamente nella colonna.

Per informazioni su come creare un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

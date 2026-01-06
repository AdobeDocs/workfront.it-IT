---
title: Panoramica della condizione e del tipo di condizione del progetto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condizione del progetto è una rappresentazione visiva dell’avanzamento del progetto. Si tratta di una variabile da segnalare determinata dalla relazione tra le date pianificate, previste e stimate del progetto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Panoramica della condizione e del tipo di condizione del progetto

<!-- Audited: 12/2023 -->

La condizione del progetto è una rappresentazione visiva dell’avanzamento del progetto. Si tratta di una variabile da segnalare determinata dalla relazione tra le date pianificate, previste e stimate del progetto.

## Panoramica sulla condizione del progetto

Per comprendere le condizioni di un progetto, considera quanto segue:

* In qualità di proprietario del progetto, puoi decidere se impostare manualmente o automaticamente la condizione di un progetto. La condizione di un progetto può essere impostata nei seguenti modi:

   * Manualmente per gli utenti che hanno accesso a Gestisci il progetto e quando il Tipo di condizione del progetto è impostato su Manuale.
   * Automaticamente da Adobe Workfront, quando il Tipo di condizione del progetto è impostato su Stato di avanzamento. Lo stato di avanzamento del progetto è determinato dall&#39;avanzamento delle attività del progetto. Per informazioni sullo stato di avanzamento del progetto, vedere [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Per informazioni su come aggiornare il tipo di condizione del progetto, vedere [Impostare il tipo di condizione di un progetto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Quando si consente a Workfront di stimare automaticamente la condizione del progetto, si consiglia di utilizzare i predecessori nelle attività in modo che l’avanzamento dell’attività si rifletta nell’avanzamento effettivo e nello stato di avanzamento del progetto.
* In qualità di proprietario del progetto, è possibile modificare il progetto in modo da utilizzare un tipo di condizione manuale anziché lo stato di avanzamento cambiando il tipo di condizione da stato di avanzamento a manuale.

  >[!NOTE]
  >
  >I progetti che si trovano in uno dei seguenti stati sono sempre contrassegnati come On Target, indipendentemente dalle date delle attività e dal loro avanzamento:
  >
  >* Idea
  >* Richiesto il
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

## Come Workfront aggiorna la condizione del progetto in base allo stato di avanzamento

Quando il Tipo di condizione del progetto è impostato su Manuale, è possibile determinare quale sia la condizione del progetto indipendentemente dallo Stato di avanzamento del progetto.

Tuttavia, si consiglia di impostare il Tipo di condizione del progetto su Stato di avanzamento in modo da poter avere un’indicazione chiara dell’avanzamento effettivo del progetto, in base all’avanzamento delle attività. Per informazioni sul modo in cui Workfront calcola lo stato di avanzamento dei progetti, vedere [Panoramica sullo stato di avanzamento dei progetti](../../../manage-work/projects/planning-a-project/project-progress-status.md).

In questo caso, i valori per Condizione progetto possono essere:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Condizione progetto</strong></td> 
   <td><strong>Stato avanzamento progetto</strong></td> 
   <td><strong>Indicatore di condizione Workfront</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Puntuale</td> 
   <td>Quando lo stato di avanzamento del progetto è Nei tempi previsti, la condizione del progetto è <strong>Su destinazione</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>A Rischio</td> 
   <td>Quando lo stato di avanzamento del progetto è <strong>Indietro</strong> o <strong>A rischio</strong>, la condizione del progetto è <strong>A rischio</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>In difficoltà</td> 
   <td>Quando lo stato di avanzamento del progetto è <strong>Late</strong>, la condizione del progetto è <strong>In difficoltà</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le condizioni possono essere personalizzate per il tuo ambiente, per cui potresti trovare più di tre opzioni per Condizione nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli elencati sopra. Per informazioni sulla personalizzazione delle Condizioni in , consulta l&#39;articolo [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapporto sulla condizione del progetto, Aggiornamento condizione progetto e Nota ultima condizione

Nella visualizzazione di un report di progetto, è possibile visualizzare i campi seguenti relativi alla condizione del progetto:

* **Condizione progetto:** mostra la condizione corrente del progetto.
* **Aggiornamento condizione progetto**: mostra l&#39;aggiornamento più recente fornito dal proprietario del progetto nel flusso di aggiornamento del progetto, insieme alla nuova condizione.\
  I commenti aggiunti agli aggiornamenti delle condizioni non vengono visualizzati nella colonna **Aggiornamento condizione**; viene visualizzato solo l&#39;aggiornamento principale.

* **Nota ultima condizione**: visualizza l&#39;ultimo aggiornamento immesso su un oggetto dal proprietario dell&#39;oggetto. Questo campo è utile per visualizzare l’attività o l’interazione più recente del proprietario su un oggetto.\
  La colonna **Nota ultima condizione** è vuota se il testo della nota dell&#39;ultima nota di un oggetto è stato eliminato. Una nuova nota immessa sull&#39;oggetto diventa l&#39;ultima nota e viene nuovamente visualizzata nella colonna.

Per informazioni su come creare un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

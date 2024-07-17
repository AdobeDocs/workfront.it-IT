---
content-type: overview
product-area: templates
keywords: sovrascrivi,campo,sovrascritto
navigation-topic: templates-navigation-topic
title: Panoramica dell’associazione di un modello a un progetto
description: Quando si allega un modello a un progetto esistente, si modificano alcune informazioni del progetto in base a quelle del modello. Alcune informazioni sul progetto rimangono invariate.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 5%

---

# Panoramica dell’associazione di un modello a un progetto

Quando si allega un modello a un progetto esistente, si modificano alcune informazioni del progetto in base a quelle del modello. Alcune informazioni sul progetto rimangono invariate.

Per informazioni su come allegare un modello a un progetto, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Considerazioni durante l’aggiunta di modelli ai progetti

Quando aggiungi modelli ai progetti, tieni presente quanto segue:

* Ai progetti è possibile allegare solo modelli attivi.
* È possibile allegare un modello a un progetto quando il progetto si trova nello stato Completato, Inattivo o In attesa di approvazione solo se l’amministratore di Adobe Workfront o un amministratore di gruppo ha abilitato questa funzionalità nell’area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* A meno che non si escluda l&#39;aggiunta di specifiche attività modello nel processo di creazione degli allegati, tutte le attività modello vengono aggiunte al progetto esistente.
* La maggior parte delle impostazioni dei modelli viene aggiunta al progetto. Alcune impostazioni di progetto vengono mantenute. Per informazioni, vedere la sezione [Comprendere le modifiche ai campi del progetto quando si allega un modello](#understand-changes-to-project-fields-when-attaching-a-template) in questo articolo.

## Comprendere le modifiche ai campi del progetto quando si allega un modello {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Associare un modello a un progetto non equivale a creare un progetto da un modello. Quando crei un progetto da un modello, tutti i campi modello vengono trasferiti al nuovo progetto. Quando si allega un modello, alcuni campi del progetto esistenti rimangono invariati.

Alcune impostazioni del modello vengono trasferite automaticamente al progetto, a meno che non vengano contrassegnate per essere escluse durante il processo di allegato del modello. Quando li contrassegni per l’esclusione, i valori dei campi del progetto vengono mantenuti.

Tuttavia, non tutti i campi del progetto sono disponibili per la gestione nel processo di associazione di un modello a un progetto. Per informazioni, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

Nella tabella seguente viene descritto il comportamento predefinito per i campi del progetto quando si allega un modello e i campi che è possibile gestire durante il processo di associazione per ignorare il comportamento predefinito:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo</td> 
   <td>Cosa accade durante il processo di associazione di un modello per impostazione predefinita</td> 
   <td>Possibilità di gestire gli aggiornamenti dei campi nel processo di creazione degli allegati </td> 
  </tr> 
  <tr> 
   <td>Descrizione</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Stato</p> </td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Trasferito dal modello, se il campo è vuoto nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Priorità</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo di condizione</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modalità pianificazione</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Le Date Pianificate</td> 
   <td>Può cambiare in base alle attività aggiunte</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Date effettive</td> 
   <td>Può cambiare in base alle attività aggiunte</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppo</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Azienda</td> 
   <td>Trasferito dal modello, se il campo è vuoto nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Lavoro Necessario</td> 
   <td>Può cambiare in base alle attività aggiunte</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Proprietario progetto</td> 
   <td>Trasferito dal modello, se il campo è vuoto nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sponsor del progetto</td> 
   <td>Trasferito dal modello, se il campo è vuoto nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Responsabile risorse</td> 
   <td>Aggiunto all'elenco dei gestori di risorse esistenti nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizzato</td> 
   <td>Sono stati aggiunti al progetto, oltre ai moduli già presenti nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bdg</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Valuta</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>MIP</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benef Pian</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vantaggio corrente</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Percorso milestone</td> 
   <td>Trasferito dal modello, se il campo è vuoto nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modalità di completamento</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modalità di completamento riepilogo</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo di aggiornamento</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Pianificazione</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Indisponibilità utente</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modalità Livellamento Risorse</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rischio (campo del progetto)</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppi di risorse</td> 
   <td>Aggiunto all'elenco dei pool di risorse esistenti nel progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipi di Ora</td> 
   <td> <p>Se viene deselezionata durante il processo di collegamento, l'impostazione Tipi di ora sul progetto rimane invariata. </p> <p>Se selezionata, l’impostazione del modello viene trasferita al progetto. Se il filtro Tipo di ora è impostato su Sì sia sul progetto che sul modello, i tipi di ora del modello vengono aggiunti a quelli del progetto.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Notifiche promemoria</td> 
   <td> <p>È stato aggiunto all’elenco dei promemoria esistenti sul progetto. </p> <p>Se viene deselezionata durante il processo di allegazione, le notifiche di promemoria del progetto rimangono invariate. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processo di approvazione predefinito attività</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Forms personalizzato predefinito attività</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Impegno di lavoro</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Consenti agli utenti di aggiungere problemi in linea</span> </td> 
   <td><span>Le informazioni sul progetto sono state conservate</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tutte le impostazioni</td> 
   <td>Le impostazioni del modello sovrascrivono quelle del progetto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>Aggiunto in fondo all'elenco delle attività, oltre alle attività di progetto esistenti</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td>Aggiunto al progetto, oltre ai documenti di progetto esistenti</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Rischi (oggetti nell'area Rischi del progetto)</td> 
   <td>Aggiunto al progetto, oltre ai rischi esistenti del progetto </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processo di approvazione</td> 
   <td>Trasferito da modello</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tariffe di fatturazione</td> 
   <td> <p>Trasferito da modello in aggiunta alle tariffe di fatturazione esistenti sul progetto. </p> <p>Se nel progetto e nel modello è presente un tasso diverso per la stessa mansione, il tasso nel progetto rimane invariato. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Record fatturazione</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Spese</td> 
   <td>Trasferito dal modello in aggiunta alle spese esistenti per il progetto</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Informazioni finanziarie</td> 
   <td> <p>Quando questa opzione è selezionata nel processo di creazione degli allegati, i campi seguenti vengono trasferiti o aggiunti al progetto: </p> 
    <ul> 
     <li> <p>Costi fissi</p> <p>Quando l’opzione è selezionata, il Costo fisso aggiornato del progetto viene calcolato con la seguente formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Reddito Fisso</p> <p>Quando l’opzione è selezionata, la Retribuzione fissa aggiornata del progetto viene calcolata utilizzando la seguente formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Tipo di costo per le attività</p> <p>Trasferito da modello</p> </li> 
     <li> <p>Tipo di retribuzione per le attività</p> <p>Trasferito da modello</p> </li> 
    </ul> <p>Se questo campo viene deselezionato durante il processo di collegamento, si verifica quanto segue:</p> 
    <ul> 
     <li> <p>I costi fissi e i ricavi fissi del progetto vengono mantenuti.</p> </li> 
     <li> <p>I tipi di costo e di ricavo per le attività aggiunte dal modello sono impostati su Nessun costo e Non fatturabile</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Ore</td> 
   <td>Le informazioni del progetto vengono conservate</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dettagli Coda, Gruppi Di Argomenti, Argomenti Coda, Regole Di Instradamento</td> 
   <td> <p>Trasferito da modello</p> <p>Se si seleziona l'opzione <strong>Impostazione delle proprietà e dei problemi della coda</strong> durante il processo di aggiunta, i dettagli della coda del modello sovrascriveranno quelli del progetto. In questo caso, le Regole di instradamento, gli Argomenti coda e i Gruppi di argomenti del modello vengono aggiunti a quelli del progetto. <br>Se il progetto è configurato come coda di richieste e il modello allegato al progetto non è configurato come coda di richieste, le informazioni sulla coda del progetto vengono rimosse se si lascia selezionata la casella <strong>Proprietà coda e configurazione problemi</strong>. <br>Se si deseleziona la casella <strong>Proprietà coda e configurazione problema</strong>, tutte le impostazioni di configurazione coda del progetto vengono mantenute e nessuna impostazione di configurazione coda del modello viene allegata.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Vincoli attività</td> 
   <td> <p>Trasferito da modello </p> <p>Se viene deselezionata durante il processo di collegamento, i vincoli delle attività vengono impostati su Il più presto possibile o Il più tardi possibile, a seconda dell'impostazione Pianifica da del progetto. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Predecessori attività</td> 
   <td> <p>Trasferito da modello</p> <p>Se viene deselezionata durante il processo di creazione degli allegati, tutte le connessioni dei predecessori tra le attività modello vengono rimosse.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Opzioni di condivisione</td> 
   <td> <p>Se deselezionata durante il processo di associazione, le autorizzazioni del progetto rimangono invariate.</p> <p>Se viene selezionato durante il processo di creazione degli allegati, le autorizzazioni del modello vengono aggiunte o sovrascritte a quelle del progetto. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se l'utente A dispone dell'autorizzazione di visualizzazione per il progetto, ma dispone delle autorizzazioni di gestione per il modello, dopo aver allegato il modello l'utente A otterrà l'accesso di gestione al progetto.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 

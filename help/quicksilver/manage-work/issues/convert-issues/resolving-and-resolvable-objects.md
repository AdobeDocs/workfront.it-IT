---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Panoramica sulla risoluzione e risoluzione di oggetti
description: Un oggetto risolvibile è un problema la cui risoluzione è legata a un oggetto di risoluzione. Un oggetto di risoluzione è un progetto, un'attività o un altro problema.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 4c4a8703cca33066f72f8f2088029382edbafc29
workflow-type: tm+mt
source-wordcount: '1732'
ht-degree: 1%

---

# Panoramica sulla risoluzione e risoluzione di oggetti

Un oggetto risolvibile è un problema la cui risoluzione è legata a un oggetto di risoluzione. Un oggetto di risoluzione è un progetto, un&#39;attività o un altro problema.

Quando si converte un problema in un&#39;attività o in un progetto, il problema diventa Oggetto risolvibile dell&#39;attività o del progetto.

Puoi anche collegare manualmente un problema a un oggetto di risoluzione, che può essere un’attività, un progetto o un problema. Per informazioni, consulta [Lega manualmente la risoluzione di un problema ad altri problemi, attività o progetti](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

Il problema originale diventa l&#39;oggetto risolvibile dell&#39;attività, del progetto o del problema, in questo scenario.

## Impostare Adobe Workfront per gestire oggetti risolvibili {#set-up-adobe-workfront-to-handle-resolvable-objects}

In qualità di amministratore di gruppo o di Workfront, è possibile decidere come gestire gli oggetti risolvibili nel sistema o per il gruppo.

È possibile scegliere di mantenere l&#39;oggetto risolvibile durante la conversione in un&#39;attività o in un progetto o di eliminarlo una volta creata l&#39;attività o il progetto. È possibile selezionare per consentire la modifica di queste impostazioni durante il processo di conversione dei problemi, che consentirà all&#39;utente di convertire i problemi per selezionare se mantenere o eliminare il problema mentre lo sta convertendo.

>[!NOTE]
>
>Gli oggetti risolvibili sono sempre problemi la cui risoluzione e stato possono dipendere dalla risoluzione e dallo stato dell&#39;oggetto di risoluzione a cui sono associati. La risoluzione degli oggetti può essere un problema, un&#39;attività o un progetto.

Per informazioni sull&#39;impostazione delle preferenze per la gestione degli oggetti risolvibili, vedere [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Gestire l’oggetto risolvibile durante la conversione in un progetto o in un’attività

A seconda del modo in cui l’amministratore di Workfront o di gruppo ha configurato le preferenze relative ai problemi a livello di sistema o di gruppo, potrebbe essere possibile gestire l’oggetto risolvibile durante la conversione di un problema in un progetto o in un’attività.

Esistono i seguenti scenari:

* Se l’amministratore di Workfront o di gruppo dispone della **Mantenere il problema originale e legarne la risoluzione all&#39;attività** e **Mantenere il problema originale e legarne la risoluzione al progetto** selezionati e **Consenti la modifica di queste impostazioni durante la conversione** deselezionata, non sarà possibile modificare queste impostazioni durante la conversione dei problemi in attività o progetti.\
   ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Se l’amministratore di Workfront o di gruppo dispone della **Mantenere il problema originale e legarne la risoluzione all&#39;attività** e **Mantenere il problema originale e legarne la risoluzione al progetto** selezionato o deselezionato e **Consenti la modifica di queste impostazioni durante la conversione** selezionando questa opzione, potrai modificare queste impostazioni durante la conversione dei problemi in attività o progetti.\
   ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Per ulteriori informazioni sulla conversione dei problemi in attività e progetti, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p> <p> <img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## Sincronizzare lo stato dell&#39;oggetto risolvibile con quello dell&#39;oggetto di risoluzione {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [Sincronizzazione degli stati quando si verifica un problema relativo alla risoluzione dell&#39;oggetto](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [Sincronizzazione degli stati quando l&#39;oggetto di risoluzione è un&#39;attività o un progetto](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Sincronizzazione degli stati quando si verifica un problema relativo alla risoluzione dell&#39;oggetto {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Se un problema viene associato manualmente a un altro problema, lo stato del secondo problema (Risoluzione dell’oggetto) attiva una modifica nello stato del primo problema (Oggetto risolvibile). Lo stato del primo problema corrisponde allo stato in cui viene modificato il secondo problema. Questo vale sia per gli stati di problema predefiniti che per quelli personalizzati.

### Sincronizzazione degli stati quando l&#39;oggetto di risoluzione è un&#39;attività o un progetto {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

Quando un problema è l&#39;oggetto risolvibile di un&#39;attività o di un progetto, le modifiche nello stato delle attività e dei progetti attivano modifiche nello stato del problema. In questo caso, gli stati predefiniti vengono attivati in modo diverso rispetto agli stati personalizzati.

* [Sincronizzare lo stato predefinito dell&#39;oggetto di risoluzione con lo stato predefinito dell&#39;oggetto risolvibile](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Sincronizzazione dello stato personalizzato dell&#39;oggetto di risoluzione con lo stato personalizzato dell&#39;oggetto risolvibile](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Sincronizzare lo stato predefinito dell&#39;oggetto di risoluzione con lo stato predefinito dell&#39;oggetto risolvibile {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Indipendentemente dal fatto che lo stato &quot;Aggiorna automaticamente il problema risolvibile quando lo stato dell&#39;opzione Risolvi oggetto cambia&quot; sia selezionato, ogni volta che lo stato predefinito cambia sugli oggetti di risoluzione (progetti o attività), lo stato dell&#39;oggetto risolvibile (problemi) cambia di conseguenza. Solo gli stati predefiniti sono già mappati per attivare tale modifica.

I seguenti stati predefiniti per le attività attivano le seguenti modifiche negli stati predefiniti per i problemi, quando il problema è impostato come oggetto di risoluzione di un&#39;attività:

| **STATO ATTIVITÀ** | **STATO DEL PROBLEMA** |
|---|---|
| Nuovo | Nuovo |
| In corso | In corso |
| Completato | Chiuso |

I seguenti stati predefiniti per i progetti attivano le seguenti modifiche negli stati predefiniti per i problemi, quando il problema è impostato come Oggetto risolvibile di un progetto. Alcuni stati del progetto non attivano le modifiche allo stato dei problemi. I problemi rimangono nello stato precedente alla trasformazione del progetto in uno di questi stati:

| **STATO DEL PROGETTO** | **STATO DEL PROBLEMA** |
|---|---|
| In Pianificazione | Nuovo |
| Attuali | In corso |
| In sospeso | In sospeso |
| Richiesto | Non attiva una modifica allo stato del problema |
| Approvato | Non attiva una modifica allo stato del problema |
| Rifiutato | Non attiva una modifica allo stato del problema |
| Idea | Non attiva una modifica allo stato del problema |
| Morto | Chiuso |
| Completato | Chiuso |

>[!NOTE]
>
>Dopo la chiusura dello stato del problema (in seguito alla chiusura dell&#39;attività o del progetto), indipendentemente dallo stato in cui l&#39;attività o il progetto cambia dopo la loro chiusura, il problema rimane chiuso.

#### Sincronizzazione dello stato personalizzato dell&#39;oggetto di risoluzione con lo stato personalizzato dell&#39;oggetto risolvibile {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

Quando si modifica lo stato dell&#39;attività o del progetto in uno stato personalizzato, lo stato del problema diventa un problema personalizzato solo se sono soddisfatte le due condizioni seguenti:

* L&#39;opzione &quot;Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;oggetto di risoluzione cambia&quot; è selezionata. Per ulteriori informazioni su come abilitare questa impostazione, vedi [Impostare Adobe Workfront per gestire oggetti risolvibili](#set-up-adobe-workfront-to-handle-resolvable-objects).

* Lo stato personalizzato del progetto o dell’attività ha lo stesso codice a tre lettere dello stato personalizzato del problema.

Puoi creare stati personalizzati con la stessa chiave per problemi e progetti o attività. Quando il progetto o l’attività (come oggetto di risoluzione) viene modificato in stato personalizzato, la modifica riflette anche lo stato del problema. La chiave di stato deve essere la stessa per il problema e lo stato del progetto o dell&#39;attività.

Ad esempio, crea uno stato personalizzato del progetto denominato &quot;Avviato&quot; con il codice a tre lettere &quot;LCD&quot; che equivale a &quot;Corrente&quot;. Inoltre, crea uno stato personalizzato del problema denominato &quot;Progetto avviato&quot;, anche con il codice lettera &quot;LCD&quot; che equivale a &quot;In corso&quot;. Quando contrassegni il progetto come &quot;Avviato&quot;, lo stato cambia automaticamente in &quot;Progetto avviato&quot;. Se lo stato del problema &quot;Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;impostazione Resolving Object changes&quot; non è stato abilitato, lo stato del problema diventa &quot;In corso&quot; (lo stato predefinito).

Per ulteriori informazioni sulla creazione di uno stato personalizzato, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Sincronizzare la percentuale di completamento di un oggetto di risoluzione con quella dell&#39;oggetto di risoluzione

Se un problema viene risolto da un&#39;attività o da un progetto, la percentuale di completamento del problema viene aggiornata sul problema risolvibile quando si verifica uno dei seguenti casi: 

* Quando un utente salva una modifica all&#39;attività o al progetto.
* Viene ricalcolata la timeline del progetto.

Se e il problema viene risolto da un altro problema, la percentuale di completamento viene aggiornata quando uno dei problemi si aggiorna.

## Individuare l&#39;oggetto risolvibile su un&#39;attività o su un progetto

La posizione dell&#39;oggetto di risoluzione è identica per le attività e i progetti.

1. Passa a un progetto o a un&#39;attività creata convertendo un problema nel progetto o nell&#39;attività.
1. Fai clic sul pulsante **Dettagli progetto** o **Dettagli attività** e fai clic su per espanderla.
1. Fai clic su **Panoramica**.
1. Nella parte inferiore della scheda , individua **Questo Risolve** campo: il problema relativo all&#39;oggetto risolvibile del progetto o dell&#39;attività è elencato in questo campo.

   >[!NOTE]
   >
   >I problemi non possono essere convertiti in altri problemi, ma possono essere associati manualmente a un problema di risoluzione. Un progetto, un&#39;attività o un problema può avere più problemi come Oggetti Risolvibili. Quando il progetto, l&#39;attività o il problema vengono risolti, viene risolto anche l&#39;oggetto risolvibile (problema). Il problema risolvibile rimane chiuso anche se il progetto, l&#39;attività o il problema che lo ha risolto viene riaperto.

## Identificare un problema con un oggetto di risoluzione in un elenco

In un elenco di problemi, è possibile identificare i problemi che sono etichettati come risoluzione di oggetti tramite icone di stato, individuando questa icona in **Icone di stato** o **Flag** colonne:

![](assets/ro1.png)

## Visualizzare informazioni sull’oggetto risolvibile e risolvibile in un rapporto

È possibile visualizzare informazioni sugli oggetti risolvibili o risolvibili nella visualizzazione o nel rapporto per progetti, attività o problemi.\
La tabella seguente mostra i campi che è possibile visualizzare e in quali viste è possibile visualizzarli:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo nella visualizzazione</strong> </th> 
   <th><strong>Vista Issue</strong> </th> 
   <th><strong>Vista Attività</strong> </th> 
   <th><strong>Vista Project</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Con valori risolvibili</strong>: Visualizza un <strong>True</strong> se al progetto o all'attività sono associati problemi risolvibili e un <strong>False</strong> se non lo fanno.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>Nome dell'emissione originale, data di ingresso dell'emissione originale, nome dell'autore</strong>: Visualizza il nome e la data di ingresso del problema originale, nonché il nome dell'utente che ha creato il problema in una visualizzazione personalizzata in modalità testo.<br>Per ulteriori informazioni sulla creazione di una visualizzazione personalizzata in modalità testo per un progetto o un report di attività o un elenco per visualizzare informazioni sul problema originale, vedere <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">Visualizza: visualizzare le informazioni originali sul problema negli elenchi di attività e progetti</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Risolvibili:</strong> Visualizza un elenco di tutti gli oggetti risolvibili in una visualizzazione personalizzata in modalità testo per un report o elenco di progetti o attività.</p> <p>Per ulteriori informazioni sulla creazione di questa visualizzazione, consulta <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">Visualizza: Oggetti risolvibili in un'attività o in un rapporto di progetto</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>Generatore di problemi convertito</strong>: Visualizza informazioni sull'utente che ha originariamente registrato il problema che è stato successivamente convertito nell'attività. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risolvi progetto</strong>: Visualizza informazioni sul progetto di risoluzione convertito dal problema originale o designato manualmente come oggetto di risoluzione di un problema.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risolvi attività</strong>: Visualizza informazioni sull'attività di risoluzione convertita dal problema originale o designata manualmente come oggetto di risoluzione di un problema.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risoluzione del problema</strong>: Visualizza informazioni sul problema di risoluzione che è stato designato manualmente come oggetto di risoluzione di un problema.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

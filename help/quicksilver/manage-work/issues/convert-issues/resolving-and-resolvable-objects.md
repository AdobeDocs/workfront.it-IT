---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Panoramica sugli oggetti risolvibili e risolvibili
description: Un oggetto risolvibile è un problema la cui risoluzione è associata a un oggetto risolutivo. Un oggetto risolutivo è un progetto, un'attività o un altro problema.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '1761'
ht-degree: 1%

---

# Panoramica sugli oggetti risolvibili e risolvibili

<!-- Audited: 5/2025 -->

Un oggetto risolvibile è un problema la cui risoluzione è associata a un oggetto risolutivo. Un oggetto risolutivo è un progetto, un&#39;attività o un altro problema.

Quando si converte un problema in un&#39;attività o in un progetto, il problema diventa l&#39;oggetto risolvibile dell&#39;attività o del progetto.

È inoltre possibile collegare manualmente un problema a un oggetto risolutivo, che può essere un&#39;attività, un progetto o un problema. Per informazioni, vedere [Collegare manualmente la risoluzione di un problema ad altri problemi, attività o progetti](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

In questo scenario, il problema originale diventa l’oggetto risolvibile dell’attività, del progetto o del problema.

## Imposta Adobe Workfront per gestire gli oggetti risolvibili {#set-up-adobe-workfront-to-handle-resolvable-objects}

In qualità di amministratore di Workfront o di amministratore di gruppo, puoi decidere come gestire gli oggetti risolvibili nel tuo sistema o per il tuo gruppo.

È possibile scegliere di mantenere l&#39;oggetto risolvibile durante la conversione in un&#39;attività o un progetto oppure di eliminarlo dopo la creazione dell&#39;attività o del progetto. È possibile scegliere di consentire la modifica di queste impostazioni durante la conversione dei problemi, in modo che l’utente possa convertire i problemi per scegliere se mantenerli o eliminarli mentre li converte.

>[!NOTE]
>
>Gli oggetti risolvibili sono sempre problemi la cui risoluzione e il cui stato possono dipendere dalla risoluzione e dallo stato dell&#39;oggetto risolutivo a cui sono associati. Gli oggetti risolti possono essere problemi, attività o progetti.

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

## Gestire l’oggetto risolvibile durante la conversione in un progetto o un’attività

A seconda del modo in cui l’amministratore di Workfront o di gruppo ha configurato le preferenze relative ai problemi a livello di sistema o di gruppo, potresti essere in grado di gestire l’oggetto risolvibile durante la conversione di un problema in un progetto o in un’attività.

Esistono i seguenti scenari:

* Se l’amministratore di Workfront o di gruppo dispone del comando Mantieni il problema originale e collegane la risoluzione all’attività e del comando Mantieni il problema originale e collegane la risoluzione al progetto selezionato e il comando Consenti la modifica di queste impostazioni durante la conversione non è selezionato, non sarà possibile modificare queste impostazioni durante la conversione dei problemi in attività o progetti.\
  ![Area problemi preferenze progetto](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Se l&#39;amministratore del Workfront o del gruppo dispone del comando Mantieni il problema originale e collegane la risoluzione all&#39;attività e del comando Mantieni il problema originale e collegane la risoluzione al progetto selezionato o non selezionato e del comando Consenti la modifica di queste impostazioni durante la conversione selezionato, sarà possibile modificare queste impostazioni durante la conversione dei problemi in attività o progetti.\
  ![Opzione per mantenere il problema](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Per ulteriori informazioni sulla conversione dei problemi in attività e progetti, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
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

## Sincronizza lo stato dell&#39;oggetto risolvibile con quello dell&#39;oggetto risolutivo {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [Sincronizzare gli stati quando l&#39;oggetto risolutivo è un problema](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [Sincronizzare gli stati quando l&#39;oggetto risolutivo è un&#39;attività o un progetto](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Sincronizzare gli stati quando l&#39;oggetto risolutivo è un problema {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Quando un problema è legato manualmente a un altro problema, lo stato del secondo problema (Oggetto risolutivo) attiva una modifica dello stato del primo problema (Oggetto risolvibile). Lo stato del primo problema corrisponde allo stato in cui viene modificato il secondo problema. Questo vale sia per gli stati di problema predefiniti che per quelli personalizzati.

### Sincronizzare gli stati quando l&#39;oggetto risolutivo è un&#39;attività o un progetto {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

Quando un problema è l’oggetto risolvibile di un’attività o di un progetto, le modifiche allo stato delle attività e dei progetti attivano le modifiche allo stato del problema. In questo caso, gli stati predefiniti vengono attivati in modo diverso dagli stati personalizzati.

Quando lo stato personalizzato di un progetto è uguale a uno stato predefinito che non attiva una modifica dello stato del problema, la modifica dello stato del progetto non attiva una modifica dello stato del problema.

* [Sincronizzare lo stato predefinito dell&#39;oggetto risolutivo con lo stato predefinito dell&#39;oggetto risolvibile](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Sincronizza lo stato personalizzato dell&#39;oggetto risolutivo con lo stato personalizzato dell&#39;oggetto risolvibile](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Sincronizza lo stato predefinito dell&#39;oggetto risolutivo con lo stato predefinito dell&#39;oggetto risolvibile {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Indipendentemente dal fatto che sia selezionata l&#39;opzione Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;opzione Modifiche all&#39;oggetto risolvibile, ogni volta che lo stato predefinito cambia sugli oggetti risolvibili (progetti o attività), lo stato dell&#39;oggetto risolvibile (problemi) cambia di conseguenza. Solo gli stati predefiniti sono già mappati per attivare tale modifica.

I seguenti stati di attività predefiniti attivano le seguenti modifiche negli stati di problema predefiniti quando il problema è impostato come oggetto di risoluzione dell’attività:

| **STATO ATTIVITÀ** | **STATO PROBLEMA** |
|---|---|
| Nuovo | Nuovo |
| In corso | In corso |
| Completato | Chiuso |

I seguenti stati predefiniti del progetto attivano le seguenti modifiche negli stati predefiniti del problema quando il problema è impostato come oggetto risolvibile di un progetto. Alcuni stati del progetto non attivano modifiche agli stati del problema. I problemi rimangono nello stato in cui si trovavano prima che il progetto diventasse uno di questi:

| **STATO PROGETTO** | **STATO PROBLEMA** |
|---|---|
| In Pianificazione | Nuovo |
| Attuali | In corso |
| In sospeso | In sospeso |
| Richiesto il | Non attiva una modifica allo stato del problema |
| Approvato | Non attiva una modifica allo stato del problema |
| Rifiutato | Non attiva una modifica allo stato del problema |
| Idea | Non attiva una modifica allo stato del problema |
| Morto | Chiuso |
| Completato | Chiuso |

>[!NOTE]
>
>Quando lo stato del problema diventa Chiuso (a seguito della chiusura dell&#39;attività o del progetto), indipendentemente da come cambia lo stato dell&#39;attività o del progetto dopo la chiusura, il problema rimane Chiuso.

#### Sincronizza lo stato personalizzato dell&#39;oggetto risolutivo con lo stato personalizzato dell&#39;oggetto risolvibile {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

Quando si cambia lo stato dell&#39;attività o del progetto in uno stato personalizzato, lo stato del problema cambia in uno stato personalizzato solo se vengono soddisfatte le due condizioni seguenti:

* Lo stato Aggiorna automaticamente lo stato del problema risolvibile quando viene selezionato lo stato dell&#39;opzione Modifica oggetto risolutivo. Per ulteriori informazioni, vedere [Configurare Adobe Workfront per la gestione degli oggetti risolvibili](#set-up-adobe-workfront-to-handle-resolvable-objects).

* Lo stato personalizzato del progetto o dell’attività ha lo stesso codice di tre lettere dello stato personalizzato del problema.

Puoi creare stati personalizzati con la stessa chiave per problemi e progetti o attività. Quando il progetto o l’attività (come oggetto risolutivo) viene riportato allo stato personalizzato, la modifica si riflette anche sullo stato del problema. La chiave dello stato deve essere la stessa per lo stato del problema e per quello del progetto o dell’attività.

Ad esempio, immagina di creare uno stato personalizzato del progetto denominato Avviato con l’LCD con codice di tre lettere, che equivale a Corrente. Successivamente, viene creato un problema con lo stato personalizzato Progetto avviato, anche con il codice di lettera LCD, che equivale a In corso. Quando contrassegni il progetto come Avviato, il problema cambia automaticamente lo stato in Progetto avviato. Se lo stato Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;impostazione delle modifiche all&#39;oggetto risolutivo non era abilitato, lo stato del problema passerebbe a In corso.

Per ulteriori informazioni sulla creazione di uno stato personalizzato, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Sincronizzare la percentuale di completamento di un oggetto risolutivo con quella dell&#39;oggetto risolvibile

Se un problema viene risolto da un&#39;attività o da un progetto, la percentuale di completamento del problema viene aggiornata in base al problema risolvibile quando si verifica una delle seguenti situazioni:

* Quando un utente salva una modifica nell&#39;attività o nel progetto.
* Quando la timeline del progetto viene ricalcolata.

Se un problema viene risolto da un altro problema, la percentuale di completamento viene aggiornata quando si aggiorna uno dei problemi.

## Individuare l&#39;oggetto risolvibile in un&#39;attività o in un progetto

>[!NOTE]
>
>Per eseguire i passaggi descritti in questa sezione, è necessario disporre almeno dell&#39;accesso di visualizzazione alle attività e ai progetti e delle autorizzazioni di visualizzazione per l&#39;attività o il progetto che contiene l&#39;oggetto risolvibile che si desidera visualizzare.

L&#39;individuazione dell&#39;oggetto di risoluzione è identica per attività e progetti.

1. Passa a un progetto o a un’attività creata convertendo un problema.
1. Sul lato sinistro della pagina, selezionare la scheda **Dettagli attività** o **Dettagli progetto**.
1. Nella parte inferiore della sezione **Panoramica**, individua il campo **Questa risoluzione** in cui viene visualizzato l&#39;oggetto risolvibile dell&#39;attività o del progetto.

   ![Questo risolve il campo](assets/this-resolves-field.png)

   >[!NOTE]
   >
   >I problemi non possono essere convertiti in altri problemi, ma possono essere associati manualmente a un problema risolutivo. Un progetto, un&#39;attività o un problema può avere più problemi come oggetti risolvibili. Quando il progetto, l’attività o il problema viene risolto, viene risolto anche l’oggetto risolvibile (problema). Il problema risolvibile rimane chiuso anche se il progetto, l’attività o il problema che lo ha risolto viene riaperto.

## Identificare un problema relativo a un oggetto risolutivo in un elenco

In un elenco di problemi è possibile identificare i problemi etichettati come oggetti di risoluzione tramite icone di stato individuando questa icona nelle colonne **Icone di stato** o **Flag**:

![Oggetto risolutivo](assets/resolving-icon.png)

## Visualizzare informazioni sugli oggetti risolvibili e risolvibili in un report

È possibile visualizzare informazioni sugli oggetti risolvibili o risolvibili nella visualizzazione o nel report per progetti, attività o problemi.

Nella tabella seguente vengono illustrati i campi che è possibile visualizzare e le visualizzazioni in cui è possibile visualizzarli:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo nella visualizzazione</strong> </th> 
   <th><strong>Visualizzazione problemi</strong> </th> 
   <th><strong>Visualizzazione attività</strong> </th> 
   <th><strong>Visualizzazione progetto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Ha elementi risolvibili</strong>: visualizza un valore True se al progetto o all'attività sono associati problemi risolvibili e un valore False in caso contrario.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>Nome problema originale, Data voce problema originale, Nome creatore</strong>: visualizza il nome e la data di voce del problema originale, nonché il nome dell'utente che ha creato il problema in una visualizzazione personalizzata in modalità testo.<br>Per ulteriori informazioni, vedere <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">Visualizza: visualizza le informazioni originali sul problema negli elenchi di attività o progetti</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Risolvibili:</strong> Visualizza un elenco di tutti gli oggetti risolvibili in una visualizzazione personalizzata in modalità testo per un report o un elenco di progetti o attività.</p> <p>Per ulteriori informazioni, vedere <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">Visualizzazione: oggetti risolvibili in un report di attività o di progetto</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>Iniziatore problema convertito</strong>: visualizza informazioni sull'utente che ha registrato originariamente il problema e che è stato successivamente convertito nell'attività. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risolvi progetto</strong>: visualizza informazioni sul progetto risolutivo convertito dal problema originale o designato manualmente come oggetto risolutivo di un problema.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risolvi attività</strong>: visualizza informazioni sull'attività di risoluzione convertita dal problema originale o designata manualmente come oggetto di risoluzione di un problema.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Risolvi problema</strong>: visualizza informazioni sul problema risolutivo designato manualmente come oggetto risolutivo di un problema.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

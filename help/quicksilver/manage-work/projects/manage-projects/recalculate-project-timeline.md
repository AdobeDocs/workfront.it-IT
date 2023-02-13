---
product-area: projects
navigation-topic: manage-projects
title: Ricalcolare le timeline dei progetti
description: Il ricalcolo delle timeline consente ai responsabili di vedere come diversi fattori correlati al progetto influiscono sulla timeline del progetto. La timeline di un progetto si riferisce alle date pianificate e proiettate.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Ricalcolare le timeline dei progetti

Il ricalcolo delle timeline consente ai responsabili di vedere come diversi fattori correlati al progetto influiscono sulla timeline del progetto. La timeline di un progetto si riferisce alle date pianificate e proiettate.

Le modifiche apportate alle pianificazioni, al tempo di inattività del personale e ad altri elementi che non rientrano nell’ambito di un progetto non influiscono immediatamente sulla timeline del progetto. La timeline del progetto viene interessata dal ricalcolo della timeline. Le influenze esterne hanno effetto sul progetto solo dopo il ricalcolo.

Questo articolo descrive i modi in cui avviene il ricalcolo della timeline.

## Requisiti di accesso

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Il ricalcolo automatico della timeline avviene senza un accesso speciale per gli utenti coinvolti nell’attività di progetto.

Tuttavia, per ricalcolare manualmente la timeline di un progetto è necessario disporre del seguente accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>L’amministratore di sistema ricalcola la cronologia di tutti i progetti nel sistema</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Ricalcolo automatico

Per impostazione predefinita, le timeline del progetto vengono ricalcolate automaticamente ogni giorno quando l’ambito del progetto cambia o ogni notte. L’amministratore di Workfront determina se calcolare automaticamente le timeline ogni notte o con ogni modifica dell’ambito gestendo le impostazioni delle timeline nell’area Preferenze progetto di Configurazione. Per ulteriori informazioni, consulta [Configurare i calcoli della timeline per i progetti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Se la tempistica di un progetto è superiore a 15 anni, il ricalcolo automatico è disattivato per quel progetto. È possibile selezionare solo un tipo di aggiornamento manuale per un progetto di durata superiore a 15 anni. Se cambi le date del progetto con meno di 15 anni, devi ricalcolare manualmente la timeline una volta prima che venga calcolata automaticamente.

* [Ricalcolo automatico delle timeline del progetto](#automatic-recalculation-of-project-timelines)
* [Azioni che attivano un ricalcolo automatico delle timeline dei progetti](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### Ricalcolo automatico delle timeline del progetto {#automatic-recalculation-of-project-timelines}

Adobe Workfront ricalcola giornalmente le timeline solo per i progetti in cui sono soddisfatte tutte le seguenti condizioni:

* Hanno lo stato Current
* Tipo di aggiornamento del progetto è impostato su Automatico o Automatico e su Modifica

   Per informazioni sul tipo di progetto Tipo di aggiornamento, consulta [Panoramica sul tipo di aggiornamento del progetto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Avere una Data ultimo aggiornamento negli ultimi tre mesi\
   L’amministratore Workfront può modificare questa funzionalità predefinita, come descritto in [Configurare i calcoli della timeline per i progetti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* L&#39;ultima data di calcolo della timeline del progetto non si trova nel giorno di calendario corrente. Ciò significa che l’ultima data di calcolo della timeline del progetto è precedente alle 00:00 del giorno corrente.

Puoi configurare la frequenza di aggiornamento della timeline del progetto. Quando la timeline del progetto viene aggiornata, viene ricalcolata in base alle modifiche apportate al progetto.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Per informazioni, consulta [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Azioni che attivano un ricalcolo automatico delle timeline dei progetti {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Varie modifiche dell’ambito nel ciclo di vita di un progetto ricalcolano automaticamente la timeline del progetto, comprese le azioni seguenti:

* Aggiornamento dello stato dell&#39;attività.
* Spostamento di un&#39;attività in un progetto diverso.
* Aggiornamento della data pianificata o delle date di completamento pianificate delle attività.
* Aggiornamento del tipo di durata, del vincolo di attività o del numero di assegnatari nelle attività.
* Aggiornamento delle relazioni predecessori delle attività.
* Aggiunta di un&#39;approvazione a un&#39;attività che aggiunge anche tempo alla data di completamento pianificata dell&#39;attività.\
   Per ulteriori informazioni sulle impostazioni di approvazione, vedi [Configurare le impostazioni di approvazione globali](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Ricalcolo manuale {#manual-recalculation}

In qualità di proprietario del progetto, puoi ricalcolare manualmente le timeline per i singoli progetti. L’amministratore di Workfront può ricalcolare manualmente tutte le timeline in Workfront.

* [Ricalcolare le timeline per singoli progetti o in serie](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Ricalcolare manualmente le timeline in blocco nella casella Modifica progetti](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Ricalcola le timeline per tutti i progetti nel sistema (solo per amministratori Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Ricalcolare le timeline per singoli progetti o in serie {#recalculate-timelines-for-individual-projects-or-in-bulk}

Puoi ricalcolare la timeline di un progetto in Workfront dalla pagina del progetto o da un elenco o da un rapporto di progetto.

1. Passa al progetto per il quale desideri ricalcolare la timeline e fai clic sul pulsante **Altro** icona ![](assets/qs-more-menu.png) a sinistra del nome del progetto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Vai a un elenco o a un rapporto di progetti e seleziona uno o più progetti, quindi fai clic su **Altro** icona ![](assets/qs-more-menu.png) in cima all&#39;elenco.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >A seconda della complessità dei progetti, si consiglia di non selezionare un gran numero di progetti quando si ricalcolano le timeline in blocco per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Fai clic su **Ricalcola timeline**.

   Una volta ricalcolata la timeline, viene visualizzato un messaggio che indica che il ricalcolo è stato eseguito correttamente.

   >[!TIP]
   >
   >Prima che il ricalcolo della timeline sia completato, alcune date pianificate o previste potrebbero apparire in grigio. Ciò significa che il ricalcolo non è ancora completato e che le date sono soggette a modifiche.

### Ricalcolare manualmente le timeline in blocco nella casella Modifica progetti {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Puoi ricalcolare manualmente le timeline di diversi progetti modificandole in blocco.

>[!TIP]
>
>A seconda della complessità dei progetti, si consiglia di non selezionare un gran numero di progetti quando li si modifica in serie per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Vai a un elenco di progetti.
1. Seleziona diversi progetti nell’elenco, quindi fai clic su **Modifica**.
1. Fai clic su **Impostazioni**, quindi seleziona **Ricalcola timeline**.

1. Fai clic su **Salva modifiche**.

### Ricalcola le timeline per tutti i progetti nel sistema (solo per amministratori Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Gli amministratori di Workfront possono eseguire la diagnostica Ricalcola timeline per ricalcolare immediatamente tutte le timeline nel sistema Workfront. Questo consente a tutti i project manager di vedere immediatamente l’influenza dei cambiamenti esterni sia sulle date pianificate che su quelle previste.

Per ulteriori informazioni sul ricalcolo delle timeline per l’intero sito Workfront, consulta la sezione &quot;Ricalcolare le timeline per l’intera istanza Workfront&quot; in [Configurare i calcoli della timeline per i progetti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->

---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Panoramica dei proprietari e degli sponsor del progetto
description: Puoi designare un proprietario del progetto e uno sponsor del progetto per un progetto.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Panoramica dei proprietari e degli sponsor del progetto

Puoi designare un proprietario del progetto e uno sponsor del progetto per un progetto.

Il proprietario del progetto è l’utente responsabile del completamento del progetto nei tempi e nel budget previsti.

Lo sponsor del progetto è un importante soggetto interessato per il progetto che ha risorse investite nel progetto. In genere, il completamento del progetto avvantaggia lo sponsor del progetto.

Per informazioni su come aggiornare il proprietario del progetto o lo sponsor di un progetto, consulta [Aggiornare i proprietari e gli sponsor del progetto](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Proprietari del progetto

Puoi designare il responsabile di un progetto specificando un proprietario di progetto in un progetto o in un modello.

Puoi definire un solo proprietario del progetto.

È possibile utilizzare il campo Proprietario progetto per quanto segue:

* Puoi designare un solo utente come proprietario del progetto.
* Puoi designare i Proprietari del progetto come approvatore delle ore per il progetto.
* È possibile designare il proprietario del progetto come approvatore generico quando si definiscono i processi di approvazione di progetti, task o problemi. Per informazioni sulle approvazioni, consulta [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Quando si assegna un&#39;approvazione al proprietario del progetto e nessuno viene designato come proprietario di un progetto, l&#39;approvazione viene riassegnata all&#39;amministratore principale di Workfront come indicato nella sezione Informazioni cliente nell&#39;area Configurazione. Per informazioni, consulta [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* Puoi abilitare alcune notifiche che vengono inviate solo al proprietario del progetto.

   Per ulteriori informazioni sulle notifiche e-mail, consulta la sezione . [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) nell&#39;articolo [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* È possibile visualizzare il campo Proprietario del progetto in un rapporto o in un elenco.

   È inoltre possibile visualizzare il campo Proprietario del progetto in una visualizzazione, in un raggruppamento o in un prompt.

   Ad esempio, puoi copiare la seguente espressione della modalità di testo in un filtro per visualizzare i progetti di proprietà dell’utente connesso: 

   ```
   ownerID=$$USER.ID
   ```

Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## sponsor del progetto

È possibile designare qualsiasi utente nel sistema come sponsor di progetto. Lo sponsor del progetto è di solito un manager, un esecutivo o un stakeholder che deve sapere cosa sta succedendo con il progetto.

Quando si assegna uno sponsor di progetto, considera quanto segue:

* Lo sponsor del progetto non ottiene alcun accesso aggiuntivo al progetto, ma viene aggiunto alle notifiche e-mail del progetto. Per informazioni sulle notifiche, consulta l’articolo [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* È possibile designare un solo sponsor di progetto.
* È possibile designare lo sponsor del progetto come approvatore generico quando si definiscono i processi di approvazione di progetti, task o problemi. Per informazioni sulle approvazioni, consulta [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Quando si assegna un&#39;approvazione allo sponsor del progetto e nessuno viene designato come sponsor di un progetto, l&#39;approvazione viene riassegnata al proprietario del progetto. Se nessuno è designato come proprietario del progetto, l’approvazione viene assegnata all’amministratore Workfront.

* È possibile visualizzare il campo Sponsor del progetto in un rapporto o in un elenco.

   È inoltre possibile visualizzare il campo Sponsor del progetto in una visualizzazione, in un raggruppamento o in un prompt.

   Ad esempio, puoi copiare la seguente espressione di modalità testo in un filtro per visualizzare i progetti sponsorizzati dall’utente connesso:

   ```
   sponsorID=$$USER.ID
   ```

    

   Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

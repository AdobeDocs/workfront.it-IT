---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Panoramica dei proprietari e degli sponsor dei progetti
description: Puoi designare un Proprietario del progetto e uno Sponsor del progetto per un progetto.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Panoramica dei proprietari e degli sponsor dei progetti

<!-- Audited: 1/2024 -->

Puoi designare un Proprietario del progetto e uno Sponsor del progetto per un progetto.

Il proprietario del progetto è la persona responsabile del completamento del progetto nei tempi e nel budget stabiliti.

Lo sponsor del progetto è un&#39;importante parte interessata per il progetto che dispone di risorse investite nel progetto. In genere, il completamento del progetto va a vantaggio dello sponsor del progetto.

Per informazioni su come aggiornare il proprietario o lo sponsor del progetto per un progetto, vedi [Aggiorna proprietari e sponsor del progetto](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Proprietari progetto

È possibile designare il manager di un progetto specificando un Proprietario del progetto in un progetto o in un modello.

Puoi definire un solo Proprietario progetto per un progetto.

Utilizzando il campo Proprietario progetto è possibile:

* È possibile designare un solo utente come Proprietario del progetto.
* È possibile designare i proprietari del progetto come approvatori delle ore per il progetto.
* È possibile designare il proprietario del progetto come approvatore generico quando si definiscono i processi di approvazione di progetti, attività o problemi. Per informazioni sulle approvazioni, consulta [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Quando si assegna un&#39;approvazione al proprietario del progetto e nessuno viene designato come proprietario di un progetto, l&#39;approvazione viene riassegnata all&#39;amministratore principale di Workfront come indicato nella sezione Informazioni cliente nell&#39;area Configura. Per informazioni, consulta [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* Puoi abilitare alcune notifiche inviate solo al proprietario del progetto.

  Per ulteriori informazioni sulle notifiche e-mail, consulta la sezione [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) nell’articolo [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* È possibile visualizzare il campo Proprietario progetto in un report o in un elenco.

  È inoltre possibile visualizzare il campo Proprietario progetto in una visualizzazione, in un raggruppamento o in un prompt.

  Ad esempio, puoi copiare la seguente espressione in modalità testo in un filtro per visualizzare i progetti di proprietà dell’utente connesso: 

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

## Sponsor del progetto

Puoi designare qualsiasi utente del sistema come sponsor del progetto. Lo sponsor del progetto è solitamente un manager, un dirigente o un soggetto interessato che deve sapere cosa sta succedendo con il progetto.

Quando si assegna uno sponsor di progetto, considera quanto segue:

* Lo sponsor del progetto non ottiene alcun accesso aggiuntivo al progetto, ma viene aggiunto alle notifiche e-mail del progetto. Per informazioni sulle notifiche, consulta l’articolo [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* È possibile designare un solo sponsor progetto.
* È possibile designare lo sponsor del progetto come un approvatore generico quando si definiscono i processi di approvazione di progetti, attività o problemi. Per informazioni sulle approvazioni, consulta [Modificare un processo di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Quando si assegna un&#39;approvazione allo sponsor del progetto e nessuno viene designato come sponsor di un progetto, l&#39;approvazione viene riassegnata al proprietario del progetto. Se nessuno è designato come proprietario del progetto, l’approvazione viene assegnata all’amministratore di Workfront.

* Puoi visualizzare il campo Sponsor progetto in un rapporto o in un elenco.

  È inoltre possibile visualizzare il campo Sponsor progetto in una visualizzazione, un raggruppamento o un prompt.

  Ad esempio, puoi copiare la seguente espressione in modalità testo in un filtro per visualizzare i progetti sponsorizzati dall’utente connesso:

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
